workspace(name = "toktok")

# Protobuf
# =========================================================

# proto_library rules implicitly depend on @com_google_protobuf//:protoc,
# which is the proto-compiler.
# This statement defines the @com_google_protobuf repo.
http_archive(
    name = "com_google_protobuf",
    sha256 = "0cc6607e2daa675101e9b7398a436f09167dffb8ca0489b0307ff7260498c13c",
    strip_prefix = "protobuf-3.5.0",
    urls = ["https://github.com/google/protobuf/archive/v3.5.0.tar.gz"],
)

# Haskell
# =========================================================

RULES_HASKELL_COMMIT = "17e070bab304f0a075de42430415a27f3b8e13b9"

http_archive(
    name = "io_tweag_rules_haskell",
    sha256 = "8c020e3ae251272dea25568baeddf6025211632e26a8bfa34c979e661c730ae3",
    strip_prefix = "rules_haskell-%s" % RULES_HASKELL_COMMIT,
    urls = ["https://github.com/tweag/rules_haskell/archive/%s.tar.gz" % RULES_HASKELL_COMMIT],
)

load("@io_tweag_rules_haskell//haskell:repositories.bzl", "haskell_repositories")

haskell_repositories()

register_toolchains("//:ghc")

new_local_repository(
    name = "my_ghc",
    build_file = "third_party/BUILD.ghc",
    path = "/usr",  # Change path accordingly.
)

new_http_archive(
    name = "haskell_MissingH",
    build_file = "third_party/haskell/BUILD.MissingH",
    sha256 = "283f2afd46625d98b4e29f77edadfa5e6009a227812ee2ece10091ad6a7e9b71",
    strip_prefix = "MissingH-1.4.0.1",
    urls = ["https://hackage.haskell.org/package/MissingH-1.4.0.1/MissingH-1.4.0.1.tar.gz"],
)

new_http_archive(
    name = "haskell_MonadRandom",
    build_file = "third_party/haskell/BUILD.MonadRandom",
    sha256 = "9e3f0f92807285302036dc504066ae6d968c8b0b4c25d9360888f31fe1730d87",
    strip_prefix = "MonadRandom-0.5.1",
    urls = ["https://hackage.haskell.org/package/MonadRandom-0.5.1/MonadRandom-0.5.1.tar.gz"],
)

new_http_archive(
    name = "haskell_QuickCheck",
    build_file = "third_party/haskell/BUILD.QuickCheck",
    sha256 = "488c5652139da0bac8b3e7d76f11320ded298549e62db530938bfee9ca981876",
    strip_prefix = "QuickCheck-2.11.3",
    urls = ["https://hackage.haskell.org/package/QuickCheck-2.11.3/QuickCheck-2.11.3.tar.gz"],
)

new_http_archive(
    name = "haskell_appar",
    build_file = "third_party/haskell/BUILD.appar",
    sha256 = "58ea66abe4dd502d2fc01eecdb0828d5e214704a3c1b33b1f8b33974644c4b26",
    strip_prefix = "appar-0.1.4",
    urls = ["https://hackage.haskell.org/package/appar-0.1.4/appar-0.1.4.tar.gz"],
)

new_http_archive(
    name = "haskell_async",
    build_file = "third_party/haskell/BUILD.async",
    sha256 = "8f0b86022a1319d3c1c68655790da4b7f98017982e27ec3f3dbfe01029d39027",
    strip_prefix = "async-2.2.1",
    urls = ["https://hackage.haskell.org/package/async-2.2.1/async-2.2.1.tar.gz"],
)

new_http_archive(
    name = "haskell_base_orphans",
    build_file = "third_party/haskell/BUILD.base-orphans",
    sha256 = "c7282aa7516652e6e4a78ccdfb654a99c9da683875748ad5898a3f200be7ad0e",
    strip_prefix = "base-orphans-0.6",
    urls = ["https://hackage.haskell.org/package/base-orphans-0.6/base-orphans-0.6.tar.gz"],
)

new_http_archive(
    name = "haskell_base16_bytestring",
    build_file = "third_party/haskell/BUILD.base16-bytestring",
    sha256 = "5afe65a152c5418f5f4e3579a5e0d5ca19c279dc9bf31c1a371ccbe84705c449",
    strip_prefix = "base16-bytestring-0.1.1.6",
    urls = ["https://hackage.haskell.org/package/base16-bytestring-0.1.1.6/base16-bytestring-0.1.1.6.tar.gz"],
)

new_http_archive(
    name = "haskell_bifunctors",
    build_file = "third_party/haskell/BUILD.bifunctors",
    sha256 = "332bb2ea19e77dac55282daff8046d89f69514ced5b987779d887e53b5d7cb11",
    strip_prefix = "bifunctors-5.5.2",
    urls = ["https://hackage.haskell.org/package/bifunctors-5.5.2/bifunctors-5.5.2.tar.gz"],
)

new_http_archive(
    name = "haskell_binary_bits",
    build_file = "third_party/haskell/BUILD.binary-bits",
    sha256 = "16534a018a4754d8d1eab051711c23fb741f41a0d141b289001c52824b5be794",
    strip_prefix = "binary-bits-0.5",
    urls = ["https://hackage.haskell.org/package/binary-bits-0.5/binary-bits-0.5.tar.gz"],
)

new_http_archive(
    name = "haskell_binary_conduit",
    build_file = "third_party/haskell/BUILD.binary-conduit",
    sha256 = "21d417aae0f9441ecd0e4f5aaac03bf9692fb9e85e48076c774d961567d14b1b",
    strip_prefix = "binary-conduit-1.2.5",
    urls = ["https://hackage.haskell.org/package/binary-conduit-1.2.5/binary-conduit-1.2.5.tar.gz"],
)

