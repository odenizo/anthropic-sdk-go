# Changelog

## 0.2.0-alpha.13 (2025-02-28)

Full Changelog: [v0.2.0-alpha.12...v0.2.0-alpha.13](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.12...v0.2.0-alpha.13)

### Features

* **api:** add support for disabling tool calls ([#133](https://github.com/anthropics/anthropic-sdk-go/issues/133)) ([90f7490](https://github.com/anthropics/anthropic-sdk-go/commit/90f7490774321fdbcadea60c4390244afd5b4c3d))


### Documentation

* update URLs from stainlessapi.com to stainless.com ([#131](https://github.com/anthropics/anthropic-sdk-go/issues/131)) ([334be2b](https://github.com/anthropics/anthropic-sdk-go/commit/334be2b932571846203e0019ee3fe5b551d42c96))

## 0.2.0-alpha.12 (2025-02-27)

Full Changelog: [v0.2.0-alpha.11...v0.2.0-alpha.12](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.11...v0.2.0-alpha.12)

### Features

* **api:** add URL source blocks for images and PDFs ([#129](https://github.com/anthropics/anthropic-sdk-go/issues/129)) ([589f5dc](https://github.com/anthropics/anthropic-sdk-go/commit/589f5dc44bdcfbec7269dcd0ad94baf72c3876b3))


### Bug Fixes

* Preserve Thinking and Signature fields in Message.ToParam() method ([#128](https://github.com/anthropics/anthropic-sdk-go/issues/128)) ([b67c786](https://github.com/anthropics/anthropic-sdk-go/commit/b67c786b64d3a3903a0dcdc50ceac07fc4a6396a))


### Chores

* **internal:** update spec ([#124](https://github.com/anthropics/anthropic-sdk-go/issues/124)) ([3b3bdad](https://github.com/anthropics/anthropic-sdk-go/commit/3b3bdad4b5038278d26ed1c82e0a37259326c049))

## 0.2.0-alpha.11 (2025-02-24)

Full Changelog: [v0.2.0-alpha.10...v0.2.0-alpha.11](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.10...v0.2.0-alpha.11)

### Features

* **api:** add claude-3.7 + support for thinking ([cc7ddcc](https://github.com/anthropics/anthropic-sdk-go/commit/cc7ddcc83a2aeabc17037035b42e94d59679d9e3))
* **client:** send `X-Stainless-Timeout` header ([#114](https://github.com/anthropics/anthropic-sdk-go/issues/114)) ([66f2aec](https://github.com/anthropics/anthropic-sdk-go/commit/66f2aec50b2abf200eaca7fd6636c64059bc884b))
* **pagination:** avoid fetching when has_more: false ([#118](https://github.com/anthropics/anthropic-sdk-go/issues/118)) ([6d90a30](https://github.com/anthropics/anthropic-sdk-go/commit/6d90a300dd0553b92b2f555cc11bc4a134593b90))


### Bug Fixes

* **client:** don't truncate manually specified filenames ([#121](https://github.com/anthropics/anthropic-sdk-go/issues/121)) ([ce64cf5](https://github.com/anthropics/anthropic-sdk-go/commit/ce64cf54d299d5d3d7b707024ea5ca65c4bd5b56))
* do not call path.Base on ContentType ([#120](https://github.com/anthropics/anthropic-sdk-go/issues/120)) ([5f20f48](https://github.com/anthropics/anthropic-sdk-go/commit/5f20f48a882546e5e25492a543a7cc56be3eb7dc))
* fix early cancel when RequestTimeout is provided for streaming requests ([#119](https://github.com/anthropics/anthropic-sdk-go/issues/119)) ([20af10e](https://github.com/anthropics/anthropic-sdk-go/commit/20af10e556caa9dd1691fee0c68aab528d61bc87))
* fix unicode encoding for json ([#111](https://github.com/anthropics/anthropic-sdk-go/issues/111)) ([699e5cd](https://github.com/anthropics/anthropic-sdk-go/commit/699e5cd7a37a20b48824d0b1b978b28df1d8afbf))
* **stream:** ensure .Close() doesn't panic ([#113](https://github.com/anthropics/anthropic-sdk-go/issues/113)) ([2125563](https://github.com/anthropics/anthropic-sdk-go/commit/2125563ac0bf773e0795ce51933e535854a30a0e))
* update stream error handling ([#117](https://github.com/anthropics/anthropic-sdk-go/issues/117)) ([40d1ea2](https://github.com/anthropics/anthropic-sdk-go/commit/40d1ea2589b3df6111c8cf000f49ec46ede7a7a4))


### Chores

* add UnionUnmarshaler for responses that are interfaces ([#116](https://github.com/anthropics/anthropic-sdk-go/issues/116)) ([93f533c](https://github.com/anthropics/anthropic-sdk-go/commit/93f533c1c940b1dd6264886344902239a268634a))
* **api:** update openapi spec url ([#108](https://github.com/anthropics/anthropic-sdk-go/issues/108)) ([8f291ed](https://github.com/anthropics/anthropic-sdk-go/commit/8f291ed434cd1cd0eb7f82a2e8b39b9e97744f6e))
* **docs:** add docstring explaining streaming pattern ([#115](https://github.com/anthropics/anthropic-sdk-go/issues/115)) ([862c3d4](https://github.com/anthropics/anthropic-sdk-go/commit/862c3d41e8d19ad4b0e9d2d228719c930e6f7d18))
* **internal:** fix devcontainers setup ([#123](https://github.com/anthropics/anthropic-sdk-go/issues/123)) ([6f9dcc1](https://github.com/anthropics/anthropic-sdk-go/commit/6f9dcc103ee4dfeeda6a5c78e3d461d0c3ddab0b))


### Documentation

* document raw responses ([#112](https://github.com/anthropics/anthropic-sdk-go/issues/112)) ([1cf3aee](https://github.com/anthropics/anthropic-sdk-go/commit/1cf3aee0a28edc06e0e19723f94290b80074d6ce))

## 0.2.0-alpha.10 (2025-01-28)

Full Changelog: [v0.2.0-alpha.9...v0.2.0-alpha.10](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.9...v0.2.0-alpha.10)

### Bug Fixes

* fix interface implementation stub names for unions ([#106](https://github.com/anthropics/anthropic-sdk-go/issues/106)) ([0ac5655](https://github.com/anthropics/anthropic-sdk-go/commit/0ac5655d4033ec3d6448ecf89216b048bccbbd85))


### Chores

* **api:** deprecate some models ([#105](https://github.com/anthropics/anthropic-sdk-go/issues/105)) ([f1e30cc](https://github.com/anthropics/anthropic-sdk-go/commit/f1e30ccd3ace4165bf0653cf5251b1fc06a1e78a))
* **docs:** updates ([#103](https://github.com/anthropics/anthropic-sdk-go/issues/103)) ([c264f59](https://github.com/anthropics/anthropic-sdk-go/commit/c264f59fc3f58a0233f8c801436cccc0f4eeef6c))
* refactor client tests ([#107](https://github.com/anthropics/anthropic-sdk-go/issues/107)) ([f02b038](https://github.com/anthropics/anthropic-sdk-go/commit/f02b038063ab0095cc3497cbe1c3f585cb471817))

## 0.2.0-alpha.9 (2025-01-23)

Full Changelog: [v0.2.0-alpha.8...v0.2.0-alpha.9](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.8...v0.2.0-alpha.9)

### Features

* **api:** add citations ([#101](https://github.com/anthropics/anthropic-sdk-go/issues/101)) ([59fd065](https://github.com/anthropics/anthropic-sdk-go/commit/59fd065fe106db20527f37e4ecdc6cc771c10418))
* **api:** add message batch delete endpoint ([#81](https://github.com/anthropics/anthropic-sdk-go/issues/81)) ([b3a63e7](https://github.com/anthropics/anthropic-sdk-go/commit/b3a63e7cbf73d06141750cf126af25412b12061d))
* **client:** support results endpoint ([#98](https://github.com/anthropics/anthropic-sdk-go/issues/98)) ([380054f](https://github.com/anthropics/anthropic-sdk-go/commit/380054fc5608380cdc054a181d83558ee7c5b946))


### Bug Fixes

* fix apijson.Port for embedded structs ([#95](https://github.com/anthropics/anthropic-sdk-go/issues/95)) ([5c3a7f7](https://github.com/anthropics/anthropic-sdk-go/commit/5c3a7f7f4d2694b8b52a0c4a36701a489a58dcf0))
* fix apijson.Port for embedded structs ([#97](https://github.com/anthropics/anthropic-sdk-go/issues/97)) ([55a3365](https://github.com/anthropics/anthropic-sdk-go/commit/55a3365c873b6b385d27f2315e370fa40736778e))
* fix header parameter value ([#90](https://github.com/anthropics/anthropic-sdk-go/issues/90)) ([d52699a](https://github.com/anthropics/anthropic-sdk-go/commit/d52699aa2036162f6842a3115eb754b6870260e1))
* prevent niche naming conflicts for string enums with different casing ([#100](https://github.com/anthropics/anthropic-sdk-go/issues/100)) ([3af5fe8](https://github.com/anthropics/anthropic-sdk-go/commit/3af5fe8993928a6985022cdbea6bfe220a6d6be5))
* support array query parameters ([#89](https://github.com/anthropics/anthropic-sdk-go/issues/89)) ([d728bcc](https://github.com/anthropics/anthropic-sdk-go/commit/d728bcc9d69414bb3ba577e504e1285f0eb22bc5))


### Chores

* bump license year ([#88](https://github.com/anthropics/anthropic-sdk-go/issues/88)) ([c8ddc6b](https://github.com/anthropics/anthropic-sdk-go/commit/c8ddc6b1364485e299e050423e459023e2d65b46))
* **internal:** remove unused field ([#94](https://github.com/anthropics/anthropic-sdk-go/issues/94)) ([b98d12a](https://github.com/anthropics/anthropic-sdk-go/commit/b98d12a3991ae2f1d714833a71ec90dedc552661))
* **internal:** rename `streaming.go` ([#96](https://github.com/anthropics/anthropic-sdk-go/issues/96)) ([ce8ac0f](https://github.com/anthropics/anthropic-sdk-go/commit/ce8ac0fe762132d230241f021eeb0cd4215f271b))
* **internal:** update examples ([#91](https://github.com/anthropics/anthropic-sdk-go/issues/91)) ([9717662](https://github.com/anthropics/anthropic-sdk-go/commit/97176628489158be07baf1747ba39f15429d3a39))


### Documentation

* **readme:** fix misplaced period ([#93](https://github.com/anthropics/anthropic-sdk-go/issues/93)) ([953d510](https://github.com/anthropics/anthropic-sdk-go/commit/953d5104b1460b749b776a6ba4df90d2604c06cd))

## 0.2.0-alpha.8 (2024-12-19)

Full Changelog: [v0.2.0-alpha.7...v0.2.0-alpha.8](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.7...v0.2.0-alpha.8)

### Bug Fixes

* **bedrock:** handle exceptions messages in bedrock stream ([7786f8f](https://github.com/anthropics/anthropic-sdk-go/commit/7786f8f7f97d073b79f5e1faaec1a6de285001c2))


### Chores

* bump testing data uri ([#79](https://github.com/anthropics/anthropic-sdk-go/issues/79)) ([0dc9c88](https://github.com/anthropics/anthropic-sdk-go/commit/0dc9c8811f211cdd25eb5451aa88f258591fb9bd))

## 0.2.0-alpha.7 (2024-12-17)

Full Changelog: [v0.2.0-alpha.6...v0.2.0-alpha.7](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.6...v0.2.0-alpha.7)

### Bug Fixes

* **vertex:** remove `anthropic_version` deletion for token counting ([15987ac](https://github.com/anthropics/anthropic-sdk-go/commit/15987ac82378e0e0d28878f91e2ddca8f6fb5ab9))

## 0.2.0-alpha.6 (2024-12-17)

Full Changelog: [v0.2.0-alpha.5...v0.2.0-alpha.6](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.5...v0.2.0-alpha.6)

### Features

* **api:** general availability updates ([#74](https://github.com/anthropics/anthropic-sdk-go/issues/74)) ([0c19b86](https://github.com/anthropics/anthropic-sdk-go/commit/0c19b86f4d0f8496d551f3b707bfb8834b98b315))
* **vertex:** add support for token counting ([86e085b](https://github.com/anthropics/anthropic-sdk-go/commit/86e085b0452926491ec11b2c77abec4c0a733d3b))


### Bug Fixes

* **messages:** correct batch params type ([2a39e4b](https://github.com/anthropics/anthropic-sdk-go/commit/2a39e4b9af65f0318374f88c2aef150b69df7107))
* replace `MessageParamContentUnion` with `ContentBlockParamUnion` to fix go script ([#70](https://github.com/anthropics/anthropic-sdk-go/issues/70)) ([5d32a5f](https://github.com/anthropics/anthropic-sdk-go/commit/5d32a5f2be05c31932451d8033e954cd71c9fbc8))
* **tests:** correct input schema type ([6514952](https://github.com/anthropics/anthropic-sdk-go/commit/6514952ac492f3f7ceed1c5726dfbc7b5b3f72db))


### Chores

* **api:** update spec version ([#72](https://github.com/anthropics/anthropic-sdk-go/issues/72)) ([854416b](https://github.com/anthropics/anthropic-sdk-go/commit/854416b61b37fff95bca34d7c91035fb11aef921))
* **internal:** update spec ([#73](https://github.com/anthropics/anthropic-sdk-go/issues/73)) ([6da0443](https://github.com/anthropics/anthropic-sdk-go/commit/6da04433a0cdf00600080f45d41cfd92064e7471))


### Documentation

* **examples:** use claude 3 sonnet more ([c02fdac](https://github.com/anthropics/anthropic-sdk-go/commit/c02fdac54687c966a8641be10035c0f389bddfe0))

## 0.2.0-alpha.5 (2024-12-01)

Full Changelog: [v0.2.0-alpha.4...v0.2.0-alpha.5](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.4...v0.2.0-alpha.5)

### Bug Fixes

* **api:** escape key values when encoding maps ([#56](https://github.com/anthropics/anthropic-sdk-go/issues/56)) ([fa49eb8](https://github.com/anthropics/anthropic-sdk-go/commit/fa49eb8c4f8d6fa7e45ec4e7eb457a87218349c4))
* **client:** no panic on missing BaseURL ([#61](https://github.com/anthropics/anthropic-sdk-go/issues/61)) ([7438b15](https://github.com/anthropics/anthropic-sdk-go/commit/7438b15855bd6b5902d62fdbf02f143544eee986))
* correct required fields for flattened unions ([#59](https://github.com/anthropics/anthropic-sdk-go/issues/59)) ([735c07c](https://github.com/anthropics/anthropic-sdk-go/commit/735c07c66a3bbf54bff97db7fe5290d7635c0774))
* forward error and close for bedrock decoder ([#66](https://github.com/anthropics/anthropic-sdk-go/issues/66)) ([5f6f6fd](https://github.com/anthropics/anthropic-sdk-go/commit/5f6f6fd822b029dffd90aa49b06add0661251de0))
* **types:** remove anthropic-instant-1.2 model ([#57](https://github.com/anthropics/anthropic-sdk-go/issues/57)) ([23fbc37](https://github.com/anthropics/anthropic-sdk-go/commit/23fbc3752122462a1e29e15327b1736072032ba3))


### Chores

* **api:** update spec version ([#62](https://github.com/anthropics/anthropic-sdk-go/issues/62)) ([1526051](https://github.com/anthropics/anthropic-sdk-go/commit/1526051561d4e1fe7792d90f0c2299036fedbc21))
* **ci:** remove unneeded workflow ([#55](https://github.com/anthropics/anthropic-sdk-go/issues/55)) ([0181fc2](https://github.com/anthropics/anthropic-sdk-go/commit/0181fc2796bc5fea1a21e2744257900caef8ee72))
* fix references to content block param types ([dea6478](https://github.com/anthropics/anthropic-sdk-go/commit/dea647890542036c1ed4cc55409002fd2e00adb6))
* **tests:** limit array example length ([#64](https://github.com/anthropics/anthropic-sdk-go/issues/64)) ([9fb231b](https://github.com/anthropics/anthropic-sdk-go/commit/9fb231b806af753b6c9aae82c023e087c2ecaefb))


### Documentation

* add missing docs for some enums ([#54](https://github.com/anthropics/anthropic-sdk-go/issues/54)) ([56db6b8](https://github.com/anthropics/anthropic-sdk-go/commit/56db6b832d0e0454895b6d4ab43d32bd6b7418b4))


### Refactors

* sort fields for squashed union structs ([#51](https://github.com/anthropics/anthropic-sdk-go/issues/51)) ([a9874d1](https://github.com/anthropics/anthropic-sdk-go/commit/a9874d193998572a28475781dd8de296d4021bf2))

## 0.2.0-alpha.4 (2024-11-04)

Full Changelog: [v0.2.0-alpha.3...v0.2.0-alpha.4](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.3...v0.2.0-alpha.4)

### Features

* **api:** add message token counting & PDFs support ([#45](https://github.com/anthropics/anthropic-sdk-go/issues/45)) ([775de6d](https://github.com/anthropics/anthropic-sdk-go/commit/775de6d75c61cd3a6b3d63fdf129b1564b1f147c))
* **api:** add new haiku model ([#48](https://github.com/anthropics/anthropic-sdk-go/issues/48)) ([8cb9d59](https://github.com/anthropics/anthropic-sdk-go/commit/8cb9d59b13d12a70866a579dca8cc965e33eeba5))


### Bug Fixes

* **types:** add missing token-counting-2024-11-01 ([#47](https://github.com/anthropics/anthropic-sdk-go/issues/47)) ([bc46a6e](https://github.com/anthropics/anthropic-sdk-go/commit/bc46a6e648f9ad804b119eff977e050843efb7f6))
* **types:** correct claude-3-5-haiku-20241022 name ([#50](https://github.com/anthropics/anthropic-sdk-go/issues/50)) ([f0016bb](https://github.com/anthropics/anthropic-sdk-go/commit/f0016bbb272fd65fcc42f0b664e3ab45a665e673))


### Chores

* **internal:** update spec version ([#40](https://github.com/anthropics/anthropic-sdk-go/issues/40)) ([b41d55f](https://github.com/anthropics/anthropic-sdk-go/commit/b41d55f13b57553bd6e639ae359c5c6f0a9031bb))

## 0.2.0-alpha.3 (2024-10-22)

Full Changelog: [v0.2.0-alpha.2...v0.2.0-alpha.3](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.2...v0.2.0-alpha.3)

### Features

* **api:** add new model and `computer-use-2024-10-22` beta ([#37](https://github.com/anthropics/anthropic-sdk-go/issues/37)) ([a520abe](https://github.com/anthropics/anthropic-sdk-go/commit/a520abeedd326cea2161166cd2259345c15a82e4))


### Chores

* **api:** add title ([#34](https://github.com/anthropics/anthropic-sdk-go/issues/34)) ([2b96326](https://github.com/anthropics/anthropic-sdk-go/commit/2b96326e58bb7179d21476f9ce1a550664f13a38))
* **internal:** update spec ([#36](https://github.com/anthropics/anthropic-sdk-go/issues/36)) ([a735bf7](https://github.com/anthropics/anthropic-sdk-go/commit/a735bf7e7872c8cc3ee08e57167860270e6cdba6))

## 0.2.0-alpha.2 (2024-10-17)

Full Changelog: [v0.2.0-alpha.1...v0.2.0-alpha.2](https://github.com/anthropics/anthropic-sdk-go/compare/v0.2.0-alpha.1...v0.2.0-alpha.2)

### Features

* move pagination package from internal to packages ([#33](https://github.com/anthropics/anthropic-sdk-go/issues/33)) ([ee3edb1](https://github.com/anthropics/anthropic-sdk-go/commit/ee3edb16dcd406435ade212cb7553f75b161e297))


### Bug Fixes

* **beta:** merge betas param with the default value ([#32](https://github.com/anthropics/anthropic-sdk-go/issues/32)) ([9191ae0](https://github.com/anthropics/anthropic-sdk-go/commit/9191ae0b8a47c3c6ea9dfbb5073f1e66f5b4e1d8))


### Chores

* fix GetNextPage docstring ([#29](https://github.com/anthropics/anthropic-sdk-go/issues/29)) ([acf8009](https://github.com/anthropics/anthropic-sdk-go/commit/acf8009c886ec27cc07665b0377a2a3b3493c336))
* **internal:** update spec URL ([#31](https://github.com/anthropics/anthropic-sdk-go/issues/31)) ([240f1c3](https://github.com/anthropics/anthropic-sdk-go/commit/240f1c3d7e4dc145988d2f8d11e45ccfd255861e))

## 0.2.0-alpha.1 (2024-10-08)

Full Changelog: [v0.1.0-alpha.2...v0.2.0-alpha.1](https://github.com/anthropics/anthropic-sdk-go/compare/v0.1.0-alpha.2...v0.2.0-alpha.1)

### Features

* **api:** add message batches api ([#28](https://github.com/anthropics/anthropic-sdk-go/issues/28)) ([169eb3c](https://github.com/anthropics/anthropic-sdk-go/commit/169eb3c83d39126b4f9ec3a8d7f70c06466d9ef6))


### Bug Fixes

* **beta:** pass beta header by default ([#27](https://github.com/anthropics/anthropic-sdk-go/issues/27)) ([c79ba68](https://github.com/anthropics/anthropic-sdk-go/commit/c79ba6826c452ca1eeefd34db1638722fa942082))


### Refactors

* **types:** improve metadata type names ([#26](https://github.com/anthropics/anthropic-sdk-go/issues/26)) ([95f0266](https://github.com/anthropics/anthropic-sdk-go/commit/95f0266f62ba90590db68f1f98e41d80ea8f5388))
* **types:** improve tool type names ([#23](https://github.com/anthropics/anthropic-sdk-go/issues/23)) ([79e4d75](https://github.com/anthropics/anthropic-sdk-go/commit/79e4d75d26bbf2339841d27696477817c01a55fc))

## 0.1.0-alpha.2 (2024-10-04)

Full Changelog: [v0.1.0-alpha.1...v0.1.0-alpha.2](https://github.com/anthropics/anthropic-sdk-go/compare/v0.1.0-alpha.1...v0.1.0-alpha.2)

### Features

* **api:** support disabling parallel tool use ([#22](https://github.com/anthropics/anthropic-sdk-go/issues/22)) ([1d8c00b](https://github.com/anthropics/anthropic-sdk-go/commit/1d8c00b317536d77a26f74d0008e1a4760b17d2e))
* **client:** send retry count header ([#19](https://github.com/anthropics/anthropic-sdk-go/issues/19)) ([d1c8ea1](https://github.com/anthropics/anthropic-sdk-go/commit/d1c8ea1f84d05002705ac7aa4d47a5ba13c388e9))
* improve error message ([#15](https://github.com/anthropics/anthropic-sdk-go/issues/15)) ([98d1ffd](https://github.com/anthropics/anthropic-sdk-go/commit/98d1ffd29f97e85ea543f36ce104c341e729a7d2))


### Bug Fixes

* **requestconfig:** copy over more fields when cloning ([#17](https://github.com/anthropics/anthropic-sdk-go/issues/17)) ([d5e7415](https://github.com/anthropics/anthropic-sdk-go/commit/d5e741578ac0ff88db3b04564810321b18f4dd40))


### Chores

* **ci:** add CODEOWNERS file ([#12](https://github.com/anthropics/anthropic-sdk-go/issues/12)) ([71c33b8](https://github.com/anthropics/anthropic-sdk-go/commit/71c33b841dece97e77f04ea4feae3d586b59b0d6))


### Documentation

* improve and reference contributing documentation ([#21](https://github.com/anthropics/anthropic-sdk-go/issues/21)) ([7288df1](https://github.com/anthropics/anthropic-sdk-go/commit/7288df1e1e62401487bee0685f77119bae5287ee))
* update CONTRIBUTING.md ([#18](https://github.com/anthropics/anthropic-sdk-go/issues/18)) ([dcfcbf8](https://github.com/anthropics/anthropic-sdk-go/commit/dcfcbf8d07e3d7a7d6b6398d60724f38eca050a4))

## 0.1.0-alpha.1 (2024-08-14)

Full Changelog: [v0.0.1-alpha.0...v0.1.0-alpha.1](https://github.com/anthropics/anthropic-sdk-go/compare/v0.0.1-alpha.0...v0.1.0-alpha.1)

### Features

* **api:** add prompt caching beta ([#11](https://github.com/anthropics/anthropic-sdk-go/issues/11)) ([78f8c72](https://github.com/anthropics/anthropic-sdk-go/commit/78f8c7266dd98ef5f76d258f485ee284b7a0e590))
* publish ([5ff0ff8](https://github.com/anthropics/anthropic-sdk-go/commit/5ff0ff8cc5706c39a6dde75ae69d11c892ef8bb3))
* simplify system prompt ([#3](https://github.com/anthropics/anthropic-sdk-go/issues/3)) ([cd3fcef](https://github.com/anthropics/anthropic-sdk-go/commit/cd3fcefad20baef3c28375adf16ab266f97e7d94))
* simplify system prompt ([#4](https://github.com/anthropics/anthropic-sdk-go/issues/4)) ([85e1b34](https://github.com/anthropics/anthropic-sdk-go/commit/85e1b349619e7dd26c06ed0d9f566ddbbe80db2a))


### Bug Fixes

* deserialization of struct unions that implement json.Unmarshaler ([#6](https://github.com/anthropics/anthropic-sdk-go/issues/6)) ([a883a3a](https://github.com/anthropics/anthropic-sdk-go/commit/a883a3a8232dfca1ce8a139047a0356a3fd6015f))
* handle nil pagination responses when HTTP status is 200 ([#2](https://github.com/anthropics/anthropic-sdk-go/issues/2)) ([2bb2325](https://github.com/anthropics/anthropic-sdk-go/commit/2bb232557a9f75d58b7e7145c69771c927574dd3))
* message accumulation with union content block ([09457cb](https://github.com/anthropics/anthropic-sdk-go/commit/09457cb2ef8019cc23bcdefa0d3102e642d64b3d))


### Chores

* add back custom code ([106c404](https://github.com/anthropics/anthropic-sdk-go/commit/106c40466382daaa403e7f472647248e14d939d7))
* bump Go to v1.21 ([#7](https://github.com/anthropics/anthropic-sdk-go/issues/7)) ([928ed50](https://github.com/anthropics/anthropic-sdk-go/commit/928ed50c83154eb4f56575cf9f405a132000888e))
* **ci:** bump prism mock server version ([#5](https://github.com/anthropics/anthropic-sdk-go/issues/5)) ([0b326c6](https://github.com/anthropics/anthropic-sdk-go/commit/0b326c6b18effa222b8b03a17c1e562d0aedce1d))
* **examples:** minor formatting changes ([#8](https://github.com/anthropics/anthropic-sdk-go/issues/8)) ([4195c55](https://github.com/anthropics/anthropic-sdk-go/commit/4195c5541a1a517a3890bfe43eb84e3ddc496bfe))


### Documentation

* add examples to README ([df47298](https://github.com/anthropics/anthropic-sdk-go/commit/df4729897b782faeaa6a0795359ecf20b4a833ca))
