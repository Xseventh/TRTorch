load("//tests/core/lowering:lowering_test.bzl", "lowering_test")

config_setting(
    name = "use_pre_cxx11_abi",
    values = {
        "define": "abi=pre_cxx11_abi",
    },
)

lowering_test(
    name = "test_linear_to_addmm",
)

lowering_test(
    name = "test_remove_contiguous_pass",
)

lowering_test(
    name = "test_remove_dropout_pass",
)

lowering_test(
    name = "test_reduce_to_pass",
)

lowering_test(
    name = "test_remove_detach_pass",
)

lowering_test(
    name = "test_operator_aliasing_pass",
)

lowering_test(
    name = "test_silu_to_sigmoid_multiplication",
)

lowering_test(
    name = "test_unpack_hardswish",
)

lowering_test(
    name = "test_unpack_reduce_ops",
)

test_suite(
    name = "lowering_tests",
    tests = [
        ":test_linear_to_addmm",
        ":test_operator_aliasing_pass",
        ":test_remove_contiguous_pass",
        ":test_remove_detach_pass",
        ":test_remove_dropout_pass",
        ":test_reduce_to_pass",
        ":test_unpack_hardswish",
        ":test_unpack_reduce_ops"
    ],
)
