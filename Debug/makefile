################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include startup/subdir.mk
-include src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: PAJ7620U2_f446re.elf

dependents:
	-cd C:/work/workspace_stm/nucleo-f446re_stdperiph_lib/Debug && $(MAKE) clean all

# Tool invocations
PAJ7620U2_f446re.elf: $(OBJS) $(USER_OBJS) C:/work/workspace_stm/nucleo-f446re_stdperiph_lib/Debug/libnucleo-f446re_stdperiph_lib.a C:\work\workspace_stm\PAJ7620U2_f446re/LinkerScript.ld
	@echo 'Building target: $@'
	@echo 'Invoking: MCU GCC Linker'
	arm-none-eabi-gcc -mcpu=cortex-m4 -mthumb -mfloat-abi=hard -mfpu=fpv4-sp-d16 -L"C:\work\workspace_stm\nucleo-f446re_stdperiph_lib\Debug" -T"C:/work/workspace_stm/PAJ7620U2_f446re/LinkerScript.ld" -Wl,-Map=output.map -Wl,--gc-sections -o "PAJ7620U2_f446re.elf" @"objects.list" $(USER_OBJS) $(LIBS) -lm
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

post-build:
	-@echo 'Generating binary and Printing size information:'
	arm-none-eabi-objcopy -O binary "PAJ7620U2_f446re.elf" "PAJ7620U2_f446re.bin"
	arm-none-eabi-size "PAJ7620U2_f446re.elf"
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY: post-build
C:/work/workspace_stm/nucleo-f446re_stdperiph_lib/Debug/libnucleo-f446re_stdperiph_lib.a:

-include ../makefile.targets