new_http_archive(
    name = "haskell_blaze_builder",
    build_file = "third_party/haskell/BUILD.blaze-builder",
    sha256 = "9ad3e4661bf5556d650fb9aa56a3ad6e6eec7575e87d472e8ab6d15eaef163d4",
    strip_prefix = "blaze-builder-0.4.0.2",
    urls = ["https://hackage.haskell.org/package/blaze-builder-0.4.0.2/blaze-builder-0.4.0.2.tar.gz"],
)

new_http_archive(
    name = "haskell_byteorder",
    build_file = "third_party/haskell/BUILD.byteorder",
    sha256 = "bd20bbb586947f99c38a4c93d9d0266f49f6fc581767b51ba568f6d5d52d2919",
    strip_prefix = "byteorder-1.0.4",
    urls = ["https://hackage.haskell.org/package/byteorder-1.0.4/byteorder-1.0.4.tar.gz"],
)

new_http_archive(
    name = "haskell_clock",
    build_file = "third_party/haskell/BUILD.clock",
    sha256 = "886601978898d3a91412fef895e864576a7125d661e1f8abc49a2a08840e691f",
    strip_prefix = "clock-0.7.2",
    urls = ["https://hackage.haskell.org/package/clock-0.7.2/clock-0.7.2.tar.gz"],
)

new_http_archive(
    name = "haskell_comonad",
    build_file = "third_party/haskell/BUILD.comonad",
    sha256 = "a7f4584d634051123c547f0d10f88eaf23d99229dbd01dfdcd98cddd41e54df6",
    strip_prefix = "comonad-5.0.3",
    urls = ["https://hackage.haskell.org/package/comonad-5.0.3/comonad-5.0.3.tar.gz"],
)

new_http_archive(
    name = "haskell_conduit",
    build_file = "third_party/haskell/BUILD.conduit",
    sha256 = "239d1bac614bc1085315ad8d15275471fc7c0eaef05950429d40a65bd73711ac",
    strip_prefix = "conduit-1.2.13",
    urls = ["https://hackage.haskell.org/package/conduit-1.2.13/conduit-1.2.13.tar.gz"],
)

new_http_archive(
    name = "haskell_conduit_extra",
    build_file = "third_party/haskell/BUILD.conduit-extra",
    sha256 = "1d5b66284703a4b9fb96a4c6a2213727208639871a675da9755e9a963fa230f6",
    strip_prefix = "conduit-extra-1.2.3.2",
    urls = ["https://hackage.haskell.org/package/conduit-extra-1.2.3.2/conduit-extra-1.2.3.2.tar.gz"],
)

new_http_archive(
    name = "haskell_data_binary_ieee754",
    build_file = "third_party/haskell/BUILD.data-binary-ieee754",
    sha256 = "59975abed8f4caa602f0780c10a9b2493479e6feb71ad189bb10c3ac5678df0a",
    strip_prefix = "data-binary-ieee754-0.4.4",
    urls = ["https://hackage.haskell.org/package/data-binary-ieee754-0.4.4/data-binary-ieee754-0.4.4.tar.gz"],
)

new_http_archive(
    name = "haskell_data_default_class",
    build_file = "third_party/haskell/BUILD.data-default-class",
    sha256 = "4f01b423f000c3e069aaf52a348564a6536797f31498bb85c3db4bd2d0973e56",
    strip_prefix = "data-default-class-0.1.2.0",
    urls = ["https://hackage.haskell.org/package/data-default-class-0.1.2.0/data-default-class-0.1.2.0.tar.gz"],
)

new_http_archive(
    name = "haskell_data_default_instances_base",
    build_file = "third_party/haskell/BUILD.data-default-instances-base",
    sha256 = "844fe453f674b6b0998da804465914abce8936c5e640d8bb8bff37ad07d7a17a",
    strip_prefix = "data-default-instances-base-0.1.0.1",
    urls = ["https://hackage.haskell.org/package/data-default-instances-base-0.1.0.1/data-default-instances-base-0.1.0.1.tar.gz"],
)

new_http_archive(
    name = "haskell_exceptions",
    build_file = "third_party/haskell/BUILD.exceptions",
    sha256 = "4d6ad97e8e3d5dc6ce9ae68a469dc2fd3f66e9d312bc6faa7ab162eddcef87be",
    strip_prefix = "exceptions-0.8.3",
    urls = ["https://hackage.haskell.org/package/exceptions-0.8.3/exceptions-0.8.3.tar.gz"],
)

new_http_archive(
    name = "haskell_hashable",
    build_file = "third_party/haskell/BUILD.hashable",
    sha256 = "94ca8789e13bc05c1582c46b709f3b0f5aeec2092be634b8606dbd9c5915bb7a",
    strip_prefix = "hashable-1.2.6.1",
    urls = ["https://hackage.haskell.org/package/hashable-1.2.6.1/hashable-1.2.6.1.tar.gz"],
)

new_http_archive(
    name = "haskell_hslogger",
    build_file = "third_party/haskell/BUILD.hslogger",
    sha256 = "d7ca6e94a4aacb47a8dc30e3960ab8deff482d2ec9dca9a87b225e03e97e452b",
    strip_prefix = "hslogger-1.2.10",
    urls = ["https://hackage.haskell.org/package/hslogger-1.2.10/hslogger-1.2.10.tar.gz"],
)

new_http_archive(
    name = "haskell_iproute",
    build_file = "third_party/haskell/BUILD.iproute",
    sha256 = "57b8d03ca8ce92f8ec1334564f3edff53a0621ccbc43c00ba02eaa5007ee3eee",
    strip_prefix = "iproute-1.7.1",
    urls = ["https://hackage.haskell.org/package/iproute-1.7.1/iproute-1.7.1.tar.gz"],
)

