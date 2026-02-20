``` rust
struct Color(u8,u8,u8);

struct ColorPalette {
	palette_data: vec<Color>
}

struct PaletteID(u32);

struct Image {
	width: u16,
	height: u16,
	image_data: vec<PaletteID>,
	palette: ColorPalette
}

impl Image {
	fn get_size(&self) {
		self.width * self.height
	}
}
```