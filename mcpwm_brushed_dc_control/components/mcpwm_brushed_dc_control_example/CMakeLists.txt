set(COMPONENT_SRCS  "mcpwm_brushed_dc_control_example.c"
                    "cmd_mcpwm_motor.c")

idf_component_register(SRCS "${COMPONENT_SRCS}"
                    INCLUDE_DIRS "./"
                    PRIV_REQUIRES 
                     console
                     rotary_encoder
                     motor_ctrl_timer
                     pid_ctrl)