new_http_archive(
    name = "haskell_language_c",
    build_file = "third_party/haskell/BUILD.language-c",
    sha256 = "a7447123f9b3bec9319ee2a22b22d97f03acd6566b4f6caf5b9a1f71e4f7a9ca",
    strip_prefix = "language-c-0.7.1",
    urls = ["https://hackage.haskell.org/package/language-c-0.7.1/language-c-0.7.1.tar.gz"],
)

new_http_archive(
    name = "haskell_lifted_base",
    build_file = "third_party/haskell/BUILD.lifted-base",
    sha256 = "8ec47a9fce7cf5913766a5c53e1b2cf254be733fa9d62e6e2f3f24e538005aab",
    strip_prefix = "lifted-base-0.2.3.11",
    urls = ["https://hackage.haskell.org/package/lifted-base-0.2.3.11/lifted-base-0.2.3.11.tar.gz"],
)

new_http_archive(
    name = "haskell_mmorph",
    build_file = "third_party/haskell/BUILD.mmorph",
    sha256 = "c1bcb45560753203f5ce3952f3c8a100b7d5b37c91746372c1da4988c4db74de",
    strip_prefix = "mmorph-1.1.0",
    urls = ["https://hackage.haskell.org/package/mmorph-1.1.0/mmorph-1.1.0.tar.gz"],
)

new_http_archive(
    name = "haskell_monad_control",
    build_file = "third_party/haskell/BUILD.monad-control",
    sha256 = "1e34a21d123f2ed8bb2708e7f30343fa1d9d7f36881f9871cbcca4bb07e7e433",
    strip_prefix = "monad-control-1.0.2.2",
    urls = ["https://hackage.haskell.org/package/monad-control-1.0.2.2/monad-control-1.0.2.2.tar.gz"],
)

new_http_archive(
    name = "haskell_mono_traversable",
    build_file = "third_party/haskell/BUILD.mono-traversable",
    sha256 = "991290797bd77ce2f2e23dd5dea32fb159c6cb9310615f64a0703ea4c6373935",
    strip_prefix = "mono-traversable-1.0.8.1",
    urls = ["https://hackage.haskell.org/package/mono-traversable-1.0.8.1/mono-traversable-1.0.8.1.tar.gz"],
)

new_http_archive(
    name = "haskell_mtl",
    build_file = "third_party/haskell/BUILD.mtl",
    sha256 = "cae59d79f3a16f8e9f3c9adc1010c7c6cdddc73e8a97ff4305f6439d855c8dc5",
    strip_prefix = "mtl-2.2.1",
    urls = ["https://hackage.haskell.org/package/mtl-2.2.1/mtl-2.2.1.tar.gz"],
)

new_http_archive(
    name = "haskell_network",
    build_file = "third_party/haskell/BUILD.network",
    sha256 = "776668b0a969d0d57ebabf78943cfc21a1aaf7e5e2ae6288322292125c9440f5",
    strip_prefix = "network-2.6.3.3",
    urls = ["https://hackage.haskell.org/package/network-2.6.3.3/network-2.6.3.3.tar.gz"],
)

new_http_archive(
    name = "haskell_old_locale",
    build_file = "third_party/haskell/BUILD.old-locale",
    sha256 = "dbaf8bf6b888fb98845705079296a23c3f40ee2f449df7312f7f7f1de18d7b50",
    strip_prefix = "old-locale-1.0.0.7",
    urls = ["https://hackage.haskell.org/package/old-locale-1.0.0.7/old-locale-1.0.0.7.tar.gz"],
)

new_http_archive(
    name = "haskell_old_time",
    build_file = "third_party/haskell/BUILD.old-time",
    sha256 = "1ccb158b0f7851715d36b757c523b026ca1541e2030d02239802ba39b4112bc1",
    strip_prefix = "old-time-1.1.0.3",
    urls = ["https://hackage.haskell.org/package/old-time-1.1.0.3/old-time-1.1.0.3.tar.gz"],
)

new_http_archive(
    name = "haskell_parsec",
    build_file = "third_party/haskell/BUILD.parsec",
    sha256 = "6f87251cb1d11505e621274dec15972de924a9074f07f7430a18892064c2676e",
    strip_prefix = "parsec-3.1.11",
    urls = ["https://hackage.haskell.org/package/parsec-3.1.11/parsec-3.1.11.tar.gz"],
)

new_http_archive(
    name = "haskell_primitive",
    build_file = "third_party/haskell/BUILD.primitive",
    sha256 = "b8e8d70213e22b3fab0e0d11525c02627489618988fdc636052ca0adce282ae1",
    strip_prefix = "primitive-0.6.2.0",
    urls = ["https://hackage.haskell.org/package/primitive-0.6.2.0/primitive-0.6.2.0.tar.gz"],
)

new_http_archive(
    name = "haskell_profunctors",
    build_file = "third_party/haskell/BUILD.profunctors",
    sha256 = "e981e6a33ac99d38a947a749179bbea3c294ecf6bfde41660fe6d8d5a2e43768",
    strip_prefix = "profunctors-5.2.2",
    urls = ["https://hackage.haskell.org/package/profunctors-5.2.2/profunctors-5.2.2.tar.gz"],
)

new_http_archive(
    name = "haskell_random",
    build_file = "third_party/haskell/BUILD.random",
    sha256 = "b718a41057e25a3a71df693ab0fe2263d492e759679b3c2fea6ea33b171d3a5a",
    strip_prefix = "random-1.1",
    urls = ["https://hackage.haskell.org/package/random-1.1/random-1.1.tar.gz"],
)

