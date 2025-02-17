# Keycap Archivist Database FORK - WORKING ON KEYAUTHOR - KEYCAP AUTHORISATION DATABASE

![Discord](https://img.shields.io/discord/707159843751854141)


Database currently contains:

- ![Element](https://img.shields.io/badge/Artisans-181-bfff00)
- ![Element](https://img.shields.io/badge/Sculpts-1856-bfff00)
- ![Element](https://img.shields.io/badge/Colorways-38005-bfff00)

CSV/JSON database of artisan keycaps based on : [https://keycap.info/](https://keycap.info/)

Synchronization is done on a daily basis using a cron github action. If there is a change, the database update itself.

## Develop

To use you need to declare a Google API Key for Drive and export it as an env variable `G_API_KEY`

## Usage

To use the master version of the catalog you can CURL those urls:

- [csv](https://raw.githubusercontent.com/keycap-archivist/database/master/db/catalog.csv)
- [json](https://raw.githubusercontent.com/keycap-archivist/database/master/db/catalog.json)

To manipulate some attributes of the catalogs you can add those to the gdoc:

- `(ka_cover)` will make the sculpt of the current cell as the cover of the catalog
- `(ka_self_order)` anywhere in the document, will use the order of the gdoc instead of alphabetical order
- `(XXXX YEAR)` will add the date on the sculpt or the colorway. Free input field. eg: `(March 2019)` or `(2019)`
- `(ka_from_XX)` will add the nationality of the maker. Free input field using 2-digit ISO code for the country. eg: `(ka_from_fr)`
- **Sculpt Header** `(ka_profile_xxx)` Specify the profile of the sculpt. Available values: `blank`/`sculpt`
- **Sculpt Header** `(ka_design_xxx)` Specify how the design was made. Available values: `physical`/`digital`/`hybrid`
- **Sculpt Header** `(ka_cast_xxx)` Specify how the cap is made. Availabe values: `resin`/`mixed`

## Source Catalogs

| Id | Catalog | Url |
| -- | ------- | --- |
| a8d34c5e | 1of1Keycaps | [link](https://docs.google.com/document/d/1p1r9wy1Url3ilU-Tn4ear2gtDtKsIkbG1WlCTTJjOKQ) |
| 7f19c7d | 2Tcraft | [link](https://docs.google.com/document/d/1aWFIxJmIVeJDZH1b_1TEWJBUOcqqsAzUJ6KgEwp069Y) |
| 70a60bc4 | 404Artisans | [link](https://docs.google.com/document/d/1Xjq3VloGrpGE9gmEcbdGhaX_NB0O5eqv7xg_PgVgHX0) |
| fbd9e173 | 8o8keys | [link](https://docs.google.com/document/d/15rWfoHxCHXtWuRjZYYX6u98H9IG0U4AugsCEHDKzLas) |
| ff5fc103 | ACkeys | [link](https://docs.google.com/document/d/1-pP9xJMH55xNGq3waZb6n5x0t6vNX9aqsQAUKaXLfv8) |
| a00953bd | Alpha Keycaps | [link](https://alphakeycaps.com/) |
| 8c954f4 | Amidst The Clouds | [link](https://docs.google.com/document/d/11BeNsND5cMw_NMfGhQfeitg4oFJGNbT4aJ9C_8_iB60) |
| c44d43cd | Anomaly Caps | [link](https://docs.google.com/document/d/1zc0G7J3wd6sdOFcdLokOmom-mQmgm6gzhXUHZO8r3kI) |
| 63243e40 | Archetype | [link](https://docs.google.com/document/d/1A8WdP-pS82xPQuxw98EuOyfmAncqlPLmLtzS2uujfWg) |
| 944a9285 | ARKEYS | [link](https://docs.google.com/document/d/1q__LoSd2vlzY95KKp0TStW2bA3XBPvKZcOQPrKprQh0) |
| 67588eb5 | Artkey | [link](https://docs.google.com/document/d/1piD-uC3eAwy0dkqxnsZoYr_-AnezmelpFnHfuK3RslM) |
| a3bffc04 | Artzeikaps | [link](https://docs.google.com/document/d/11l5gZpMa9dCoSm3RYnhKc0YXSpSm__WIfLyQsg7asto) |
| a738fd7e | AsianJoyCo | [link](https://docs.google.com/document/d/1s02KAr-bTy2ZHR6YU4O2NLqLNxM9cAeJ9HrZ1Q3uWYI) |
| 8cae7fe0 | Ato Works | [link](https://docs.google.com/document/d/1rye8X24IRtPhhXHcuPhisZUs16oKWM7zeqtjBU_SSPg) |
| 3fbc0f79 | Avocaps | [link](https://docs.google.com/document/d/1hOGoAtIWAxII-y3X8cSJ4hKLHOlrdhkc6iObC0DzWt4) |
| 9adb7126 | AX Studio | [link](https://docs.google.com/document/d/10pezHskqq5EVPEKb2fkm2e8gFrch-rWtXB3eQy_KbkI) |
| f8deaa65 | Azi Keycaps | [link](https://docs.google.com/document/d/1ysgu4CCl_hRjyGUqJbgEJrC69MYOcy5Mo0BgR6457fk) |
| a9328677 | B.o.B Handcraft | [link](https://docs.google.com/document/d/1Igk_at2yvP_Bd6GNd3_GLCQmooNszkNDDvm2b6yqIQM) |
| 634ef7c | Backward Caps | [link](https://docs.google.com/document/d/1eHoHMjOIaZv57h3XgOfamgWaE4nfMbFKLj827XNKSac) |
| b6cb880b | Bad and Booj Keys | [link](https://docs.google.com/document/d/15OgzFWmOJWM5h0JBMV85041Vjd88lNXfj6cWkwd-BFM) |
| 32a182c4 | Bad Habit Caps | [link](https://docs.google.com/document/d/1MUoyBLW1slC819V1IdDa2eAV5adU2IHGa5YjmFY5w88) |
| 3a10499 | Bailong | [link](https://docs.google.com/document/d/1f3h3roO2nk229BoeQZxuQVd-HgAJXXqToNSKFVbyIEI) |
| 6b6b943f | Bhomass Caps | [link](https://docs.google.com/document/d/1N8RgbXu7BVt1uXa38uyJMMQJ5FzqxgmvqktNpp9MA_Y) |
| 85b28a01 | Binirias | [link](https://docs.google.com/document/d/11EAZ-nVLgIKuRXEXQDQ1SJotvq871jPLMo9HlS3eAZg) |
| 1c160278 | BKM Caps | [link](https://docs.google.com/document/d/1LinZIytdrqwGE7H3TBWeIrj6ICQ_2DzWVm2Mmk904Y8) |
| 6175f0c7 | Black Mage Caps | [link](https://docs.google.com/document/d/1uIATE-QeIMq_kZnXi_EVfZZoHpM3dmc2woBekYV4L2A) |
| 4fa3abe3 | BladeMX | [link](https://docs.google.com/document/d/1phPDeQ05dFkGzaXeVZzCjv-E8c58xh6skD0cR_koE1k) |
| df1a1521 | Blank Works | [link](https://docs.google.com/document/d/1ehAQBiLvDzM6FUqAKxP2kpJFEQaDnq3yR75TuM0L8vY) |
| ff8ad9cd | Bludgeoned Kaps | [link](https://docs.google.com/document/d/1KKMT4uvPquXcrWF1dX3p3R-PJ_0A98oUO2kwkNvLOd8) |
| d84851f7 | Bogan Caps | [link](https://docs.google.com/document/d/1n0ptNP1tZHnMtpJAI_s_qlnvulYl9SZBJwkCHdU5vHI) |
| 4d74b92e | Bogwitch Brie | [link](https://docs.google.com/document/d/106B5I-IfI1pZex401MHj6c_e7MPUSPyplQsvUOPxmO4) |
| 84748ce6 | BoomSnap Caps | [link](https://docs.google.com/document/d/1Uj-JdFhGKaEhKw7-O3HGzzrNctD1c4a8zwC6lezk9nQ) |
| 3c63e8bf | Booper-Omniclectic | [link](https://docs.google.com/document/d/18QS_4zYR3rFtGLLV1fPZCce5vc6i8_3kauY36xUtTdk) |
| dc6c280a | Bowbie | [link](https://docs.google.com/document/d/1CyKhBbny0xMHcbHtdFQC_P0nrczYOpYdz3KV6ujdPnc) |
| 40217679 | BrewCaps | [link](https://docs.google.com/document/d/1ibnukzm73aRIkBm83OhmPsT6wdyA1GH3MRQ6FPBkOSA) |
| 6b8946c4 | Bro Caps | [link](https://docs.google.com/document/d/1SLiSnTXJXR6X5jT5VnmAe4e3K2yFgZosxBUY1kQQKwo) |
| f4340f3e | Bungkee | [link](https://docs.google.com/document/d/1n1Wcp3UNo6M161050sW-tFL1Wn7tgRYpG3CeKLo1jn4) |
| 384b501d | C.Y.O Keycaps | [link](https://docs.google.com/document/d/1Rhig59IdZh5IZ3JP3R_FjZncRxo2M5tfPiUyxJBuLq8) |
| 4a55e0be | Cantoclicks | [link](https://docs.google.com/document/d/1AOw5Rczpa5NEohg5DQScnqi5Efvc6R8z4F46JIYoOP0) |
| 7893764b | Captomaniacs | [link](https://docs.google.com/document/d/14VMtz60UJoIfm-Lq66lqJjpwwofk4ZlREq4JKSMEFPo) |
| f3c6b75f | Catto Caps | [link](https://docs.google.com/document/d/1Lb8WPFy3mCNnt49yAkhJwqQugKJdo11PBLJfeMfodHI) |
| b2618556 | ChickenCap | [link](https://docs.google.com/document/d/1pkiYq1bxrHYqydM7yj9dKZPG8vC8fNBMGOrQGSyT7qQ) |
| 746e9d1 | Clack Factory | [link](https://docs.google.com/document/d/1C9I7PaXFtpNzI8Zb_6ZTjHLMrQ8ERyWn_IvMD8mVoq0) |
| 155af2e6 | Coconut Keycaps | [link](https://docs.google.com/document/d/1lx648GXchw4ZpctFtirPx_teQcpcgVWuy83W32JY4KU) |
| 84c8facf | CozCaps | [link](https://docs.google.com/document/d/14EBfRe0AxEbCok856_HrL6teQAlkeQL3kpa3z8lenTc) |
| fd91c007 | Craftkey | [link](https://docs.google.com/document/d/1Ruol_1a4kzgLyXkeQ4d7ayu2shpsJPrHVUu7dBIYOYQ) |
| 1be8013f | Crystal Pieces | [link](https://docs.google.com/document/d/1cR7ceg-E5K8D-AxTq4-9Wm3s_qeUTFjTcJIJBWBZnJU) |
| 52730e4a | CYSM | [link](https://docs.google.com/document/d/1c0H4ABr3csHH5B9WP7yyKfCcjLvBE7aJrNwlQzcczcI) |
| ba4abd | Daisy Skull Studio | [link](https://docs.google.com/document/d/12mtyujoMo0dB2iiWR4utBunOAXyIeGEClFuYHEx0Fzg) |
| 120fb8f2 | Dalifu Caps | [link](https://docs.google.com/document/d/1JpL8NeP-J85x_Viy_VGzM5fRpEAMPw_giRO78eHnc4E) |
| bced6bca | DCcaps | [link](https://docs.google.com/document/d/1ENp3M-HymI9LsJRloDGuo3o9s-FXHzFj6hWazGfXSEQ) |
| bf97de89 | DDOR Studio | [link](https://docs.google.com/document/d/1x6w725FhjkOUwu3ZMYMMtDgZg9404CdexIYKgQdBE8Y) |
| df46082a | DeagCaps | [link](https://docs.google.com/document/d/1SsLhATHPRDOSAiywL5ktrGAuZbW9swCOd2cBGuUds3E) |
| 97279208 | Death Dealer | [link](https://docs.google.com/document/d/1ffA0_Y8zC68So3XPeoP41JsAC2M68RSRfNAxzaFdslY) |
| 6ff97cfa | Deathcaps | [link](https://docs.google.com/document/d/1Y1Ip37QbnjNNiOYEAvbv9KVz9A74DFEufDDF22F1OvA) |
| d9ecb1c0 | DELLA KEY | [link](https://docs.google.com/document/d/1beOD7ijqhqVV3FaWnvMF08FQ5KQGO-PENN5hohyrEm4) |
| 3d066446 | Destroyer Caps | [link](https://docs.google.com/document/d/1Me6mlm7YPdH0v5nkCQBZrGJ555gT2RAXwLzC_g4cdIg) |
| 95f25c5d | Dollartacos | [link](https://docs.google.com/document/d/1iAaGXFW6zqBa8lx6sKyQmKTvtiDA1zEiAM4jR4zd-Bs) |
| 2230f9b3 | Doohickeys | [link](https://docs.google.com/document/d/16IlT-1jACqQYUyyEz15-XWG684vyM73z8zM_ABx_UMs) |
| 685c2588 | Dreadkeys | [link](https://docs.google.com/document/d/1tzm7_NLV5XdM2tuM2naiZhDjMMygstN2XneBU_GWbeY) |
| 690a1b90 | DRiiiP Keys | [link](https://docs.google.com/document/d/1hIFJszQMhrQgfo0wjpplbWcvcWIAs5y3HwfwrbFI9e4) |
| 1eb1d13a | DustyCaps | [link](https://docs.google.com/document/d/1EZstC5O7OMdsCMMzs-YbV3Y5pooytHrHpLWaULr3pEI) |
| 3e9cabfa | Dwarf Factory | [link](https://docs.google.com/document/d/13sG3yOqu-7AFkHRcSulp_Iwm0N4g9SOKwSi0vWxx2yA) |
| 54707c4b | EchoppCaps | [link](https://docs.google.com/document/d/1EJ-AUHXajDE3Iih5Af9C3SF8N5guTOeTNC4C0BYlGbM) |
| 68cdf6dc | EzKeys | [link](https://docs.google.com/document/d/1NGfIh3aAU5CwE425oshmoUBEjs11In1j7pVUHrov8Vs) |
| bac9503f | Fraktal Kaps | [link](https://docs.google.com/document/d/13LmVzCkuN7uGhair0QXq1sJkI7LK6jBs-uhnVU-hDII) |
| 6cae29b | FromScratch Caps | [link](https://docs.google.com/document/d/1xeyfq3YJTwOhGnUBFFZLMCj5S9D7gUrd6Umf12GPAzA) |
| 8d20284c | Frumpzkeys | [link](https://docs.google.com/document/d/15arZPVtJHvLxrF20l_Oc-cZCwZrwtMI_SyiD2KDsvWg) |
| 23634907 | Gaia’s Creature | [link](https://docs.google.com/document/d/1EJ8IodjlMPG-TtmKwTZuCvIQYO9uuD_phTnMiNqjh4s) |
| 6829387 | Girlycaps Studios | [link](https://docs.google.com/document/d/1cDD3aNsQXHJfyskP8906BUwfc1_4H_JJTtZ9akhQkOc) |
| 321e47e3 | Glyco Caps | [link](https://docs.google.com/document/d/1SOtOKEBn8oUXnECK0_9-sJ5YBh6BijlbKB6CZsNEBbc) |
| f52fa070 | Goldenstar Keycap | [link](https://docs.google.com/document/d/1rCP_Nn_PQeMiqsFlJ2_8TvFHFPsTpq90-QPgDBo7H40) |
| fb0800a2 | Gooey Keys | [link](https://gooey.link/keycap-archivist.json) |
| 84c0fb40 | Gothcaps | [link](https://docs.google.com/document/d/17YdYcvKifysUDk6mt750Jgq7Zke2kSi66kfqc9BE6RQ) |
| 8a2782a7 | Grimey as Fuck | [link](https://docs.google.com/document/d/1AdPXkALzPErnyMQZrWDJ6o-jCvFB34XeZyz00FDDvLY) |
| cc91fabb | GTB | [link](https://docs.google.com/document/d/1qoQ7zBUrkCvfu-xMHcCvxObflfy8z8fWJnkMBJcdp_w) |
| f74b1fa4 | HDKey | [link](https://docs.google.com/document/d/1eAcxA8lthmxRaPe77X9QpFmThezCcr9BjPpw17aSB6U) |
| 8ffca07f | Hellbent Caps | [link](https://docs.google.com/document/d/15NNk_ttTXCBCHTzyEE3_EigOHPYnc1M5fVGRZJIt0AA) |
| ada5e593 | Hello Caps | [link](https://docs.google.com/document/d/1r_RNJJW5uagd8SL47-c_b_lvb2TuxBsqU6zJhFzs2Vk) |
| c0c9ffa9 | Hot Keys Project | [link](https://docs.google.com/document/d/1KcZjWQ59gmgNoX1piEdf6MX1r6sBig2_G9AYrs1SjBQ) |
| 4183ab23 | Hunger Work Studio | [link](https://docs.google.com/document/d/1UGadEUhjZ-wyVywIb1-Qwpd32jPkobNaYisQTuJG-wQ) |
| 1ff2c383 | Jelly Key | [link](https://docs.google.com/document/d/1Y9hJ5WgjSjXhKEpeLudk542Mj_P0B9aJt56CLdf5Oas) |
| 594d1920 | Jibii | [link](https://docs.google.com/document/d/1KTJ1Up_7Jjr81xbjNSzNswNBXnfSgOsEZr4wc2ODEEo) |
| 79bfad4f | Jusherhoe | [link](https://docs.google.com/document/d/171XoC3BAC13iMQlAJ85impbm-jj7irgCDZwGwYfNTfc) |
| d6c0d49e | Just Another Keymaker | [link](https://docs.google.com/document/d/15c2a6DnBQPJbnVhbjH54KIKVr_I-twb7EQgXB37GAlM) |
| 6513dfae | KapCave | [link](https://kapcave.nachie.com/api/v1/catalog/list) |
| cdd91103 | Kaphaus | [link](https://docs.google.com/document/d/1QXedbahyT1FndM9QdxZ8HC0RshpbyCvChTuQTY688lE) |
| e4eb5c37 | Kapsule Lab | [link](https://docs.google.com/document/d/1aY15g26g_KGpSfBv5XPPeXPFnP9Lq9xgJUlF3IVsm_c) |
| 357a2610 | KB Keycraft | [link](https://docs.google.com/document/d/12mZSYQV5qtEyRFm-ojm3Bu6B1bX-pePAxoyz-5cE-v8) |
| 8cb07a8b | KBK-KWK | [link](https://docs.google.com/document/d/1656SEjL_uolfVYeUgiAjbelyM_HhxAg77oTCPWiviD8) |
| 6efbabef | Key Capital | [link](https://docs.google.com/document/d/11s6cWXG1-_m0x4JpFF0kUD716laUxKUhtIzO0r_OP1U) |
| dc9c4003 | KeyCapCustoms | [link](https://docs.google.com/document/d/1AkBXbURT4fcY65uW0HgU4lHXS0_YqGmdJoXUz8kXWCs) |
| f2a7d69d | Keycat | [link](https://docs.google.com/document/d/1VNVGf02zR9t3QBYXbxV9SqJFuilQBpKxWHTj0iWrX3w) |
| 7b28db24 | KeyCravings | [link](https://docs.google.com/document/d/1QjFV7yp4Ez8k51qPo2fx_2sXVH9l7SdbI3_sy_E7R_o) |
| 1091a0ac | KeyForge | [link](https://docs.google.com/document/d/1d-CVHj9vA0l-qQjYOFws6Wh9YPLSpCfFCwGDsmDLoJA) |
| 5137e37f | KeyKollectiv | [link](https://docs.google.com/document/d/18jTzayNzUDECKOfe-ZXa6oDucNj8_Pp0jEjsdzvvSws) |
| dbf82e90 | KeyLabs Keycaps | [link](https://docs.google.com/document/d/1-VofkRGFmgtlq7R8986aXr8kdMYw9gsT59cjhEgn8D8) |
| 785e721c | Keyzen | [link](https://docs.google.com/document/d/1YljdTx25HavIPtY4ZFNWT1eULVTbCS-i1bUYjEVjwU4) |
| da43467e | Kin Caps | [link](https://docs.google.com/document/d/1oSC6767-PT4EzL_qaj8Q1kFWyl64QqzH40Fgg_jzadw) |
| db87932a | KiyoKaps | [link](https://docs.google.com/document/d/1eC4oLh3QZ-4kUeejnhWTPEnh7_D2pqp7CsQDziXf6uQ) |
| 29a8f167 | Klaykaps | [link](https://docs.google.com/document/d/1U_Te4TY5Nxwme5CjnFMd3tGqSYXJxrkYK7c7VlkI2MU) |
| c14e96a7 | KrakenKap | [link](https://docs.google.com/document/d/1zvIUqPg7D-vge_JzpzqmnD4lEkQgzaQCBFc10FXmasA) |
| 9e85468d | Krap Shop | [link](https://docs.google.com/document/d/1YUGAY-ZxuFC9dCF_fXZ8tVW8T0LSN9FlLjxRTscnoVc) |
| acfac611 | KUG | [link](https://docs.google.com/document/d/1_GW1c005RK7X2olNW2flNdkJEcM9_TOZ1e4ONUfHUYU) |
| 4e1aff89 | LandCaps | [link](https://docs.google.com/document/d/1qDHsR0Y2U0W_pBPgtvB_i_xh09a1VVInbg3rK7al7Ug) |
| ab1d3b22 | Latrialum | [link](https://docs.google.com/document/d/1crfV15xlpsIIfDxo0PGoEE40ZZfMUkl4JOZO_d1sILY) |
| 4e2dec37 | LazyCaps | [link](https://docs.google.com/document/d/1yyLznWKS7QTrOLTTfP9izvDIlEE_q9n0To1Id3N_0FQ) |
| fa0bf049 | Level caps | [link](https://docs.google.com/document/d/1YEx3xAI3r_MIXrrdWzTBdsPC7rdBoxd87TWwxpfsMyE) |
| ddaf1f8c | Lividity | [link](https://docs.google.com/document/d/18mc8abYoFIYDEqpvJzG5qYLXoQBTBUu9DUp7JSmIFxM) |
| 814e90b | Lo-Ki Caps | [link](https://docs.google.com/document/d/1QGRxPMGI-GIN63LCatprE60zDfcVmy67cG53aXLDf8M) |
| d0cb9c83 | Luna Keycaps | [link](https://docs.google.com/document/d/1AV5u4TtQY2iKOisKygGIn7IYFGzcqU9hhjqI76UzkbM) |
| 3b7e4de6 | Mad Labs Keycaps | [link](https://docs.google.com/document/d/176oXSO83YXhYkVDBpoanyiroWaqXq7SmOY8OQfO6bfY) |
| ea0b31fa | Mastonon.kaps | [link](https://docs.google.com/document/d/1XwH1785exI1NCfr3M-ZtkcTxDe4fICVP0Tmbvg00HXQ) |
| b53ce2ec | Matae Keycaps | [link](https://docs.google.com/document/d/1PZ-Rf46GQiDdG3E6R837QEknkapMMbmqPPXnq0l2vbg) |
| f79138dd | MelonKeys | [link](https://docs.google.com/document/d/1ceCQ48nyCfZ2u0jnzgnvVW0nuxd01a0QS48cx_TVh-U) |
| e0a04a0c | meof | [link](https://docs.google.com/document/d/1Gb0HeMF0jE8wfN6sUJEsVRcWjC88VmWJQnABIKEv28o) |
| cef53f28 | MFC | [link](https://docs.google.com/document/d/1Q4JOAQQIY3iat1tBhDXs8aT8hw0JEk92aJlVRxRI3bY) |
| e57c41a | Miniworld | [link](https://docs.google.com/document/d/1K2IP5lV4-6PLuJcFLhpR-gJAqHhxY7baxZSG2DaSPvo) |
| 69a18319 | Miroticaps | [link](https://docs.google.com/document/d/1tu1aiEHLDCMX3E7nv8ikNl60o-xv4fFdar8krU6Cstc) |
| b71e0cd0 | Monstera Keycaps | [link](https://docs.google.com/document/d/1BVfiGhTs-8dCm2u_KpAxKGALy9X7CT94rDljgyFl0uE) |
| 1bbabce6 | MOZIcaps | [link](https://docs.google.com/document/d/1fq6yWk8Gsye4U5M1Fr7SWqTrBMBOx88855RhkUvC10k) |
| fee4aab | MUBAI | [link](https://docs.google.com/document/d/1xWL_Y12WVbijqpWek8dIYPAAoHns6YBb3OPrYBZNryY) |
| 610d23fa | Myth Caps | [link](https://docs.google.com/document/d/1-CkxK7KHUIy9gzJkguA36eC463cBHkNeGfgLa40BKVE) |
| 82ad8553 | Namong | [link](https://docs.google.com/document/d/1vqBrU8VL6Mf6dmRRETjvo5d23HCQuwBQsG1m7w9ClmA) |
| 8b68584c | Navacaps | [link](https://docs.google.com/document/d/1YP-CG6HSuG04dWwG-PUyql0_sBwmae_3q3ukr5N8nJM) |
| b1832521 | NibbNubb Keycaps | [link](https://docs.google.com/document/d/1VDaL0vyFLSMyfmw2k-Aa3RleuEU9o3H6JPiV33zTDy4) |
| 1fac6e72 | Nightcaps | [link](https://docs.google.com/document/d/1GpFn7f6xb2hF0REHKe4ts2wUeHR5CLX8yUMAqSlGW0k) |
| de6ddfab | Nork | [link](https://docs.google.com/document/d/192BiqrPFiOag5NmKTmkAVl9jak0toBjxAOQO8coyO_M) |
| d2df83d9 | Nubbinator | [link](https://docs.google.com/document/d/1sjsPqvqcjt3Wm3MDomwffYVQYjn_g3SDQX-7G1bNN0U) |
| e14f5f5a | Nuhz Caps | [link](https://docs.google.com/document/d/1-BcprHM7kp7znXKbCKrcCnKbd2q5GvX4UI8qod5J3rA) |
| 2f6b5457 | Object.Garage | [link](https://docs.google.com/document/d/1RWKUmcfE9XYslR5GDldajorjTxCqBVM0UE7wBxeB6G4) |
| 8874564c | Obscura | [link](https://docs.google.com/document/d/1nhTGlHevXa6adT_nUrr8aSwt0MevlqlRA3K4_AAr7nE) |
| f086fafc | Ochre + Moss | [link](https://docs.google.com/document/d/1r3HhhDyLTnLJrDb5kpCazx_-j7SwOk9GHl9G-zek-N0) |
| a205ce0a | okeydokey studio | [link](https://docs.google.com/document/d/1_khNYhY3YlyeRK9Tok3qDQ-FJU-lBittK0fsNiLbWhI) |
| efe02066 | Omega Keycaps | [link](https://docs.google.com/document/d/1b9lWjQr0m151takmQQPI7h40cLy_uo6HpDTan418SFE) |
| 500aa195 | Phage Caps | [link](https://docs.google.com/document/d/1m7S6LaNaAg7vfZP9Bt23EYX7v3boC3TpTaqF0gBsEaM) |
| 869ac01f | PhangKey | [link](https://docs.google.com/document/d/1awYbT9shWhsI6wnpXVUozJxwQjFbiYXhTNNPQOCeAvE) |
| afdb1ce2 | Picaps | [link](https://docs.google.com/document/d/1SyKkp4PhrCCealubpwHz5GUWfZejQGspXmgWW2T0qzw) |
| e2792284 | Plastic Drug Dealer | [link](https://docs.google.com/document/d/1dHvxJWBcyuM4mrPUu3Hinqn-Ue1au9INzfljCa_Ue7I) |
| b05d0831 | Polymer Salon | [link](https://docs.google.com/document/d/16FowOOELHP9DmQ7rKdVmgvvEGEgiOhwDtxAA58IDJCg) |
| a73f210e | PrimeCaps | [link](https://docs.google.com/document/d/1EwmD8ej34LImbIWi9hw_5Tsk7GAGZBhoVMJwIFG_Ad8) |
| 8dac3435 | ProjectKey | [link](https://docs.google.com/document/d/1UGwGloN5Cf6w_goJB6FX3FcDiB8EsCjHLLB4r17T3OE) |
| 55851cb5 | Psycho Keycaps | [link](https://docs.google.com/document/d/1V0lB6MTcTkSoClOEakYI57sAI6xOThP9diEwCCQLR1c) |
| 6b46c555 | Q Qaps | [link](https://docs.google.com/document/d/1D1Pt_Jp0Mm35O0a2vFQ6mh2UzcjT1JBWxjqUcc2tSBY) |
| c6e4a02a | RADcaps | [link](https://docs.google.com/document/d/1KINOK9cUUA28pSGnHc8ZI-RM36o12ADojXp7ZeNdTh4) |
| e0a4bf52 | Rathcaps | [link](https://docs.google.com/document/d/1mX-wUILSjmOGULIju5SKD3zKn7VE9hLl2BHgZZPTnG0) |
| d7421e66 | Rejeck Kaps | [link](https://docs.google.com/document/d/10EGmT_ifrjOuqFENtfrxfWljiR8etxHdmyU-gLAhfQw) |
| 2842faca | Resin Party | [link](https://docs.google.com/document/d/172dSOYEqvHX0ihkMkq-iB4fwqKAuKaoSQDDCdLDucVc) |
| 1544e340 | Ritual Master | [link](https://docs.google.com/document/d/1ou0Nk0lPbYXwOHdAOOI9UgbIQHwzd7l3XidY9WK9E7w) |
| 55b03b25 | rtg_caps_ | [link](https://docs.google.com/document/d/1XNeLhAdqfwbgmpm4qbN9nUFQzLktN0JiEJGgRVCEnpk) |
| d1df0782 | Rubrehose | [link](https://docs.google.com/document/d/1dCtWhW9ng-IgVFi-98HyglVmfVLIqiFN6w8u5-0EU4E) |
| 958ea08d | S-Craft Studio | [link](https://docs.google.com/document/d/1zM8PAeSNFJ1Voo4m2Qpcjqtymy_umMBBMVt_USkoYCs) |
| f3efa727 | Sandun | [link](https://docs.google.com/document/d/1xvrzm5YONiCodBoYCWdL3hP1rDPPklq4WXNbsjDT-w4) |
| e035ee16 | shirouu.kaps | [link](https://docs.google.com/document/d/177W_IQZ1HRQbSZ4pjLuWqGlhvS9sTpVZcKV_Ucs-h9M) |
| 61895633 | Simulacra Caps | [link](https://docs.google.com/document/d/1tY7twR6E65afan23BediwbxwvsjJqXtleE949r5mNeg) |
| 980bdc64 | SirReal Caps | [link](https://docs.google.com/document/d/1EllRzUrKjgARXPRYy180K9ru_aYgVG89DQ8CxxFViRc) |
| a31490c1 | Slime Scholar | [link](https://docs.google.com/document/d/14jF0ewtoj5S2GPXkGrfppH3zu0Dd2Y8aZnJ_nP1kPuw) |
| 34fb9c1f | Sludgekidd | [link](https://docs.google.com/document/d/1NDxNP0oKZOGW_13FrXevtgagTYmgHTGn66V7MYf7sx0) |
| 45d1c689 | Smyleey x Godmade | [link](https://docs.google.com/document/d/1pbpzRVKy4kv4yRc5Ztj8M6H-FlHCID4nASttnwn1pYE) |
| 834a1ae7 | SodieCaps | [link](https://docs.google.com/document/d/1R2dHjC3M2dab4_pMVnc-ti11gazoD42Lqknjm5EW2R0) |
| 62a4c768 | Stone Keys | [link](https://docs.google.com/document/d/1kVAbEYLLsFT4y6k0b7A1aenvKOtPzX93cSDXqC_f2eQ) |
| 257e3462 | Sublyme Keys | [link](https://docs.google.com/document/d/1Q6lOKRofrQXEFxQddLXDYC2B_9rZ6pd7qbUfueiranI) |
| 366c9651 | Suited Up Keycaps | [link](https://docs.google.com/document/d/17XHW8yaMXVS5i82lOrjXIF7Q68NwCg6w9B6BiEn7A1k) |
| ede9ca7c | Sway Caps | [link](https://docs.google.com/document/d/1tRhoMKBVZuBxE9UAynqtBNrm__OEjQnOF07NIUamQtE) |
| ff33c7c3 | T-Lab | [link](https://docs.google.com/document/d/1sjUG3_qviJnpMV7w6hAAPKjcLtLVrk-8vrGVXqCptdc) |
| 4e4eda29 | Tech. Stoned. Amish. | [link](https://docs.google.com/document/d/1CzwP-Zj8cLVvMdQRJqDFL_kiZOaOHAcgp3F0owh4-nY) |
| 663df7c5 | theboxkeycap | [link](https://docs.google.com/document/d/1R-0hie5BZ66Uqv-FILFqHEfanQPAYwpBPMGqFWVGR_A) |
| dd852aca | TinyMakesThings | [link](https://docs.google.com/document/d/17Zb-LmujFdcnOZ2_VFhoPHKP1gZJmzEKJH2fawFeqpk) |
| 72ec7d70 | Tokkipee | [link](https://docs.google.com/document/d/1kZoXY-9rV25G5cSwgQxAHwmcjVXNL_LUj8vxhmYYk7k) |
| d518e1b0 | TripleNight.Kaps | [link](https://docs.google.com/document/d/1q_LPkHEAF7Hp-_jBul6foA65RC6LHPKVeN9ExqghsrQ) |
| 985ff9d3 | trmk | [link](https://docs.google.com/document/d/19r0FNbI7cLrjogfDviC7WT2HkuRax9RmPZwn3B_DNOY) |
| a8ab97a4 | Unbranded.caps | [link](https://docs.google.com/document/d/1nQIdjUjkWGyGAIgiEl2oXANX2MJj91uFhCPKOLx2qWw) |
| 2dc47fe3 | Vice Caps | [link](https://docs.google.com/document/d/1WR23MyXbLOAi0Vh6UoeRQqmZ2UsilJNVunw0Y_Hf9fU) |
| de28aff1 | Wildstory Caps | [link](https://docs.google.com/document/d/1745lR0WbiVE9-loe1n4evgd6cPE07yAysP-nZxF2ji0) |
| e2285960 | Win Keys | [link](https://docs.google.com/document/d/1RKX9sVYGkGQKnfGjaLeiFuYwA5zbi5UYfdwSYxHK90w) |
| 15c2097d | YoungsterHarris | [link](https://docs.google.com/document/d/1OB-qI-3izrbmWZG08Qi-ihNaCRRB_qmvivs0KCEWpAk) |
| 3bc74ac3 | Yu.Keys | [link](https://docs.google.com/document/d/1OENdni0rgtO6J2cYKqD1ccrubulXDn-bCHt26TG4nHU) |
| 225e11c2 | ZellKey | [link](https://docs.google.com/document/d/1SS3g7HabIxQhRCb9_dEKRBWkXF24XyeELFtlf09hOdQ) |
| 6848aaa0 | Zero Keycaps | [link](https://docs.google.com/document/d/1pJjELN0W1faMi0kcwyrc9do4XwXorlruZfDVMh9Av3Q) |
| ff972406 | Zorbcaps | [link](https://docs.google.com/document/d/1_wtEVliorr29dTkO7NHHBkM3fu80V_rU6eJKMVwd8qQ) |
| ce8a8e22 | Zy.cap | [link](https://docs.google.com/document/d/1iFu8FhwjqIJSrweEA9ziazm0eD5rz3k3NgMtzIHzNw0) |
