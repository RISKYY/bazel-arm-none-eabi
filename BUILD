# BUILD

package(default_visibility = ["//visibility:public"])

config_setting(
    name = "darwin",
    constraint_values = [
        "@platforms//os:macos",
    ],
)

config_setting(
    name = "linux",
    constraint_values = [
        "@platforms//cpu:x86_64",
        "@platforms//os:linux",
    ],
)

config_setting(
    name = "linuxaarch64",
    constraint_values = [
        "@platforms//cpu:aarch64",
        "@platforms//os:linux",
    ],
)

config_setting(
    name = "windows",
    constraint_values = [
        "@platforms//cpu:x86_64",
        "@platforms//os:windows",
    ],
)

filegroup(
    name = "gcc",
    srcs = select({
        "darwin": ["@arm_none_eabi_darwin_x86_64//:bin/arm-none-eabi-gcc"],
        "linux": ["@arm_none_eabi_linux_x86_64//:bin/arm-none-eabi-gcc"],
        "linuxaarch64": ["@arm_none_eabi_linux_aarch64//:bin/arm-none-eabi-gcc"],
        "windows": ["@arm_none_eabi_windows_x86_32//:bin/arm-none-eabi-gcc.exe"],
    }),
)

filegroup(
    name = "ar",
    srcs = select({
        "darwin": ["@arm_none_eabi_darwin_x86_64//:bin/arm-none-eabi-ar"],
        "linux": ["@arm_none_eabi_linux_x86_64//:bin/arm-none-eabi-ar"],
        "linuxaarch64": ["@arm_none_eabi_linux_aarch64//:bin/arm-none-eabi-ar"],
        "windows": ["@arm_none_eabi_windows_x86_32//:bin/arm-none-eabi-ar.exe"],
    }),
)

filegroup(
    name = "ld",
    srcs = select({
        "darwin": ["@arm_none_eabi_darwin_x86_64//:bin/arm-none-eabi-ld"],
        "linux": ["@arm_none_eabi_linux_x86_64//:bin/arm-none-eabi-ld"],
        "linuxaarch64": ["@arm_none_eabi_linux_aarch64//:bin/arm-none-eabi-ld"],
        "windows": ["@arm_none_eabi_windows_x86_32//:bin/arm-none-eabi-ld.exe"],
    }),
)

filegroup(
    name = "nm",
    srcs = select({
        "darwin": ["@arm_none_eabi_darwin_x86_64//:bin/arm-none-eabi-nm"],
        "linux": ["@arm_none_eabi_linux_x86_64//:bin/arm-none-eabi-nm"],
        "linuxaarch64": ["@arm_none_eabi_linux_aarch64//:bin/arm-none-eabi-nm"],
        "windows": ["@arm_none_eabi_windows_x86_32//:bin/arm-none-eabi-nm.exe"],
    }),
)

filegroup(
    name = "objcopy",
    srcs = select({
        "darwin": ["@arm_none_eabi_darwin_x86_64//:bin/arm-none-eabi-objcopy"],
        "linux": ["@arm_none_eabi_linux_x86_64//:bin/arm-none-eabi-objcopy"],
        "linuxaarch64": ["@arm_none_eabi_linux_aarch64//:bin/arm-none-eabi-objcopy"],
        "windows": ["@arm_none_eabi_windows_x86_32//:bin/arm-none-eabi-objcopy.exe"],
    }),
)

filegroup(
    name = "objdump",
    srcs = select({
        "darwin": ["@arm_none_eabi_darwin_x86_64//:bin/arm-none-eabi-objdump"],
        "linux": ["@arm_none_eabi_linux_x86_64//:bin/arm-none-eabi-objdump"],
        "linuxaarch64": ["@arm_none_eabi_linux_aarch64//:bin/arm-none-eabi-objdump"],
        "windows": ["@arm_none_eabi_windows_x86_32//:bin/arm-none-eabi-objdump.exe"],
    }),
)

filegroup(
    name = "strip",
    srcs = select({
        "darwin": ["@arm_none_eabi_darwin_x86_64//:bin/arm-none-eabi-strip"],
        "linux": ["@arm_none_eabi_linux_x86_64//:bin/arm-none-eabi-strip"],
        "linuxaarch64": ["@arm_none_eabi_linux_aarch64//:bin/arm-none-eabi-strip"],
        "windows": ["@arm_none_eabi_windows_x86_32//:bin/arm-none-eabi-strip.exe"],
    }),
)

filegroup(
    name = "as",
    srcs = select({
        "darwin": ["@arm_none_eabi_darwin_x86_64//:bin/arm-none-eabi-as"],
        "linux": ["@arm_none_eabi_linux_x86_64//:bin/arm-none-eabi-as"],
        "linuxaarch64": ["@arm_none_eabi_linux_aarch64//:bin/arm-none-eabi-as"],
        "windows": ["@arm_none_eabi_windows_x86_32//:bin/arm-none-eabi-as.exe"],
    }),
)

filegroup(
    name = "gdb",
    srcs = select({
        "darwin": ["@arm_none_eabi_darwin_x86_64//:bin/arm-none-eabi-gdb"],
        "linux": ["@arm_none_eabi_linux_x86_64//:bin/arm-none-eabi-gdb"],
        "linuxaarch64": ["@arm_none_eabi_linux_aarch64//:bin/arm-none-eabi-gdb"],
        "windows": ["@arm_none_eabi_windows_x86_32//:bin/arm-none-eabi-gdb.exe"],
    }),
)