new_http_archive(
    name = "haskell_regex_base",
    build_file = "third_party/haskell/BUILD.regex-base",
    sha256 = "20dc5713a16f3d5e2e6d056b4beb9cfdc4368cd09fd56f47414c847705243278",
    strip_prefix = "regex-base-0.93.2",
    urls = ["https://hackage.haskell.org/package/regex-base-0.93.2/regex-base-0.93.2.tar.gz"],
)

new_http_archive(
    name = "haskell_regex_compat",
    build_file = "third_party/haskell/BUILD.regex-compat",
    sha256 = "d57cb1a5a4d66753b18eaa37a1621246f660472243b001894f970037548d953b",
    strip_prefix = "regex-compat-0.95.1",
    urls = ["https://hackage.haskell.org/package/regex-compat-0.95.1/regex-compat-0.95.1.tar.gz"],
)

new_http_archive(
    name = "haskell_regex_posix",
    build_file = "third_party/haskell/BUILD.regex-posix",
    sha256 = "56019921cd4a4c9682b81ec614236fea816ba8ed8785a1640cd66d8b24fc703e",
    strip_prefix = "regex-posix-0.95.2",
    urls = ["https://hackage.haskell.org/package/regex-posix-0.95.2/regex-posix-0.95.2.tar.gz"],
)

new_http_archive(
    name = "haskell_resourcet",
    build_file = "third_party/haskell/BUILD.resourcet",
    sha256 = "346ed5c3eca87e1b2df5ca97419bd896e27ad39d997b8eea5b62f67c98a824d9",
    strip_prefix = "resourcet-1.1.11",
    urls = ["https://hackage.haskell.org/package/resourcet-1.1.11/resourcet-1.1.11.tar.gz"],
)

new_http_archive(
    name = "haskell_saltine",
    build_file = "third_party/haskell/BUILD.saltine",
    sha256 = "a2bc34fb3b9485c300e4a9eac4e6d83ef584275016be845fe5e28aec08df6dc2",
    strip_prefix = "saltine-0.1.0.0",
    urls = ["https://hackage.haskell.org/package/saltine-0.1.0.0/saltine-0.1.0.0.tar.gz"],
)

new_http_archive(
    name = "haskell_semigroups",
    build_file = "third_party/haskell/BUILD.semigroups",
    sha256 = "589e3042329a6bcffb5c0e85834143586db22eb7a2aae094d492cd004f685d27",
    strip_prefix = "semigroups-0.18.4",
    urls = ["https://hackage.haskell.org/package/semigroups-0.18.4/semigroups-0.18.4.tar.gz"],
)

new_http_archive(
    name = "haskell_split",
    build_file = "third_party/haskell/BUILD.split",
    sha256 = "1dcd674f7c5f276f33300f5fd59e49d1ac6fc92ae949fd06a0f6d3e9d9ac1413",
    strip_prefix = "split-0.2.3.3",
    urls = ["https://hackage.haskell.org/package/split-0.2.3.3/split-0.2.3.3.tar.gz"],
)

new_http_archive(
    name = "haskell_stm",
    build_file = "third_party/haskell/BUILD.stm",
    sha256 = "31d7db183f13beed5c71409d12747a7f4cf3e145630553dc86336208540859a7",
    strip_prefix = "stm-2.4.5.0",
    urls = ["https://hackage.haskell.org/package/stm-2.4.5.0/stm-2.4.5.0.tar.gz"],
)

new_http_archive(
    name = "haskell_streaming_commons",
    build_file = "third_party/haskell/BUILD.streaming-commons",
    sha256 = "43fcae90df5548d9968b31371f13ec7271df86ac34a484c094616867ed4217a7",
    strip_prefix = "streaming-commons-0.1.19",
    urls = ["https://hackage.haskell.org/package/streaming-commons-0.1.19/streaming-commons-0.1.19.tar.gz"],
)

new_http_archive(
    name = "haskell_syb",
    build_file = "third_party/haskell/BUILD.syb",
    sha256 = "b8757dce5ab4045c49a0ae90407d575b87ee5523a7dd5dfa5c9d54fcceff42b5",
    strip_prefix = "syb-0.7",
    urls = ["https://hackage.haskell.org/package/syb-0.7/syb-0.7.tar.gz"],
)

new_http_archive(
    name = "haskell_tagged",
    build_file = "third_party/haskell/BUILD.tagged",
    sha256 = "e47c51c955ed77b0fa36897f652df990aa0a8c4eb278efaddcd604be00fc8d99",
    strip_prefix = "tagged-0.8.5",
    urls = ["https://hackage.haskell.org/package/tagged-0.8.5/tagged-0.8.5.tar.gz"],
)

new_http_archive(
    name = "haskell_text",
    build_file = "third_party/haskell/BUILD.text",
    sha256 = "20e0b1627f613b32cc7f2d2e8dcc48a4a61938b24f3d14fb77cee694f0c9311a",
    strip_prefix = "text-1.2.3.0",
    urls = ["https://hackage.haskell.org/package/text-1.2.3.0/text-1.2.3.0.tar.gz"],
)

new_http_archive(
    name = "haskell_tf_random",
    build_file = "third_party/haskell/BUILD.tf-random",
    sha256 = "2e30cec027b313c9e1794d326635d8fc5f79b6bf6e7580ab4b00186dadc88510",
    strip_prefix = "tf-random-0.5",
    urls = ["https://hackage.haskell.org/package/tf-random-0.5/tf-random-0.5.tar.gz"],
)

