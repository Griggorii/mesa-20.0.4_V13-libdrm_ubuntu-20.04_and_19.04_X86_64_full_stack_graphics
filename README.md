# mesa-20.0.4_V15-libdrm_ubuntu-20.04_and_19.04_X86_64_full_stack_graphics
graphics , mesa , 20.0.4 , libpng12 , support , x86_64 , gallium-pipe , OpenCL , d3d , nine , vdpau , libGLX_indirect , linux , ubuntu 20.04 , ubuntu 19.04 , EGL1.4 , not freeze game play steam wayland session , libc-2.31 , old stable video driver , самая лучшая в мире гамма и цветовая контрастность в браузерах , best color gamma in browsers

Ubuntu X64 ubuntu 19.04 disco dingo , ubuntu 20.04 focal fossa , Ubuntu 20.10 Groovy Gorilla , not test support ubuntu 18.10.19.10 , alternative driver libglu драйвер работает даже если вы его установите и поверх новой версии mesa тем самым заменив её.

sudo apt install libpciaccess0 -y  upgrade mesa do 20.0.4-2ubuntu1 install tar.xz

Mesa download + instructions: https://yadi.sk/d/efWd28SVdl1zJA Readme install

Benchmark: https://radikal.ru/video/EvoiJVc0EvC

Example install V8 video run firefox browser : https://radikal.ru/video/37hX8285dzn

