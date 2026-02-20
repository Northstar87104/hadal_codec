# File Header
Codec Version: u8
Width: u16
Height: u16
Palette ID Count: u32 (written as 24 bits)

# Palette
// One field for every ID
Red: u8
Green: u8
Blue: u8

# Image Data
// 1 entry for each pixel
Palette ID: u32, trailing zeroes cut