new_http_archive(
    name = "haskell_th_abstraction",
    build_file = "third_party/haskell/BUILD.th-abstraction",
    sha256 = "e52e289a547d68f203d65f2e63ec2d87a3c613007d2fe873615c0969b981823c",
    strip_prefix = "th-abstraction-0.2.6.0",
    urls = ["https://hackage.haskell.org/package/th-abstraction-0.2.6.0/th-abstraction-0.2.6.0.tar.gz"],
)

new_http_archive(
    name = "haskell_transformers_base",
    build_file = "third_party/haskell/BUILD.transformers-base",
    sha256 = "6aa3494fc70659342fbbb163035d5827ecfd8079e3c929e2372adf771fd52387",
    strip_prefix = "transformers-base-0.4.4",
    urls = ["https://hackage.haskell.org/package/transformers-base-0.4.4/transformers-base-0.4.4.tar.gz"],
)

new_http_archive(
    name = "haskell_transformers_compat",
    build_file = "third_party/haskell/BUILD.transformers-compat",
    sha256 = "d881ef4ec164b631591b222efe7ff555af6d5397c9d86475b309ba9402a8ca9f",
    strip_prefix = "transformers-compat-0.5.1.4",
    urls = ["https://hackage.haskell.org/package/transformers-compat-0.5.1.4/transformers-compat-0.5.1.4.tar.gz"],
)

new_http_archive(
    name = "haskell_typed_process",
    build_file = "third_party/haskell/BUILD.typed-process",
    sha256 = "d214d88575dc0fe919d23eacd91a212ed7bf5b1dbb4360038e99926ff9bcdcd0",
    strip_prefix = "typed-process-0.2.1.0",
    urls = ["https://hackage.haskell.org/package/typed-process-0.2.1.0/typed-process-0.2.1.0.tar.gz"],
)

new_http_archive(
    name = "haskell_unliftio_core",
    build_file = "third_party/haskell/BUILD.unliftio-core",
    sha256 = "7550b017d87af53ae3e0d3b8524e24a77faf739073f35e40663454a9e9752385",
    strip_prefix = "unliftio-core-0.1.1.0",
    urls = ["https://hackage.haskell.org/package/unliftio-core-0.1.1.0/unliftio-core-0.1.1.0.tar.gz"],
)

new_http_archive(
    name = "haskell_unordered_containers",
    build_file = "third_party/haskell/BUILD.unordered-containers",
    sha256 = "a4a188359ff28640359131061953f7dbb8258da8ecf0542db0d23f08bfa6eea8",
    strip_prefix = "unordered-containers-0.2.8.0",
    urls = ["https://hackage.haskell.org/package/unordered-containers-0.2.8.0/unordered-containers-0.2.8.0.tar.gz"],
)

new_http_archive(
    name = "haskell_vector",
    build_file = "third_party/haskell/BUILD.vector",
    sha256 = "b100ee79b9da2651276278cd3e0f08a3c152505cc52982beda507515af173d7b",
    strip_prefix = "vector-0.12.0.1",
    urls = ["https://hackage.haskell.org/package/vector-0.12.0.1/vector-0.12.0.1.tar.gz"],
)

new_http_archive(
    name = "haskell_vector_algorithms",
    build_file = "third_party/haskell/BUILD.vector-algorithms",
    sha256 = "ed460a41ca068f568bc2027579ab14185fbb72c7ac469b5179ae5f8a52719070",
    strip_prefix = "vector-algorithms-0.7.0.1",
    urls = ["https://hackage.haskell.org/package/vector-algorithms-0.7.0.1/vector-algorithms-0.7.0.1.tar.gz"],
)

new_http_archive(
    name = "haskell_zlib",
    build_file = "third_party/haskell/BUILD.zlib",
    sha256 = "e4eb4e636caf07a16a9730ce469a00b65d5748f259f43edd904dd457b198a2bb",
    strip_prefix = "zlib-0.6.1.2",
    urls = ["https://hackage.haskell.org/package/zlib-0.6.1.2/zlib-0.6.1.2.tar.gz"],
)

# Go
# =========================================================

http_archive(
    name = "io_bazel_rules_go",
    sha256 = "4d8d6244320dd751590f9100cf39fd7a4b75cd901e1f3ffdfd6f048328883695",
    urls = ["https://github.com/bazelbuild/rules_go/releases/download/0.9.0/rules_go-0.9.0.tar.gz"],
)

http_archive(
    name = "bazel_gazelle",
    sha256 = "0103991d994db55b3b5d7b06336f8ae355739635e0c2379dea16b8213ea5a223",
    urls = ["https://github.com/bazelbuild/bazel-gazelle/releases/download/0.9/bazel-gazelle-0.9.tar.gz"],
)

load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains")
load("@io_bazel_rules_go//go/private:go_repository.bzl", "go_repository")
load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies")

go_rules_dependencies()

go_register_toolchains()

gazelle_dependencies()

go_repository(
    name = "com_github_streamrail_concurrent_map",
    commit = "master",
    importpath = "github.com/streamrail/concurrent-map",
)

#go_repository(
#    name = "com_github_petermattis_goid",
#    commit = "master",
#    importpath = "github.com/petermattis/goid",
#)
#
# Workaround for https://github.com/bazelbuild/rules_go/issues/1262.
new_http_archive(
    name = "com_github_petermattis_goid",
    build_file = "third_party/BUILD.com_github_petermattis_goid",
    sha256 = "2c9e36159a9e3061d3b2839e33ff453d238a247483d9eac3917b567cc50b5f1c",
    strip_prefix = "goid-176e84a949d354dcef722e602b312b1a75bacddc",
    urls = ["https://github.com/petermattis/goid/archive/176e84a949d354dcef722e602b312b1a75bacddc.tar.gz"],
)

