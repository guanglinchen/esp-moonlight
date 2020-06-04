set(component_srcs 
    "qcloud_iot_c_sdk/sdk_src"
    "qcloud_iot_c_sdk/platform"
    )

set(include_dirs 
    "qcloud_iot_c_sdk/include"
    "qcloud_iot_c_sdk/include/exports"
	"qcloud_iot_c_sdk/sdk_src/internal_inc"
    )

idf_component_register(SRCS "${component_srcs}"
                       INCLUDE_DIRS "${include_dirs}"
                       REQUIRES mbedtls
                       )
                       