Драйвер может заработать не сразу и какое то время фризы в wayland будут выполните sudo rm -rf /var/cache/apparmor/* rm -rf ~/.cache/*

Test perfomance 2D https://www.shadertoy.com/view/3lsSzf replace my fix string compile flag rerun

News + libGLESv1 , GLU , GLX , OPENGL , libGLESv2 pkgconfig + libglu library libglu.a + libxatracker.la 01.07.2020

Данный драйвер считаю лучшим по оттенкам и цветам он не теряет даже в темноте дальше у фирм идут драйверы цыфрой выше , но уже этого нету в браузере выставите флаг srgb и смотрите видео в лучшем цветовом пространстве и чёткости и не замыливании изображения. Вероятно этого человека если кто попросит https://habr.com/ru/post/440566/ может он сможет инструкции и всю эту цветность дёрнуть через гидру которые в моём драйвере , да ещё и может ускорить , но я не совсеми могу разговаривать я на взгляд перебрал много драйверов и могу только доказать что зрение у меня по лучше чем обращение со всякими регистрами драйверов потому что я не учился на это.

Test wayland video 4K and 8K https://www.youtube.com/watch?v=gYO1uk7vIcc

Внимание если вы используете мой дистрибутив гке проводником является nemo и вы обновились у вас в wayland может появиться дублирование иконок из за лиц которые тянут одеяло на себя делаем sudo -rm -rf /usr/share/gnome-shell/extensions/desktop-icons@csoriano

Если же иконки перестали появляться того же nemo значит переинсталируйте снова этот драйвер они его подменяют не заметно от пользователя по типу windows достаточно им свои ssh терминалом включить terminal=false на более медленный. На счет efi в /boot/efi/EFI/ubuntu там не должно быть лишних фаилов типа shimsshX64 всего два фаила должно быть grub.cfg и grubx64.efi


Драйвер уже фактически не тормозит в wayland видимо новый вулкан как то повлиял , а может где то что то отремонтировали и что бы не ломать структуру где была поимана эта точка то после любого обновления его наверное лучше переустанавливать именно в этой заморозке. Ранее было сильное торможение когда вкладка браузера в самом его окне не могла загрузить либо прорисовать контент иногда нельзя было переключиться на другую вкладку когда браузер был развернут полностью в размер рабочего стола в окружении wayland. Более того этот драивер работает двоекратно что усиливает качество текста и изображения как будто выставлено sRGB проверить можно запутив через терминал  nemo , nautilus либо другие программы где должно продублироваться два раза сторока вида Gtk-Message: 17:57:50.981: Failed to load module "appmenu-gtk-module" при обычном драивере эта строка не дублируется. Я пока не использовал гидру для того что бы просмотреть всю структуру и почему этот драйвер на wayland вообще идеален ещё стоит разобраться какая связь между vulkan версии 1.2.131.2 и egl1.4 что в паре получается не тормозящий работу композитор через который можно даже запустить steam и в ваших играх не будет такого дикого торможения учитывая что это wayland плюсы которого это плавность и полное отсутствие тиринга. На данный момент нету захвата видео в этом драйвере , но для тех кто может скрещивать коды есть идеяя надо посмотреть как устроен захват скриншота в коде gnome-screenshot потому что он может скринить этот композитор и сделать на основе этого библиотеку для obs-studio или green-recorder. В общем на данный момент получается с этим драйвером можно поставить убунту на телефон и он будет очень быстро работать , а запускать и гонять игры еще быстрее за счет того что размер окна мобильного телефона меньше в десятки и сотни раз , а такой драйвер работает как мне известно гораздо быстрее если экран более меньшего размера хотя там и будет у телефонов огромное разрешение.

Интересно сможет ли nvidia сделать драивер лучше пока остается в воздухе , но для работы как я понял отсюда https://github.com/NVIDIA/nvidia-docker инструменты есть , но это не к спеху я бы им посоветовал разобраться почему obs не пишет в nvenc на nvidia optimus , а потом уже лезть обгонять этот драивер который возможно быстрее и не сделаешь на wayland.

Драйвер желательно переинсталировать после каждого обновления mesa иначе можно получить торможение оболочки в wayland каждые 5-15 секунд , я пока не знаю обратили внимание на этот драйвер или просто захотят его присвоить себе никому не выдав долгожданный источник который прямо тут когда узнают что именно этого лаг тут удается почти обойти , так что как я и говорю лучше его пере инсталировать , пока это самый удачный в мире драйвер кое где в графических настройках можете выставить вертикальную синхронизацию и производительность может наоборот увеличиться , компонента драйвера гибридная по скольку тот же gles1 выключен в оригинале и какая то часть моя какая то каноникал.

Portage dump structure driver ubuntu 16.04-18.04 https://youtu.be/F5SYMzrTxjI?t=104

Brave browser profile srgb https://www.youtube.com/watch?v=I2aHs2mRtXc

________________________________________________________________________________________________________________________________________________________________

$ glxinfo
name of display: :0
display: :0  screen: 0
direct rendering: Yes
server glx vendor string: SGI
server glx version string: 1.4
server glx extensions:
    GLX_ARB_context_flush_control, GLX_ARB_create_context, 
    GLX_ARB_create_context_no_error, GLX_ARB_create_context_profile, 
    GLX_ARB_fbconfig_float, GLX_ARB_framebuffer_sRGB, GLX_ARB_multisample, 
    GLX_EXT_create_context_es2_profile, GLX_EXT_create_context_es_profile, 
    GLX_EXT_fbconfig_packed_float, GLX_EXT_framebuffer_sRGB, 
    GLX_EXT_import_context, GLX_EXT_libglvnd, GLX_EXT_no_config_context, 
    GLX_EXT_texture_from_pixmap, GLX_EXT_visual_info, GLX_EXT_visual_rating, 
    GLX_MESA_copy_sub_buffer, GLX_OML_swap_method, GLX_SGIS_multisample, 
    GLX_SGIX_fbconfig, GLX_SGIX_pbuffer, GLX_SGIX_visual_select_group, 
    GLX_SGI_make_current_read
client glx vendor string: Mesa Project and SGI
client glx version string: 1.4
client glx extensions:
    GLX_ARB_context_flush_control, GLX_ARB_create_context, 
    GLX_ARB_create_context_no_error, GLX_ARB_create_context_profile, 
    GLX_ARB_create_context_robustness, GLX_ARB_fbconfig_float, 
    GLX_ARB_framebuffer_sRGB, GLX_ARB_get_proc_address, GLX_ARB_multisample, 
    GLX_EXT_buffer_age, GLX_EXT_create_context_es2_profile, 
    GLX_EXT_create_context_es_profile, GLX_EXT_fbconfig_packed_float, 
    GLX_EXT_framebuffer_sRGB, GLX_EXT_import_context, 
    GLX_EXT_texture_from_pixmap, GLX_EXT_visual_info, GLX_EXT_visual_rating, 
    GLX_INTEL_swap_event, GLX_MESA_copy_sub_buffer, 
    GLX_MESA_multithread_makecurrent, GLX_MESA_query_renderer, 
    GLX_MESA_swap_control, GLX_OML_swap_method, GLX_OML_sync_control, 
    GLX_SGIS_multisample, GLX_SGIX_fbconfig, GLX_SGIX_pbuffer, 
    GLX_SGIX_visual_select_group, GLX_SGI_make_current_read, 
    GLX_SGI_swap_control, GLX_SGI_video_sync
GLX version: 1.4
GLX extensions:
    GLX_ARB_create_context, GLX_ARB_create_context_no_error, 
    GLX_ARB_create_context_profile, GLX_ARB_fbconfig_float, 
    GLX_ARB_framebuffer_sRGB, GLX_ARB_get_proc_address, GLX_ARB_multisample, 
    GLX_EXT_buffer_age, GLX_EXT_create_context_es2_profile, 
    GLX_EXT_create_context_es_profile, GLX_EXT_fbconfig_packed_float, 
    GLX_EXT_framebuffer_sRGB, GLX_EXT_import_context, 
    GLX_EXT_texture_from_pixmap, GLX_EXT_visual_info, GLX_EXT_visual_rating, 
    GLX_MESA_copy_sub_buffer, GLX_MESA_query_renderer, GLX_MESA_swap_control, 
    GLX_OML_swap_method, GLX_OML_sync_control, GLX_SGIS_multisample, 
    GLX_SGIX_fbconfig, GLX_SGIX_pbuffer, GLX_SGIX_visual_select_group, 
    GLX_SGI_make_current_read, GLX_SGI_video_sync
Extended renderer info (GLX_MESA_query_renderer):
    Vendor: Intel Open Source Technology Center (0x8086)
    Device: Mesa DRI Intel(R) HD Graphics 3000 (SNB GT2) (0x116)
    Version: 20.0.4
    Accelerated: yes
    Video memory: 1536MB
    Unified memory: yes
    Preferred profile: core (0x1)
    Max core profile version: 3.3
    Max compat profile version: 3.0
    Max GLES1 profile version: 1.1
    Max GLES[23] profile version: 3.0
OpenGL vendor string: Intel Open Source Technology Center
OpenGL renderer string: Mesa DRI Intel(R) HD Graphics 3000 (SNB GT2)
OpenGL core profile version string: 3.3 (Core Profile) Mesa 20.0.4-2ubuntu1
OpenGL core profile shading language version string: 3.30
OpenGL core profile context flags: (none)
OpenGL core profile profile mask: core profile
OpenGL core profile extensions:
    GL_3DFX_texture_compression_FXT1, GL_AMD_draw_buffers_blend, 
    GL_AMD_seamless_cubemap_per_texture, GL_AMD_shader_trinary_minmax, 
    GL_AMD_texture_texture4, GL_AMD_vertex_shader_layer, 
    GL_AMD_vertex_shader_viewport_index, GL_ANGLE_texture_compression_dxt3, 
    GL_ANGLE_texture_compression_dxt5, GL_APPLE_object_purgeable, 
    GL_ARB_ES2_compatibility, GL_ARB_ES3_compatibility, 
    GL_ARB_arrays_of_arrays, GL_ARB_base_instance, GL_ARB_blend_func_extended, 
    GL_ARB_buffer_storage, GL_ARB_clear_buffer_object, GL_ARB_clear_texture, 
    GL_ARB_clip_control, GL_ARB_compressed_texture_pixel_storage, 
    GL_ARB_conditional_render_inverted, GL_ARB_copy_buffer, GL_ARB_copy_image, 
    GL_ARB_cull_distance, GL_ARB_debug_output, GL_ARB_depth_buffer_float, 
    GL_ARB_depth_clamp, GL_ARB_direct_state_access, GL_ARB_draw_buffers, 
    GL_ARB_draw_buffers_blend, GL_ARB_draw_elements_base_vertex, 
    GL_ARB_draw_instanced, GL_ARB_enhanced_layouts, 
    GL_ARB_explicit_attrib_location, GL_ARB_explicit_uniform_location, 
    GL_ARB_fragment_coord_conventions, GL_ARB_fragment_layer_viewport, 
    GL_ARB_fragment_shader, GL_ARB_framebuffer_object, 
    GL_ARB_framebuffer_sRGB, GL_ARB_get_program_binary, 
    GL_ARB_get_texture_sub_image, GL_ARB_half_float_pixel, 
    GL_ARB_half_float_vertex, GL_ARB_instanced_arrays, 
    GL_ARB_internalformat_query, GL_ARB_internalformat_query2, 
    GL_ARB_invalidate_subdata, GL_ARB_map_buffer_alignment, 
    GL_ARB_map_buffer_range, GL_ARB_multi_bind, GL_ARB_occlusion_query2, 
    GL_ARB_parallel_shader_compile, GL_ARB_pipeline_statistics_query, 
    GL_ARB_pixel_buffer_object, GL_ARB_point_sprite, 
    GL_ARB_polygon_offset_clamp, GL_ARB_program_interface_query, 
    GL_ARB_provoking_vertex, GL_ARB_robustness, GL_ARB_sample_shading, 
    GL_ARB_sampler_objects, GL_ARB_seamless_cube_map, 
    GL_ARB_seamless_cubemap_per_texture, GL_ARB_separate_shader_objects, 
    GL_ARB_shader_bit_encoding, GL_ARB_shader_draw_parameters, 
    GL_ARB_shader_group_vote, GL_ARB_shader_objects, GL_ARB_shader_subroutine, 
    GL_ARB_shader_texture_lod, GL_ARB_shader_viewport_layer_array, 
    GL_ARB_shading_language_420pack, GL_ARB_shading_language_include, 
    GL_ARB_shading_language_packing, GL_ARB_sync, GL_ARB_texture_barrier, 
    GL_ARB_texture_buffer_object, GL_ARB_texture_buffer_object_rgb32, 
    GL_ARB_texture_buffer_range, GL_ARB_texture_compression_rgtc, 
    GL_ARB_texture_cube_map_array, GL_ARB_texture_filter_anisotropic, 
    GL_ARB_texture_float, GL_ARB_texture_gather, 
    GL_ARB_texture_mirror_clamp_to_edge, GL_ARB_texture_multisample, 
    GL_ARB_texture_non_power_of_two, GL_ARB_texture_query_levels, 
    GL_ARB_texture_query_lod, GL_ARB_texture_rectangle, GL_ARB_texture_rg, 
    GL_ARB_texture_rgb10_a2ui, GL_ARB_texture_storage, 
    GL_ARB_texture_storage_multisample, GL_ARB_texture_swizzle, 
    GL_ARB_timer_query, GL_ARB_transform_feedback2, 
    GL_ARB_transform_feedback_overflow_query, GL_ARB_uniform_buffer_object, 
    GL_ARB_vertex_array_bgra, GL_ARB_vertex_array_object, 
    GL_ARB_vertex_attrib_binding, GL_ARB_vertex_buffer_object, 
    GL_ARB_vertex_shader, GL_ARB_vertex_type_10f_11f_11f_rev, 
    GL_ARB_vertex_type_2_10_10_10_rev, GL_ARB_viewport_array, 
    GL_ATI_blend_equation_separate, GL_ATI_texture_float, 
    GL_EXT_EGL_image_storage, GL_EXT_EGL_sync, GL_EXT_abgr, 
    GL_EXT_blend_equation_separate, GL_EXT_demote_to_helper_invocation, 
    GL_EXT_draw_buffers2, GL_EXT_draw_instanced, GL_EXT_framebuffer_blit, 
    GL_EXT_framebuffer_multisample, GL_EXT_framebuffer_multisample_blit_scaled, 
    GL_EXT_framebuffer_object, GL_EXT_framebuffer_sRGB, 
    GL_EXT_packed_depth_stencil, GL_EXT_packed_float, 
    GL_EXT_pixel_buffer_object, GL_EXT_polygon_offset_clamp, 
    GL_EXT_provoking_vertex, GL_EXT_shader_framebuffer_fetch_non_coherent, 
    GL_EXT_shader_integer_mix, GL_EXT_texture_array, 
    GL_EXT_texture_compression_dxt1, GL_EXT_texture_compression_rgtc, 
    GL_EXT_texture_compression_s3tc, GL_EXT_texture_filter_anisotropic, 
    GL_EXT_texture_integer, GL_EXT_texture_sRGB, GL_EXT_texture_sRGB_R8, 
    GL_EXT_texture_sRGB_decode, GL_EXT_texture_shadow_lod, 
    GL_EXT_texture_shared_exponent, GL_EXT_texture_snorm, 
    GL_EXT_texture_swizzle, GL_EXT_timer_query, GL_EXT_transform_feedback, 
    GL_EXT_vertex_array_bgra, GL_IBM_multimode_draw_arrays, 
    GL_INTEL_performance_query, GL_KHR_blend_equation_advanced, 
    GL_KHR_context_flush_control, GL_KHR_debug, GL_KHR_no_error, 
    GL_KHR_parallel_shader_compile, GL_KHR_robustness, GL_MESA_pack_invert, 
    GL_MESA_shader_integer_functions, GL_MESA_texture_signed_rgba, 
    GL_NV_conditional_render, GL_NV_depth_clamp, GL_NV_packed_depth_stencil, 
    GL_NV_texture_barrier, GL_OES_EGL_image, GL_S3_s3tc

OpenGL version string: 3.0 Mesa 20.0.4-2ubuntu1
OpenGL shading language version string: 1.30
OpenGL context flags: (none)
OpenGL extensions:
    GL_3DFX_texture_compression_FXT1, GL_AMD_draw_buffers_blend, 
    GL_AMD_seamless_cubemap_per_texture, GL_AMD_shader_trinary_minmax, 
    GL_AMD_texture_texture4, GL_ANGLE_texture_compression_dxt3, 
    GL_ANGLE_texture_compression_dxt5, GL_APPLE_object_purgeable, 
    GL_APPLE_packed_pixels, GL_ARB_ES2_compatibility, 
    GL_ARB_ES3_compatibility, GL_ARB_arrays_of_arrays, 
    GL_ARB_blend_func_extended, GL_ARB_buffer_storage, 
    GL_ARB_clear_buffer_object, GL_ARB_clear_texture, GL_ARB_clip_control, 
    GL_ARB_color_buffer_float, GL_ARB_compressed_texture_pixel_storage, 
    GL_ARB_conditional_render_inverted, GL_ARB_copy_buffer, GL_ARB_copy_image, 
    GL_ARB_cull_distance, GL_ARB_debug_output, GL_ARB_depth_buffer_float, 
    GL_ARB_depth_clamp, GL_ARB_depth_texture, GL_ARB_draw_buffers, 
    GL_ARB_draw_buffers_blend, GL_ARB_draw_elements_base_vertex, 
    GL_ARB_draw_instanced, GL_ARB_explicit_attrib_location, 
    GL_ARB_explicit_uniform_location, GL_ARB_fragment_coord_conventions, 
    GL_ARB_fragment_layer_viewport, GL_ARB_fragment_program, 
    GL_ARB_fragment_program_shadow, GL_ARB_fragment_shader, 
    GL_ARB_framebuffer_object, GL_ARB_framebuffer_sRGB, 
    GL_ARB_get_program_binary, GL_ARB_get_texture_sub_image, 
    GL_ARB_half_float_pixel, GL_ARB_half_float_vertex, 
    GL_ARB_instanced_arrays, GL_ARB_internalformat_query, 
    GL_ARB_internalformat_query2, GL_ARB_invalidate_subdata, 
    GL_ARB_map_buffer_alignment, GL_ARB_map_buffer_range, GL_ARB_multi_bind, 
    GL_ARB_multisample, GL_ARB_multitexture, GL_ARB_occlusion_query, 
    GL_ARB_occlusion_query2, GL_ARB_parallel_shader_compile, 
    GL_ARB_pipeline_statistics_query, GL_ARB_pixel_buffer_object, 
    GL_ARB_point_parameters, GL_ARB_point_sprite, GL_ARB_polygon_offset_clamp, 
    GL_ARB_program_interface_query, GL_ARB_provoking_vertex, 
    GL_ARB_robustness, GL_ARB_sample_shading, GL_ARB_sampler_objects, 
    GL_ARB_seamless_cube_map, GL_ARB_seamless_cubemap_per_texture, 
    GL_ARB_separate_shader_objects, GL_ARB_shader_bit_encoding, 
    GL_ARB_shader_draw_parameters, GL_ARB_shader_group_vote, 
    GL_ARB_shader_objects, GL_ARB_shader_texture_lod, 
    GL_ARB_shading_language_100, GL_ARB_shading_language_420pack, 
    GL_ARB_shading_language_include, GL_ARB_shading_language_packing, 
    GL_ARB_shadow, GL_ARB_sync, GL_ARB_texture_barrier, 
    GL_ARB_texture_border_clamp, GL_ARB_texture_compression, 
    GL_ARB_texture_compression_rgtc, GL_ARB_texture_cube_map, 
    GL_ARB_texture_cube_map_array, GL_ARB_texture_env_add, 
    GL_ARB_texture_env_combine, GL_ARB_texture_env_crossbar, 
    GL_ARB_texture_env_dot3, GL_ARB_texture_filter_anisotropic, 
    GL_ARB_texture_float, GL_ARB_texture_gather, 
    GL_ARB_texture_mirror_clamp_to_edge, GL_ARB_texture_mirrored_repeat, 
    GL_ARB_texture_multisample, GL_ARB_texture_non_power_of_two, 
    GL_ARB_texture_query_levels, GL_ARB_texture_query_lod, 
    GL_ARB_texture_rectangle, GL_ARB_texture_rg, GL_ARB_texture_rgb10_a2ui, 
    GL_ARB_texture_storage, GL_ARB_texture_storage_multisample, 
    GL_ARB_texture_swizzle, GL_ARB_timer_query, GL_ARB_transform_feedback2, 
    GL_ARB_transform_feedback_overflow_query, GL_ARB_transpose_matrix, 
    GL_ARB_uniform_buffer_object, GL_ARB_vertex_array_bgra, 
    GL_ARB_vertex_array_object, GL_ARB_vertex_attrib_binding, 
    GL_ARB_vertex_buffer_object, GL_ARB_vertex_program, GL_ARB_vertex_shader, 
    GL_ARB_vertex_type_10f_11f_11f_rev, GL_ARB_vertex_type_2_10_10_10_rev, 
    GL_ARB_window_pos, GL_ATI_blend_equation_separate, GL_ATI_draw_buffers, 
    GL_ATI_separate_stencil, GL_ATI_texture_env_combine3, 
    GL_ATI_texture_float, GL_EXT_EGL_image_storage, GL_EXT_EGL_sync, 
    GL_EXT_abgr, GL_EXT_bgra, GL_EXT_blend_color, 
    GL_EXT_blend_equation_separate, GL_EXT_blend_func_separate, 
    GL_EXT_blend_minmax, GL_EXT_blend_subtract, GL_EXT_compiled_vertex_array, 
    GL_EXT_copy_texture, GL_EXT_demote_to_helper_invocation, 
    GL_EXT_direct_state_access, GL_EXT_draw_buffers2, GL_EXT_draw_instanced, 
    GL_EXT_draw_range_elements, GL_EXT_fog_coord, GL_EXT_framebuffer_blit, 
    GL_EXT_framebuffer_multisample, GL_EXT_framebuffer_multisample_blit_scaled, 
    GL_EXT_framebuffer_object, GL_EXT_framebuffer_sRGB, 
    GL_EXT_gpu_program_parameters, GL_EXT_gpu_shader4, 
    GL_EXT_multi_draw_arrays, GL_EXT_packed_depth_stencil, 
    GL_EXT_packed_float, GL_EXT_packed_pixels, GL_EXT_pixel_buffer_object, 
    GL_EXT_point_parameters, GL_EXT_polygon_offset_clamp, 
    GL_EXT_provoking_vertex, GL_EXT_rescale_normal, GL_EXT_secondary_color, 
    GL_EXT_separate_specular_color, 
    GL_EXT_shader_framebuffer_fetch_non_coherent, GL_EXT_shader_integer_mix, 
    GL_EXT_shadow_funcs, GL_EXT_stencil_two_side, GL_EXT_stencil_wrap, 
    GL_EXT_subtexture, GL_EXT_texture, GL_EXT_texture3D, 
    GL_EXT_texture_array, GL_EXT_texture_compression_dxt1, 
    GL_EXT_texture_compression_rgtc, GL_EXT_texture_compression_s3tc, 
    GL_EXT_texture_cube_map, GL_EXT_texture_edge_clamp, 
    GL_EXT_texture_env_add, GL_EXT_texture_env_combine, 
    GL_EXT_texture_env_dot3, GL_EXT_texture_filter_anisotropic, 
    GL_EXT_texture_integer, GL_EXT_texture_lod_bias, GL_EXT_texture_object, 
    GL_EXT_texture_rectangle, GL_EXT_texture_sRGB, GL_EXT_texture_sRGB_R8, 
    GL_EXT_texture_sRGB_decode, GL_EXT_texture_shadow_lod, 
    GL_EXT_texture_shared_exponent, GL_EXT_texture_snorm, 
    GL_EXT_texture_swizzle, GL_EXT_timer_query, GL_EXT_transform_feedback, 
    GL_EXT_vertex_array, GL_EXT_vertex_array_bgra, 
    GL_IBM_multimode_draw_arrays, GL_IBM_rasterpos_clip, 
    GL_IBM_texture_mirrored_repeat, GL_INGR_blend_func_separate, 
    GL_INTEL_performance_query, GL_KHR_blend_equation_advanced, 
    GL_KHR_context_flush_control, GL_KHR_debug, GL_KHR_no_error, 
    GL_KHR_parallel_shader_compile, GL_KHR_robustness, GL_MESA_pack_invert, 
    GL_MESA_shader_integer_functions, GL_MESA_texture_signed_rgba, 
    GL_MESA_window_pos, GL_NV_blend_square, GL_NV_conditional_render, 
    GL_NV_depth_clamp, GL_NV_fog_distance, GL_NV_light_max_exponent, 
    GL_NV_packed_depth_stencil, GL_NV_primitive_restart, 
    GL_NV_texgen_reflection, GL_NV_texture_barrier, 
    GL_NV_texture_env_combine4, GL_NV_texture_rectangle, GL_OES_EGL_image, 
    GL_OES_read_format, GL_S3_s3tc, GL_SGIS_generate_mipmap, 
    GL_SGIS_texture_border_clamp, GL_SGIS_texture_edge_clamp, 
    GL_SGIS_texture_lod, GL_SUN_multi_draw_arrays

OpenGL ES profile version string: OpenGL ES 3.0 Mesa 20.0.4-2ubuntu1
OpenGL ES profile shading language version string: OpenGL ES GLSL ES 3.00
OpenGL ES profile extensions:
    GL_ANGLE_texture_compression_dxt3, GL_ANGLE_texture_compression_dxt5, 
    GL_APPLE_texture_max_level, GL_EXT_EGL_image_storage, 
    GL_EXT_base_instance, GL_EXT_blend_func_extended, GL_EXT_blend_minmax, 
    GL_EXT_clip_control, GL_EXT_clip_cull_distance, GL_EXT_color_buffer_float, 
    GL_EXT_compressed_ETC1_RGB8_sub_texture, 
    GL_EXT_demote_to_helper_invocation, GL_EXT_depth_clamp, 
    GL_EXT_discard_framebuffer, GL_EXT_disjoint_timer_query, 
    GL_EXT_draw_buffers, GL_EXT_draw_buffers_indexed, 
    GL_EXT_draw_elements_base_vertex, GL_EXT_float_blend, GL_EXT_frag_depth, 
    GL_EXT_map_buffer_range, GL_EXT_multi_draw_arrays, 
    GL_EXT_occlusion_query_boolean, GL_EXT_polygon_offset_clamp, 
    GL_EXT_read_format_bgra, GL_EXT_robustness, GL_EXT_sRGB_write_control, 
    GL_EXT_separate_shader_objects, 
    GL_EXT_shader_framebuffer_fetch_non_coherent, GL_EXT_shader_integer_mix, 
    GL_EXT_texture_border_clamp, GL_EXT_texture_compression_dxt1, 
    GL_EXT_texture_compression_rgtc, GL_EXT_texture_compression_s3tc, 
    GL_EXT_texture_compression_s3tc_srgb, GL_EXT_texture_filter_anisotropic, 
    GL_EXT_texture_format_BGRA8888, GL_EXT_texture_query_lod, 
    GL_EXT_texture_rg, GL_EXT_texture_sRGB_R8, GL_EXT_texture_sRGB_decode, 
    GL_EXT_texture_shadow_lod, GL_EXT_texture_type_2_10_10_10_REV, 
    GL_EXT_unpack_subimage, GL_INTEL_performance_query, 
    GL_KHR_blend_equation_advanced, GL_KHR_context_flush_control, 
    GL_KHR_debug, GL_KHR_no_error, GL_KHR_parallel_shader_compile, 
    GL_KHR_robustness, GL_MESA_framebuffer_flip_y, 
    GL_MESA_shader_integer_functions, GL_NV_conditional_render, 
    GL_NV_draw_buffers, GL_NV_fbo_color_attachments, GL_NV_read_buffer, 
    GL_NV_read_depth, GL_NV_read_depth_stencil, GL_NV_read_stencil, 
    GL_OES_EGL_image, GL_OES_EGL_image_external, 
    GL_OES_EGL_image_external_essl3, GL_OES_EGL_sync, 
    GL_OES_compressed_ETC1_RGB8_texture, GL_OES_depth24, GL_OES_depth_texture, 
    GL_OES_depth_texture_cube_map, GL_OES_draw_buffers_indexed, 
    GL_OES_draw_elements_base_vertex, GL_OES_element_index_uint, 
    GL_OES_fbo_render_mipmap, GL_OES_get_program_binary, GL_OES_mapbuffer, 
    GL_OES_packed_depth_stencil, GL_OES_required_internalformat, 
    GL_OES_rgb8_rgba8, GL_OES_sample_shading, GL_OES_sample_variables, 
    GL_OES_shader_multisample_interpolation, GL_OES_standard_derivatives, 
    GL_OES_stencil8, GL_OES_surfaceless_context, GL_OES_texture_3D, 
    GL_OES_texture_border_clamp, GL_OES_texture_float, 
    GL_OES_texture_float_linear, GL_OES_texture_half_float, 
    GL_OES_texture_half_float_linear, GL_OES_texture_npot, 
    GL_OES_vertex_array_object, GL_OES_vertex_half_float

76 GLX Visuals
    visual  x   bf lv rg d st  colorbuffer  sr ax dp st accumbuffer  ms  cav
  id dep cl sp  sz l  ci b ro  r  g  b  a F gb bf th cl  r  g  b  a ns b eat
----------------------------------------------------------------------------
0x024 24 tc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x025 24 dc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x290 24 tc  0  32  0 r  . .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x292 24 tc  0  32  0 r  y .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x294 24 tc  0  32  0 r  y .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x2a2 24 tc  0  32  0 r  . .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x2a4 24 tc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8 16 16 16 16  0 0 Slow
0x2a5 24 tc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x2a6 24 tc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8 16 16 16 16  0 0 Slow
0x2ad 24 tc  0  24  0 r  . .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x2af 24 tc  0  24  0 r  y .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x2b1 24 tc  0  24  0 r  y .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x2bf 24 tc  0  24  0 r  . .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x2c1 24 tc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x2c2 24 tc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8 16 16 16  0  0 0 Slow
0x2c3 24 tc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x2c4 24 tc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8 16 16 16  0  0 0 Slow
0x2cb 24 tc  0  32  0 r  . .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x2cd 24 tc  0  32  0 r  y .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x2cf 24 tc  0  32  0 r  y .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x2dd 24 tc  0  32  0 r  . .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x2df 24 tc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x2e0 24 tc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8 16 16 16 16  0 0 Slow
0x2e1 24 tc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x2e2 24 tc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8 16 16 16 16  0 0 Slow
0x2e9 24 tc  0  24  0 r  . .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x2eb 24 tc  0  24  0 r  y .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x2ed 24 tc  0  24  0 r  y .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x2fb 24 tc  0  24  0 r  . .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x2fd 24 tc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x2fe 24 tc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8 16 16 16  0  0 0 Slow
0x2ff 24 tc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x300 24 tc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8 16 16 16  0  0 0 Slow
0x307 24 dc  0  32  0 r  . .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x309 24 dc  0  32  0 r  y .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x30b 24 dc  0  32  0 r  y .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x319 24 dc  0  32  0 r  . .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x31b 24 dc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8 16 16 16 16  0 0 Slow
0x31c 24 dc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x31d 24 dc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8 16 16 16 16  0 0 Slow
0x324 24 dc  0  24  0 r  . .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x326 24 dc  0  24  0 r  y .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x328 24 dc  0  24  0 r  y .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x336 24 dc  0  24  0 r  . .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x338 24 dc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x339 24 dc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8 16 16 16  0  0 0 Slow
0x33a 24 dc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x33b 24 dc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8 16 16 16  0  0 0 Slow
0x342 24 dc  0  32  0 r  . .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x344 24 dc  0  32  0 r  y .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x346 24 dc  0  32  0 r  y .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x354 24 dc  0  32  0 r  . .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x356 24 dc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x357 24 dc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8 16 16 16 16  0 0 Slow
0x358 24 dc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x359 24 dc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8 16 16 16 16  0 0 Slow
0x360 24 dc  0  24  0 r  . .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x362 24 dc  0  24  0 r  y .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x364 24 dc  0  24  0 r  y .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x372 24 dc  0  24  0 r  . .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x374 24 dc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x375 24 dc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8 16 16 16  0  0 0 Slow
0x376 24 dc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x377 24 dc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8 16 16 16  0  0 0 Slow
0x055 32 tc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x37e 32 tc  0  32  0 r  . .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x37f 32 tc  0  32  0 r  y .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x380 32 tc  0  32  0 r  y .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x387 32 tc  0  32  0 r  . .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x388 32 tc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x38c 32 tc  0  32  0 r  . .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x38d 32 tc  0  32  0 r  y .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x38e 32 tc  0  32  0 r  y .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x395 32 tc  0  32  0 r  . .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x396 32 tc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x397 32 tc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None

58 GLXFBConfigs:
    visual  x   bf lv rg d st  colorbuffer  sr ax dp st accumbuffer  ms  cav
  id dep cl sp  sz l  ci b ro  r  g  b  a F gb bf th cl  r  g  b  a ns b eat
----------------------------------------------------------------------------
0x0ce 24 tc  0  32  0 r  . .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x0d0 24 tc  0  32  0 r  y .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x0e0 24 tc  0  32  0 r  . .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x0e2 24 tc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x0e3 24 tc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8 16 16 16 16  0 0 Slow
0x0ec 24 tc  0  24  0 r  . .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x0ee 24 tc  0  24  0 r  y .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x0fe 24 tc  0  24  0 r  . .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x100 24 tc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x101 24 tc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8 16 16 16  0  0 0 Slow
0x10a 24 tc  0  32  0 r  . .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x10c 24 tc  0  32  0 r  y .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x11c 24 tc  0  32  0 r  . .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x11e 24 tc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x11f 24 tc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8 16 16 16 16  0 0 Slow
0x128 24 tc  0  24  0 r  . .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x12a 24 tc  0  24  0 r  y .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x13a 24 tc  0  24  0 r  . .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x13c 24 tc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x13d 24 tc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8 16 16 16  0  0 0 Slow
0x146  0 tc  0  16  0 r  . .   5  6  5  0 .  .  0  0  0  0  0  0  0  0 0 None
0x148  0 tc  0  16  0 r  y .   5  6  5  0 .  .  0  0  0  0  0  0  0  0 0 None
0x158  0 tc  0  16  0 r  . .   5  6  5  0 .  .  0 24  8  0  0  0  0  0 0 None
0x15a  0 tc  0  16  0 r  y .   5  6  5  0 .  .  0 24  8  0  0  0  0  0 0 None
0x15b  0 tc  0  16  0 r  y .   5  6  5  0 .  .  0 24  8 16 16 16  0  0 0 Slow
0x1dc 24 dc  0  32  0 r  . .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x1de 24 dc  0  32  0 r  y .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x1ee 24 dc  0  32  0 r  . .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x1f0 24 dc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x1f1 24 dc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8 16 16 16 16  0 0 Slow
0x1fa 24 dc  0  24  0 r  . .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x1fc 24 dc  0  24  0 r  y .   8  8  8  0 .  .  0  0  0  0  0  0  0  0 0 None
0x20c 24 dc  0  24  0 r  . .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x20e 24 dc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8  0  0  0  0  0 0 None
0x20f 24 dc  0  24  0 r  y .   8  8  8  0 .  .  0 24  8 16 16 16  0  0 0 Slow
0x218 24 dc  0  32  0 r  . .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x21a 24 dc  0  32  0 r  y .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x22a 24 dc  0  32  0 r  . .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x22c 24 dc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x22d 24 dc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8 16 16 16 16  0 0 Slow
0x236 24 dc  0  24  0 r  . .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x238 24 dc  0  24  0 r  y .   8  8  8  0 .  s  0  0  0  0  0  0  0  0 0 None
0x248 24 dc  0  24  0 r  . .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x24a 24 dc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8  0  0  0  0  0 0 None
0x24b 24 dc  0  24  0 r  y .   8  8  8  0 .  s  0 24  8 16 16 16  0  0 0 Slow
0x254  0 dc  0  16  0 r  . .   5  6  5  0 .  .  0  0  0  0  0  0  0  0 0 None
0x256  0 dc  0  16  0 r  y .   5  6  5  0 .  .  0  0  0  0  0  0  0  0 0 None
0x266  0 dc  0  16  0 r  . .   5  6  5  0 .  .  0 24  8  0  0  0  0  0 0 None
0x268  0 dc  0  16  0 r  y .   5  6  5  0 .  .  0 24  8  0  0  0  0  0 0 None
0x269  0 dc  0  16  0 r  y .   5  6  5  0 .  .  0 24  8 16 16 16  0  0 0 Slow
0x272 32 tc  0  32  0 r  . .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x273 32 tc  0  32  0 r  y .   8  8  8  8 .  .  0  0  0  0  0  0  0  0 0 None
0x27b 32 tc  0  32  0 r  . .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x27c 32 tc  0  32  0 r  y .   8  8  8  8 .  .  0 24  8  0  0  0  0  0 0 None
0x281 32 tc  0  32  0 r  . .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x282 32 tc  0  32  0 r  y .   8  8  8  8 .  s  0  0  0  0  0  0  0  0 0 None
0x28a 32 tc  0  32  0 r  . .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None
0x28b 32 tc  0  32  0 r  y .   8  8  8  8 .  s  0 24  8  0  0  0  0  0 0 None