go_repository(
    name = "com_github_sasha_s_go_deadlock",
    commit = "master",
    importpath = "github.com/sasha-s/go-deadlock",
)

go_repository(
    name = "org_bitbucket_kardianos_osext",
    commit = "tip",
    importpath = "bitbucket.org/kardianos/osext",
)

# C/C++ dependencies
# =========================================================

new_local_repository(
    name = "asound",
    build_file = "third_party/BUILD.asound",
    path = "/usr",
)

new_local_repository(
    name = "openal",
    build_file = "third_party/BUILD.openal",
    path = "/usr",
)

new_local_repository(
    name = "opencv",
    build_file = "third_party/BUILD.opencv",
    path = "/usr",
)

new_http_archive(
    name = "bzip2",
    build_file = "third_party/BUILD.bzip2",
    sha256 = "a2848f34fcd5d6cf47def00461fcb528a0484d8edef8208d6d2e2909dc61d9cd",
    strip_prefix = "bzip2-1.0.6",
    urls = ["http://www.bzip.org/1.0.6/bzip2-1.0.6.tar.gz"],
)

new_http_archive(
    name = "curl",
    build_file = "third_party/BUILD.curl",
    sha256 = "cc245bf9a1a42a45df491501d97d5593392a03f7b4f07b952793518d97666115",
    strip_prefix = "curl-7.58.0",
    urls = ["https://github.com/curl/curl/releases/download/curl-7_58_0/curl-7.58.0.tar.gz"],
)

new_http_archive(
    name = "ffmpeg",
    build_file = "third_party/BUILD.ffmpeg",
    sha256 = "f3443e20154a590ab8a9eef7bc951e8731425efc75b44ff4bee31d8a7a574a2c",
    strip_prefix = "ffmpeg-3.4.1",
    urls = ["http://ffmpeg.org/releases/ffmpeg-3.4.1.tar.bz2"],
)

new_http_archive(
    name = "filter_audio",
    build_file = "third_party/BUILD.filter_audio",
    sha256 = "fb135592c5133c3b4b664da18f988f58609db912f204059abe16277df044a366",
    strip_prefix = "filter_audio-0.0.1",
    urls = ["https://github.com/irungentoo/filter_audio/archive/v0.0.1.tar.gz"],
)

http_archive(
    name = "com_google_googletest",
    sha256 = "da3d22cc2e096456573939ec21a1d989aca5a60fa1c89037ae05205c00202e4a",
    strip_prefix = "googletest-15392f1a38fa0b8c3f13a9732e94b209069efa1c",
    urls = ["https://github.com/google/googletest/archive/15392f1a38fa0b8c3f13a9732e94b209069efa1c.tar.gz"],
)

new_http_archive(
    name = "json",
    build_file = "third_party/BUILD.json",
    sha256 = "2b7234fca394d1e27b7e017117ed80b7518fafbb4f4c13a7c069624f6f924673",
    strip_prefix = "include",
    urls = ["https://github.com/nlohmann/json/releases/download/v3.1.0/include.zip"],
)

new_http_archive(
    name = "libcap",
    build_file = "third_party/BUILD.libcap",
    sha256 = "4ca80dc6f9f23d14747e4b619fd9784434c570e24a7346f326c692784ed83a86",
    strip_prefix = "libcap-2.25",
    urls = ["https://www.kernel.org/pub/linux/libs/security/linux-privs/libcap2/libcap-2.25.tar.gz"],
)

new_http_archive(
    name = "libconfig",
    build_file = "third_party/BUILD.libconfig",
    sha256 = "f67ac44099916ae260a6c9e290a90809e7d782d96cdd462cac656ebc5b685726",
    strip_prefix = "libconfig-1.7.2",
    urls = ["https://github.com/hyperrealm/libconfig/archive/v1.7.2.tar.gz"],
)

new_http_archive(
    name = "libexif",
    build_file = "third_party/BUILD.libexif",
    sha256 = "8cb37aa1745ca9050403c501ad4da2924e98ec5460bbd5c9d09bd57f0c746636",
    strip_prefix = "libexif-libexif-0_6_21-release",
    urls = ["https://github.com/libexif/libexif/archive/libexif-0_6_21-release.tar.gz"],
)

new_http_archive(
    name = "libidn2",
    build_file = "third_party/BUILD.libidn2",
    sha256 = "644b6b03b285fb0ace02d241d59483d98bc462729d8bb3608d5cad5532f3d2f0",
    strip_prefix = "libidn2-2.0.4",
    urls = ["https://ftp.gnu.org/gnu/libidn/libidn2-2.0.4.tar.gz"],
)

new_http_archive(
    name = "libqrencode",
    build_file = "third_party/BUILD.libqrencode",
    sha256 = "c2c8a8110354463a3332cb48abf8581c8d94136af4dc1418f891cc9c7719e3c1",
    strip_prefix = "libqrencode-4.0.0",
    urls = ["https://github.com/fukuchi/libqrencode/archive/v4.0.0.tar.gz"],
)

new_http_archive(
    name = "libsodium",
    build_file = "third_party/BUILD.libsodium",
    sha256 = "eeadc7e1e1bcef09680fb4837d448fbdf57224978f865ac1c16745868fbd0533",
    strip_prefix = "libsodium-1.0.16",
    urls = ["https://github.com/jedisct1/libsodium/releases/download/1.0.16/libsodium-1.0.16.tar.gz"],
)

new_http_archive(
    name = "libvpx",
    build_file = "third_party/BUILD.libvpx",
    sha256 = "1fec931eb5c94279ad219a5b6e0202358e94a93a90cfb1603578c326abfc1238",
    strip_prefix = "libvpx-1.7.0",
    urls = ["https://github.com/webmproject/libvpx/archive/v1.7.0.tar.gz"],
)

