# Changelog

## [0.53.0](https://github.com/aquasecurity/trivy/compare/v0.52.0...v0.53.0) (2024-06-07)


### Features

* **dart:** use first version of constraint for dependencies using SDK version ([#6239](https://github.com/aquasecurity/trivy/issues/6239)) ([042d6b0](https://github.com/aquasecurity/trivy/commit/042d6b08c283105c258a3dda98983b345a5305c3))
* **misconf:** add metadata to Cloud schema ([#6831](https://github.com/aquasecurity/trivy/issues/6831)) ([02d5404](https://github.com/aquasecurity/trivy/commit/02d540478d495416b50d7e8b187ff9f5bba41f45))
* **plugin:** add support for nested archives ([#6845](https://github.com/aquasecurity/trivy/issues/6845)) ([622c67b](https://github.com/aquasecurity/trivy/commit/622c67b7647f94d0a0ca3acf711d8f847cdd8d98))


### Bug Fixes

* **misconf:** fix caching of modules in subdirectories ([#6814](https://github.com/aquasecurity/trivy/issues/6814)) ([0bcfedb](https://github.com/aquasecurity/trivy/commit/0bcfedbcaa9bbe30ee5ecade5b98e9ce3cc54c9b))
* **misconf:** parsing numbers without fraction as int ([#6834](https://github.com/aquasecurity/trivy/issues/6834)) ([8141a13](https://github.com/aquasecurity/trivy/commit/8141a137ba50b553a9da877d95c7ccb491d041c6))
* **nodejs:** fix infinity loops for `pnpm` with cyclic imports ([#6857](https://github.com/aquasecurity/trivy/issues/6857)) ([7d083bc](https://github.com/aquasecurity/trivy/commit/7d083bc890eccc3bf32765c6d7e922cab2e2ef94))
* **python:** compare pkg names from `poetry.lock` and `pyproject.toml` in lowercase ([#6852](https://github.com/aquasecurity/trivy/issues/6852)) ([faa9d92](https://github.com/aquasecurity/trivy/commit/faa9d92cfeb8d924deda2dac583b6c97099c08d9))
* **sbom:** don't overwrite `srcEpoch` when decoding SBOM files ([#6866](https://github.com/aquasecurity/trivy/issues/6866)) ([04af59c](https://github.com/aquasecurity/trivy/commit/04af59c2906bcfc7f7970b4e8f45a90f04313170))
* **secret:** `Asymmetric Private Key` shouldn't start with space ([#6867](https://github.com/aquasecurity/trivy/issues/6867)) ([bb26445](https://github.com/aquasecurity/trivy/commit/bb26445e3df198df77930329f532ac5ab7a67af2))

## [0.52.0](https://github.com/aquasecurity/trivy/compare/v0.51.1...v0.52.0) (2024-06-03)


### Features

* Add Julia language analyzer support ([#5635](https://github.com/aquasecurity/trivy/issues/5635)) ([fecafb1](https://github.com/aquasecurity/trivy/commit/fecafb1fc5bb129c7485342a0775f0dd8bedd28e))
* add support for plugin index ([#6674](https://github.com/aquasecurity/trivy/issues/6674)) ([26faf8f](https://github.com/aquasecurity/trivy/commit/26faf8f3f04b1c5f9f81c03ffc6b2008732207e2))
* **misconf:** Add support for deprecating a check ([#6664](https://github.com/aquasecurity/trivy/issues/6664)) ([88702cf](https://github.com/aquasecurity/trivy/commit/88702cfd5918b093defc5b5580f7cbf16f5f2417))
* **misconf:** add Terraform 'removed' block to schema ([#6640](https://github.com/aquasecurity/trivy/issues/6640)) ([b7a0a13](https://github.com/aquasecurity/trivy/commit/b7a0a131a03ed49c08d3b0d481bc9284934fd6e1))
* **misconf:** register builtin Rego funcs from trivy-checks ([#6616](https://github.com/aquasecurity/trivy/issues/6616)) ([7c22ee3](https://github.com/aquasecurity/trivy/commit/7c22ee3df5ee51beb90e44428a99541b3d19ab98))
* **misconf:** resolve tf module from OpenTofu compatible registry ([#6743](https://github.com/aquasecurity/trivy/issues/6743)) ([ac74520](https://github.com/aquasecurity/trivy/commit/ac7452009bf7ca0fa8ee1de8807c792eabad405a))
* **misconf:** support for VPC resources for inbound/outbound rules ([#6779](https://github.com/aquasecurity/trivy/issues/6779)) ([349caf9](https://github.com/aquasecurity/trivy/commit/349caf96bc3dd81551d488044f1adfdb947f39fb))
* **misconf:** support symlinks inside of Helm archives ([#6621](https://github.com/aquasecurity/trivy/issues/6621)) ([4eae37c](https://github.com/aquasecurity/trivy/commit/4eae37c52b035b3576361c12f70d3d9517d0a73c))
* **nodejs:** add v9 pnpm lock file support ([#6617](https://github.com/aquasecurity/trivy/issues/6617)) ([1e08648](https://github.com/aquasecurity/trivy/commit/1e0864842e32a709941d4b4e8f521602bcee684d))
* **plugin:** specify plugin version ([#6683](https://github.com/aquasecurity/trivy/issues/6683)) ([d6dc567](https://github.com/aquasecurity/trivy/commit/d6dc56732babbc9d7f788c280a768d8648aa093d))
* **python:** add license support for `requirement.txt` files ([#6782](https://github.com/aquasecurity/trivy/issues/6782)) ([29615be](https://github.com/aquasecurity/trivy/commit/29615be85e8bfeaf5a0cd51829b1898c55fa4274))
* **python:** add line number support for `requirement.txt` files ([#6729](https://github.com/aquasecurity/trivy/issues/6729)) ([2bc54ad](https://github.com/aquasecurity/trivy/commit/2bc54ad2752aba5de4380cb92c13b09c0abefd73))
* **report:** Include licenses and secrets filtered by rego to ModifiedFindings ([#6483](https://github.com/aquasecurity/trivy/issues/6483)) ([fa3cf99](https://github.com/aquasecurity/trivy/commit/fa3cf993eace4be793f85907b42365269c597b91))
* **vex:** improve relationship support in CSAF VEX ([#6735](https://github.com/aquasecurity/trivy/issues/6735)) ([a447f6b](https://github.com/aquasecurity/trivy/commit/a447f6ba94b6f8b14177dc5e4369a788e2020d90))
* **vex:** support non-root components for products in OpenVEX ([#6728](https://github.com/aquasecurity/trivy/issues/6728)) ([9515695](https://github.com/aquasecurity/trivy/commit/9515695d45e9b5c20890e27e21e3ab45bfd4ce5f))


### Bug Fixes

* clean up golangci lint configuration ([#6797](https://github.com/aquasecurity/trivy/issues/6797)) ([62de6f3](https://github.com/aquasecurity/trivy/commit/62de6f3feba6e4c56ad3922441d5b0f150c3d6b7))
* **cli:** always output fatal errors to stderr ([#6827](https://github.com/aquasecurity/trivy/issues/6827)) ([c2b9132](https://github.com/aquasecurity/trivy/commit/c2b9132a7e933a68df4cc0eb86aab23719ded1b5))
* close APKINDEX archive file ([#6672](https://github.com/aquasecurity/trivy/issues/6672)) ([5caf437](https://github.com/aquasecurity/trivy/commit/5caf4377f3a7fcb1f6e1a84c67136ae62d100be3))
* close settings.xml ([#6768](https://github.com/aquasecurity/trivy/issues/6768)) ([9c3e895](https://github.com/aquasecurity/trivy/commit/9c3e895fcb0852c00ac03ed21338768f76b5273b))
* close testfile ([#6830](https://github.com/aquasecurity/trivy/issues/6830)) ([aa0c413](https://github.com/aquasecurity/trivy/commit/aa0c413814e8915b38d2285c6a8ba5bc3f0705b4))
* **conda:** add support `pip` deps for `environment.yml` files ([#6675](https://github.com/aquasecurity/trivy/issues/6675)) ([150a773](https://github.com/aquasecurity/trivy/commit/150a77313e980cd63797a89a03afcbc97b285f38))
* **go:** add only non-empty root modules for `gobinaries` ([#6710](https://github.com/aquasecurity/trivy/issues/6710)) ([c96f2a5](https://github.com/aquasecurity/trivy/commit/c96f2a5b3de820da37e14594dd537c3b0949ae9c))
* **go:** include only `.version`|`.ver` (no prefixes) ldflags for `gobinaries` ([#6705](https://github.com/aquasecurity/trivy/issues/6705)) ([afb4f9d](https://github.com/aquasecurity/trivy/commit/afb4f9dc4730671ba004e1734fa66422c4c86dad))
* Golang version parsing from binaries w/GOEXPERIMENT ([#6696](https://github.com/aquasecurity/trivy/issues/6696)) ([696f2ae](https://github.com/aquasecurity/trivy/commit/696f2ae0ecdd4f90303f41249924a09ace70dd78))
* include packages unless it is not needed ([#6765](https://github.com/aquasecurity/trivy/issues/6765)) ([56dbe1f](https://github.com/aquasecurity/trivy/commit/56dbe1f6768fe67fbc1153b74fde0f83eaa1b281))
* **misconf:** don't shift ignore rule related to code ([#6708](https://github.com/aquasecurity/trivy/issues/6708)) ([39a746c](https://github.com/aquasecurity/trivy/commit/39a746c77837f873e87b81be40676818030f44c5))
* **misconf:** skip Rego errors with a nil location ([#6638](https://github.com/aquasecurity/trivy/issues/6638)) ([a2c522d](https://github.com/aquasecurity/trivy/commit/a2c522ddb229f049999c4ce74ef75a0e0f9fdc62))
* **misconf:** skip Rego errors with a nil location ([#6666](https://github.com/aquasecurity/trivy/issues/6666)) ([a126e10](https://github.com/aquasecurity/trivy/commit/a126e1075a44ef0e40c0dc1e214d1c5955f80242))
* node-collector high and critical cves ([#6707](https://github.com/aquasecurity/trivy/issues/6707)) ([ff32deb](https://github.com/aquasecurity/trivy/commit/ff32deb7bf9163c06963f557228260b3b8c161ed))
* **plugin:** initialize logger ([#6836](https://github.com/aquasecurity/trivy/issues/6836)) ([728e77a](https://github.com/aquasecurity/trivy/commit/728e77a7261dc3fcda1e61e79be066c789bbba0c))
* **python:** add package name and version validation for `requirements.txt` files. ([#6804](https://github.com/aquasecurity/trivy/issues/6804)) ([ea3a124](https://github.com/aquasecurity/trivy/commit/ea3a124fc7162c30c7f1a59bdb28db0b3c8bb86d))
* **report:** hide empty tables if all vulns has been filtered ([#6352](https://github.com/aquasecurity/trivy/issues/6352)) ([3d388d8](https://github.com/aquasecurity/trivy/commit/3d388d8552ef42d4d54176309a38c1879008527b))
* **sbom:** fix panic for `convert` mode when scanning json file derived from sbom file ([#6808](https://github.com/aquasecurity/trivy/issues/6808)) ([f92ea09](https://github.com/aquasecurity/trivy/commit/f92ea096856c7c262b05bd4d31c62689ebafac82))
* use of specified context to obtain cluster name ([#6645](https://github.com/aquasecurity/trivy/issues/6645)) ([39ebed4](https://github.com/aquasecurity/trivy/commit/39ebed45f8c218509d264bd3f3ca548fc33d2b3a))


### Performance Improvements

* **misconf:** parse rego input once ([#6615](https://github.com/aquasecurity/trivy/issues/6615)) ([67c6b1d](https://github.com/aquasecurity/trivy/commit/67c6b1d473999003d682bdb42657bbf3a4a69a9c))
