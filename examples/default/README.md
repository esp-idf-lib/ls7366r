# Example for `ls7366r` driver

## Datasheet

[LS7366R](https://www.lsicsi.com/datasheets/LS7366R.pdf)

## What it does

The example configures a `ls7366r` device on a SPI bus. It creates a task to
toggle `CONFIG_EXAMPLE_PIN_NUM_TEST` pin, and configures an interrupt handler
to receive interrupts.

It reads the counter value from the device in a loop.

## Wiring

| Name | Description | Defaults |
|------|-------------|----------|
| `CONFIG_EXAMPLE_PIN_NUM_MOSI` | GPIO number for `MOSI` | "23" for `esp32`, `esp32s2`, and `esp32s3`, "5" for `esp32c2`, `esp32c3`, `esp32c5`, `esp32c6`, `esp32c61`, `esp32h2`, and `esp32p4` |
| `CONFIG_EXAMPLE_PIN_NUM_MISO` | GPIO number for `MISO` | "19" for `esp32`, `esp32s2`, and `esp32s3`, "4" for `esp32c2`, `esp32c3`, `esp32c5`, `esp32c6`, `esp32c61`, `esp32h2`, and `esp32p4` |
| `CONFIG_EXAMPLE_PIN_NUM_CLK`  | GPIO number for `CLK`  | "18" for `esp32`, `esp32s2`, and `esp32s3`, "6" for `esp32c2`, `esp32c3`, `esp32c5`, `esp32c6`, `esp32c61`, `esp32h2`, and `esp32p4` |
| `CONFIG_EXAMPLE_PIN_NUM_CS`       | GPIO number for `CS` | "5" for `esp32`, `esp32s2`, `esp32s3`, and `esp32c3`, "7" for `esp32c2`, `esp32c5`, `esp32c6`, `esp32c61`, `esp32h2`, and `esp32p4` |
| `CONFIG_EXAMPLE_PIN_NUM_TEST` | GPIO number for test pin | "25" |
| `CONFIG_EXAMPLE_PIN_NUM_INTR` | GPIO number for interrupt pin | "4" |