new_http_archive(
    name = "libzmq",
    build_file = "third_party/BUILD.libzmq",
    sha256 = "b428c6cdf1df4b5cdcb3a6727c6ece85c7fb05d7907c532566a115b4dda113a8",
    strip_prefix = "libzmq-4.2.3",
    urls = ["https://github.com/zeromq/libzmq/archive/v4.2.3.tar.gz"],
)

new_http_archive(
    name = "openssl",
    build_file = "third_party/BUILD.openssl",
    sha256 = "4f4bc907caff1fee6ff8593729e5729891adcee412049153a3bb4db7625e8364",
    strip_prefix = "openssl-OpenSSL_1_0_2n",
    urls = ["https://github.com/openssl/openssl/archive/OpenSSL_1_0_2n.tar.gz"],
)

new_http_archive(
    name = "opus",
    build_file = "third_party/BUILD.opus",
    sha256 = "6d258ffc874070087d15c584c0c491864baad14a55873730d9af35bf72fb1ce1",
    strip_prefix = "opus-1.2.1",
    urls = ["https://github.com/xiph/opus/archive/v1.2.1.tar.gz"],
)

new_http_archive(
    name = "portaudio",
    build_file = "third_party/BUILD.portaudio",
    sha256 = "f5a21d7dcd6ee84397446fa1fa1a0675bb2e8a4a6dceb4305a8404698d8d1513",
    strip_prefix = "portaudio",
    urls = ["http://www.portaudio.com/archives/pa_stable_v190600_20161030.tgz"],
)

new_http_archive(
    name = "sndfile",
    build_file = "third_party/BUILD.sndfile",
    sha256 = "1ff33929f042fa333aed1e8923aa628c3ee9e1eb85512686c55092d1e5a9dfa9",
    strip_prefix = "libsndfile-1.0.28",
    urls = ["http://www.mega-nerd.com/libsndfile/files/libsndfile-1.0.28.tar.gz"],
)

new_http_archive(
    name = "libxz",
    build_file = "third_party/BUILD.libxz",
    sha256 = "71928b357d0a09a12a4b4c5fafca8c31c19b0e7d3b8ebb19622e96f26dbf28cb",
    strip_prefix = "xz-5.2.3",
    urls = ["https://netix.dl.sourceforge.net/project/lzmautils/xz-5.2.3.tar.gz"],
)

new_http_archive(
    name = "yasm",
    build_file = "third_party/BUILD.yasm",
    sha256 = "f708be0b7b8c59bc1dbe7134153cd2f31faeebaa8eec48676c10f972a1f13df3",
    strip_prefix = "yasm-1.3.0",
    urls = ["https://github.com/yasm/yasm/archive/v1.3.0.tar.gz"],
)

new_http_archive(
    name = "zlib",
    build_file = "third_party/BUILD.zlib",
    sha256 = "629380c90a77b964d896ed37163f5c3a34f6e6d897311f1df2a7016355c45eff",
    strip_prefix = "zlib-1.2.11",
    urls = ["https://github.com/madler/zlib/archive/v1.2.11.tar.gz"],
)

# Maven dependencies
# =========================================================

load("@bazel_tools//tools/build_defs/repo:maven_rules.bzl", "maven_aar")

local_repository(
    name = "org_bytedeco_javacpp_presets_ffmpeg_platform",
    path = "third_party/javacpp/ffmpeg",
)

local_repository(
    name = "org_bytedeco_javacpp_presets_opencv_platform",
    path = "third_party/javacpp/opencv",
)

maven_aar(
    name = "com_timehop_stickyheadersrecyclerview_library",
    artifact = "com.timehop.stickyheadersrecyclerview:library:0.4.3",
    sha1 = "44a237a0ebff7c7ebb10c79698f97f6d635d0e26",
)

maven_aar(
    name = "com_tonicartos_superslim",
    artifact = "com.tonicartos:superslim:0.4.13",
    sha1 = "b05a0931a2d97fd370dc4ae6e003a9f57eada69a",
)

maven_aar(
    name = "de_hdodenhof_circleimageview",
    artifact = "de.hdodenhof:circleimageview:2.1.0",
    sha1 = "c0fcd515432ccb654bc5b44af60320703880a0f6",
)

maven_aar(
    name = "com_sothree_slidinguppanel_library",
    artifact = "com.sothree.slidinguppanel:library:3.4.0",
    sha1 = "a46c103238d666c097f6fefcffb479ebb450d365",
)

maven_jar(
    name = "com_chuusai_shapeless",
    artifact = "com.chuusai:shapeless_2.11:2.3.3",
    sha1 = "ea34d4b6128b9090386945dcb952816bd9e87ce2",
)

maven_jar(
    name = "com_google_guava_guava",
    artifact = "com.google.guava:guava:19.0",
    sha1 = "6ce200f6b23222af3d8abb6b6459e6c44f4bb0e9",
)

maven_jar(
    name = "com_intellij_annotations",
    artifact = "com.intellij:annotations:12.0",
    sha1 = "bbcf6448f6d40abe506e2c83b70a3e8bfd2b4539",
)

maven_jar(
    name = "com_typesafe_scala_logging_scala_logging",
    artifact = "com.typesafe.scala-logging:scala-logging_2.11:3.7.2",
    sha1 = "5015fe84c5aec4f8eb3daa2d1663d447d65f8c02",
)

maven_jar(
    name = "junit_junit",
    artifact = "junit:junit:4.12",
    sha1 = "2973d150c0dc1fefe998f834810d68f278ea58ec",
)

