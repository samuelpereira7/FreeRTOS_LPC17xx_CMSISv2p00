################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: Example15.axf

dependents:
	-cd C:/Users/samuelpereira/Documents/LPCXpresso_8.2.2_650/workspace_FreeRTOS/CMSISv2p00_LPC17xx/Debug && $(MAKE) clean all
	-cd C:/Users/samuelpereira/Documents/LPCXpresso_8.2.2_650/workspace_FreeRTOS/FreeRTOS_Library/Debug && $(MAKE) clean all

# Tool invocations
Example15.axf: $(OBJS) $(USER_OBJS) C:/Users/samuelpereira/Documents/LPCXpresso_8.2.2_650/workspace_FreeRTOS/CMSISv2p00_LPC17xx/Debug/libCMSISv2p00_LPC17xx.a C:/Users/samuelpereira/Documents/LPCXpresso_8.2.2_650/workspace_FreeRTOS/FreeRTOS_Library/Debug/libFreeRTOS_Library.a
	@echo 'Building target: $@'
	@echo 'Invoking: MCU Linker'
	arm-none-eabi-gcc -nostdlib -L"C:\Users\samuelpereira\Documents\LPCXpresso_8.2.2_650\workspace_FreeRTOS\FreeRTOS_Library\Debug" -L"C:\Users\samuelpereira\Documents\LPCXpresso_8.2.2_650\workspace_FreeRTOS\CMSISv2p00_LPC17xx\Debug" -Xlinker --gc-sections -Xlinker -Map=Example15.map -mcpu=cortex-m3 -mthumb -T "Example15_Debug.ld" -o "Example15.axf" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) $(EXECUTABLES)$(OBJS)$(C_DEPS) Example15.axf
	-@echo ' '

post-build:
	-@echo 'Performing post-build steps'
	-arm-none-eabi-size Example15.axf; # arm-none-eabi-objcopy -O ihex Example15.axf Example15.hex ;
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY: post-build
C:/Users/samuelpereira/Documents/LPCXpresso_8.2.2_650/workspace_FreeRTOS/CMSISv2p00_LPC17xx/Debug/libCMSISv2p00_LPC17xx.a:
C:/Users/samuelpereira/Documents/LPCXpresso_8.2.2_650/workspace_FreeRTOS/FreeRTOS_Library/Debug/libFreeRTOS_Library.a:

-include ../makefile.targets
