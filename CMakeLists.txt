include_directories(
	.
	backends
	${glfw_SOURCE_DIR}/include
	${glfw_SOURCE_DIR}/deps
	../glad/include
)

add_library(imgui STATIC
	imgui_draw.cpp
	imgui_tables.cpp
	imgui_widgets.cpp
	imgui.cpp
	backends/imgui_impl_opengl3.cpp
	backends/imgui_impl_glfw.cpp
 "imgui_spectrum.h")

 target_compile_definitions(imgui PRIVATE GLFW_INCLUDE_NONE)