maven_jar(
    name = "log4j_log4j",
    artifact = "log4j:log4j:1.2.17",
    sha1 = "5af35056b4d257e4b64b9e8069c0746e8b08629f",
)

maven_jar(
    name = "org_apache_commons_commons_lang3",
    artifact = "org.apache.commons:commons-lang3:3.4",
    sha1 = "5fe28b9518e58819180a43a850fbc0dd24b7c050",
)

maven_jar(
    name = "org_bytedeco_javacpp",
    artifact = "org.bytedeco:javacpp:1.4",
    sha1 = "6e9062d70f863a4e55b3827d42d302f94e89d7e5",
)

maven_jar(
    name = "org_bytedeco_javacpp_presets_ffmpeg",
    artifact = "org.bytedeco.javacpp-presets:ffmpeg:3.4.1-1.4",
    sha1 = "bf46f2d74014475c948f1a8e063fae50ab724520",
)

maven_jar(
    name = "org_bytedeco_javacpp_presets_opencv",
    artifact = "org.bytedeco.javacpp-presets:opencv:3.4.0-1.4",
    sha1 = "b82eeed2295f30369044b2520937d764efeb3e1e",
)

maven_jar(
    name = "org_bytedeco_javacv",
    artifact = "org.bytedeco:javacv:1.4",
    sha1 = "c443d8c648fb7e53428837e469ced47369a297af",
)

maven_jar(
    name = "org_bytedeco_javacv_platform",
    artifact = "org.bytedeco:javacv-platform:1.4",
    sha1 = "9a674bb8266e02f6c85b6f5644b7eab13119f14e",
)

maven_jar(
    name = "org_scalacheck_scalacheck",
    artifact = "org.scalacheck:scalacheck_2.11:1.13.4",
    sha1 = "7845816647d5a80d30e5a71862b31f3fee894549",
)

maven_jar(
    name = "org_scalactic_scalactic",
    artifact = "org.scalactic:scalactic_2.11:3.0.4",
    sha1 = "a97b52d531f6010b424813af260ac6ce748e187e",
)

maven_jar(
    name = "org_scalatest_scalatest",
    artifact = "org.scalatest:scalatest_2.11:3.0.4",
    sha1 = "a0df09cc87bb681674b05a883462b121866784e5",
)

maven_jar(
    name = "org_slf4j_slf4j_api",
    artifact = "org.slf4j:slf4j-api:1.7.25",
    sha1 = "da76ca59f6a57ee3102f8f9bd9cee742973efa8a",
)

maven_jar(
    name = "org_slf4j_slf4j_android",
    artifact = "org.slf4j:slf4j-android:1.7.22",
    sha1 = "74825860214ed889b38d0fc865b89af18f4e95a7",
)

maven_jar(
    name = "org_slf4j_slf4j_log4j12",
    artifact = "org.slf4j:slf4j-log4j12:1.7.22",
    sha1 = "3bb94b26c2ad2f8755302aa9bf96f03b23a76639",
)

# Scala toolchain
# =========================================================

rules_scala_version = "7522c866450cf7810eda443e91ff44d2a2286ba1"

http_archive(
    name = "io_bazel_rules_scala",
    sha256 = "66eb5e124d5542bbcab646aab34515bcb636004dd6dcb67cf8fa3f67f3f31f05",
    strip_prefix = "rules_scala-%s" % rules_scala_version,
    urls = ["https://github.com/bazelbuild/rules_scala/archive/%s.zip" % rules_scala_version],
)

load("@io_bazel_rules_scala//scala:scala.bzl", "scala_repositories")
load("@io_bazel_rules_scala//scala:toolchains.bzl", "scala_register_toolchains")
load("@io_bazel_rules_scala//scala_proto:scala_proto.bzl", "scala_proto_repositories")

scala_register_toolchains()

scala_repositories()

scala_proto_repositories()

git_repository(
    name = "gmaven_rules",
    commit = "5e89b7cdc94d002c13576fad3b28b0ae30296e55",
    remote = "https://github.com/aj-michael/gmaven_rules",
)

load("@gmaven_rules//:gmaven.bzl", "gmaven_rules")

gmaven_rules()

android_sdk_repository(
    name = "androidsdk",
    api_level = 27,
    build_tools_version = "27.0.3",
    path = "third_party/android/sdk",
)

# Qt5
# =========================================================

new_local_repository(
    name = "qt",
    build_file = "third_party/BUILD.qt",
    path = "third_party/qt",
)

# Linux headers
# =========================================================

new_local_repository(
    name = "linux",
    build_file = "third_party/BUILD.linux",
    path = "/usr/include",
)

# Python
# =========================================================

load("//tools/workspace:python.bzl", "python_repository")

python_repository(
    name = "python2",
    version = "2.7",
)

python_repository(
    name = "python3",
    version = "3.5",
)

# Node.js
# =========================================================

RULES_NODE_COMMIT = "56eadbd6e7545411e740d97fe1741c56dab42285"

http_archive(
    name = "org_pubref_rules_node",
    sha256 = "9ed54e5fda5154aeff7b5ed51b85b83cbb630f70178ca1a1798af671c6cf945c",
    strip_prefix = "rules_node-%s" % RULES_NODE_COMMIT,
    url = "https://github.com/pubref/rules_node/archive/%s.zip" % RULES_NODE_COMMIT,
)

load("@org_pubref_rules_node//node:rules.bzl", "node_repositories", "yarn_modules")

node_repositories()

yarn_modules(
    name = "yarn_modules",
    install_tools = [
        "sh",
        "dirname",
    ],
    package_json = "//js-toxcore-c:package.json",
)

yarn_modules(
    name = "mocha_modules",
    deps = {"mocha": "3.5.3"},
)
