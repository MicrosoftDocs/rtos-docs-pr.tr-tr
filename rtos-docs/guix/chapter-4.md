---
title: Bölüm 4-Gux hizmetlerinin açıklaması
description: Bu bölüm, tüm GUıDX hizmetlerinin (aşağıda listelenmiştir) alfabetik sırada bir açıklamasını içerir.
author: philmea
ms.author: philmea
ms.date: 05/19/2020
ms.topic: article
ms.service: rtos
ms.openlocfilehash: 7a17ab0d2500d021bb9397dbf673427362c45173
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104826452"
---
# <a name="chapter-4---description-of-guix-services"></a>Bölüm 4-Gux hizmetlerinin açıklaması

Bu bölüm, tüm GUıDX hizmetlerinin (aşağıda listelenmiştir) alfabetik sırada bir açıklamasını içerir.  

Aşağıdaki API açıklamalarındaki "dönüş değerleri" bölümünde, **kalın** olmayan değerler, API hata denetimini devre dışı bırakmak için kullanılan **GX_DISABLE_ERROR_CHECKING** tanımlanmasından etkilenmez, ancak kalın olmayan değerler tamamen devre dışı bırakılır. 

| **GUX hizmeti**                      | **Açıklama**                                                                             |
| -------------------------------------- | -------------------------------------------------------------------------------------------- |
| gx_accordion_menu_create            | Accordion menüsü oluşturma                                                                        |
| gx_accordion_menu_draw              | Accordion menüsünü çiz                                                                          |
| gx_accordion_menu_event_process    | İşlem Accordion Menü olayı                                                                 |
| gx_accordion_menu_position          | Menü öğelerini Konumlandır                                                                          |
| gx_animation_canvas_define          | Sonraki animasyonlar için kullanılacak bir tuval için animasyon denetleyicisine bellek sağlayın. |
| gx_animation_create                  | Animasyon denetleyicisi oluşturma                                                               |
| gx_animation_delete                  | Animasyon denetleyicisini silme                                                               |
| gx_animation_drag_disable           | Ekran Sürükle animasyon kancasını devre dışı bırak                                                           |
| gx_animation_drag_enable            | Ekran Sürükle animasyon kancasını etkinleştir                                                            |
| gx_animation_landing_speed_set     | Ekran sürükleme animasyonu için giriş hızını ayarla                                                  |
| gx_animation_start                   | Animasyon sırası başlatma                                                               |
| gx_animation_stop                    | Animasyon sırasını askıya alma                                                                |
| gx_binres_language_count_get      |  Bir ikili kaynak dosyasından dil sayısını Al                                          |
| gx_binres_language_info_load      |  İkili kaynak dosyasından dil adı ve boyut bilgilerini okuyun.                           |
| gx_binres_language_table_load      | kullanım dışı İkili kaynak veri arabelleğinden bir dil tablosu yükleme                          |
| gx_binres_language_table_load_ext | İkili kaynak veri arabelleğinden bir dil tablosu yükleme                                       |
| gx_binres_theme_load                | İkili kaynak veri arabelleğinden tema yükleme                                                |
| gx_brush_default                     | Geçerli fırçayı varsayılanlara Başlat                                                         |
| gx_brush_define                      | Fırça Tanımla                                                                                 |
| gx_button_background_draw           | Düğme arka planı çiz                                                                       |
| gx_button_create                     | Oluştur düğmesi                                                                                |
| gx_button_deselect                   | Seçimi Kaldır düğmesi                                                                              |
| gx_button_draw                       | Çiz düğmesi                                                                                  |
| gx_button_event_process            | İşlem düğmesi olayı                              |
| gx_button_select                    | Düğme Seç                                     |
| gx_canvas_alpha_set                | Tuval için alfa Blend değeri ayarlama                  |
| gx_canvas_arc_draw                 | Daire yay çiz                                   |
| gx_canvas_block_move               | Blok taşı                                        |
| gx_canvas_circle_draw              | Daire çiz                                       |
| gx_canvas_create                    | Tuval oluşturma                                   |
| gx_canvas_delete                    | Tuvali silme                                   |
| gx_canvas_drawing_complete         | Tuval çizimini tamamen doldurun                           |
| gx_canvas_drawing_initiate         | Tuvalde çizim Başlat                        |
| gx_canvas_ellipse_draw             | Elips çizme                                   |
| gx_canvas_hardware_layer_bind     | Tuvali grafik katmanına bağlama                     |
| gx_canvas_hide                      | Tuvali görünmez yapma                           |
| gx_canvas_line_draw                | Çizgi çiz                                         |
| gx_canvas_memory_define            | Tuval bellek adresi ata                      |
| gx_canvas_offset_set               | Tuval x, y görüntüleme boşluğu ata                  |
| gx_canvas_pie_draw                 | Pasta (kama) şekli çiz                          |
| gx_canvas_pixel_draw               | Tek bir piksel çiz                               |
| gx_canvas_pixelmap_blend           | Bir pixelmap ile arka plan Blend                  |
| gx_canvas_pixelmap_get             | Tuval verilerine işaret eden bir pixelmap al            |
| gx_canvas_pixelmap_draw            | Pixelmap çiz                                     |
| gx_canvas_pixelmap_rotate          | Pixelmap 'i döndür                                   |
| gx_canvas_pixelmap_tile            | Kutucuk pixelmap                                     |
| gx_canvas_polygon_draw             | Çokgen Çiz                                      |
| gx_canvas_rectangle_draw           | Dikdörtgen çiz                                    |
| gx_canvas_rotated_text_draw       | kullanım dışı Orta nokta ile döndürülen metin çiz |
| gx_canvas_rotated_text_draw_ext  | Orta nokta ile döndürülen metin çiz              |
| gx_canvas_shift                     | X, y için tuval kaydır                               |
| gx_canvas_show                      | Tuvali görünür yapma                             |
| gx_canvas_text_draw                | kullanım dışı Metin çiz                            |
| gx_canvas_text_draw_ext           | Metin çiz                                         |
| gx_checkbox_create                  | Onay kutusu oluşturma                                 |
| gx_checkbox_draw                    | Onay kutusu çiz                                   |
| gx_checkbox_event_process          | CheckBox olay işlem işlevi                   |
| gx_checkbox_pixelmap_set           | Onay kutusu pixelmap ata                          |
| gx_checkbox_select                  | Onay kutusunu seçin                                   |
| gx_circular_gauge_angle_get       | Ölçer pencere öğesi iğne açısını al                |
| gx_circular_gauge_angle_set       | Ölçer atama pencere öğesi iğne açısı                  |
| gx_circular_gauge_animation_set   | Dairesel ölçer animasyonunu tanımla                   |
| gx_circular_gauge_background_draw | Dairesel ölçer arka planı çiz                    |
| gx_circular_gauge_create           | Dairesel ölçer pencere öğesi oluştur                    |
| gx_circular_gauge_draw             | Dairesel ölçer pencere öğesi çiz                      |
| gx_circular_gauge_event_process   | Döngüsel ölçer olayını işle                      |
| gx_context_brush_default            | Geçerli bağlam fırçasını ayarla                                      |
| gx_context_brush_define             | Geçerli bağlamın fırçayı tanımlayın                                       |
| gx_context_brush_get                | Geçerli bağlamın fırçasını al                                          |
| gx_context_brush_pattern_set       | Geçerli bağlam fırçasının şeklini ayarla                           |
| gx_context_brush_set                | Geçerli bağlam fırçası ayarla                                          |
| gx_context_brush_style_set         | Geçerli bağlamın Fırça stilini ayarla                                    |
| gx_context_brush_width_set         | Geçerli bağlam 'in fırça genişliğini ayarla                                     |
| gx_context_color_get                | Renk KIMLIĞINI renk değerine çözümle                                     |
| gx_context_fill_color_set          | Geçerli bağlamın Fill rengini ayarla                                     |
| gx_context_font_get                 | Yazı tipi KIMLIĞINI yazı tipi işaretçisi değerine çözümle                               |
| gx_context_font_set                 | Geçerli bağlamın yazı tipini ayarla                                           |
| gx_context_line_color_set          | Geçerli bağlamın çizgi rengini ayarla                                     |
| gx_context_pixelmap_get             | Bir pixelmap KIMLIĞINI pixelmap işaretçisi değerine çözümle                       |
| gx_context_pixelmap_set             | Alan dolguları için kullanılan fırça pixelmap atama                            |
| gx_context_raw_brush_define        | Geçerli bağlamın ham fırçasını tanımlayın                                   |
| gx_context_raw_fill_color_set     | Geçerli bağlamın ham dolgusu rengini ayarla                                 |
| gx_context_raw_line_color_set     | Geçerli bağlamın ham çizgi rengini ayarla                                 |
| gx_context_string_get               | Geçerli çizim bağlamıyla ilişkili dizeyi al (kullanım dışı). |
| gx_context_string_get_ext          | Geçerli çizim bağlamıyla ilişkili dizeyi al (kullanım dışı). |
| gx_display_active_language_set     | Etkin dil ata                                                |
| gx_display_color_set                | Görüntüleme rengi tablosundaki bir renk değerini değiştirin.                       |
| gx_display_color_table_set         | Bir görüntü tarafından kullanılan renk tablosunu atama                              |
| gx_display_create                    | Görüntü oluştur                                                        |
| gx_display_delete                    | Görünümü Sil                                                        |
| gx_display_font_table_set          | Bir görüntü tarafından kullanılan yazı tipi tablosunu atama                               |
| gx_display_language_table_get      | Bir görüntüleme ile ilişkili dil tablosunu alma (kullanım dışı)    |
| gx_display_language_table_get_ext | Bir ekran ile ilişkili dil tablosunu alma                 |
| gx_display_language_table_set      | Dil tablosunu belirtilen görüntüleme (kullanım dışı) olarak ata           |
| gx_display_language_table_set_ext | Belirtilen görüntüleme için dil tablosunu atayın.                       |
| gx_display_pixelmap_table_set      | Bir görüntü tarafından kullanılan pixelmap tablosunu atama                           |
| gx_display_string_get               | Dize KIMLIĞIYLE ilişkili dizeyi al (kullanım dışı)                |
| gx_display_string_get_ext          | Dize KIMLIĞIYLE ilişkili dizeyi al                             |
| gx_display_string_table_get             | Belirtilen görüntüleme (kullanım dışı) ile ilişkili dize tablosunu alın. |
| gx_display_string_table_get_ext        | Belirtilen görüntü ile ilişkili dize tablosunu al               |
| gx_display_theme_install                 | Temaları belirtilen görüntüsüne yükler                               |
| gx_drop_list_close                       | Bırakma listesini kapat                                                       |
| gx_drop_list_create                      | Bırakma listesi oluştur                                                      |
| gx_drop_list_event_process               | Liste olayı işlemeyi bırak                                            |
| gx_drop_list_open                        | Bırakma listesini aç                                                        |
| gx_drop_list_pixelmap_set               | Pixelmap 'i bırakma listesine ayarla                                             |
| gx_drop_list_popup_set                  | Açılan listeyi bırakma listesine ayarla                                                |
| gx_horizontal_list_children_position    | Alt öğeleri yatay listede Konumlandır                          |
| gx_horizontal_list_create                | Yatay liste oluştur                                                |
| gx_horizontal_list_event_process        | Olayı yatay listede işle                                      |
| gx_horizontal_list_page_index_set      | Yatay liste sayfası dizinini ata                                     |
| gx_horizontal_list_selected_index_get  | Seçili öğe dizinini al                                           |
| gx_horizontal_list_selected_widget_get | Seçili öğe pencere öğesini al                                          |
| gx_horizontal_list_selected_set         | Seçili öğeyi ayarla                                                 |
| gx_horizontal_list_total_columns_set   | Oluşturulduktan sonra liste sütunlarının sayısını değiştirme                          |
| gx_horizontal_scrollbar_create           | Yatay kaydırma çubuğu oluştur                                           |
| gx_icon_button_create                    | Simge Oluştur düğmesi                                                    |
| gx_icon_button_draw                      | Bir simge düğmesi çiz                                                   |
| gx_icon_button_pixelmap_set             | Simge düğmesinde pixelmap ayarla                                           |
| gx_icon_background_draw                  | Çizim simgesi arka planı                                                  |
| gx_icon_create                            | Oluştur simgesi                                                           |
| gx_icon_draw                              | Çizim simgesi                                                             |
| gx_icon_event_process                    | Simge olay işleme işlevi                                        |
| gx_icon_pixelmap_set                     | Simgeye yönelik pixelmap ayarla                                                 |
| gx_image_reader_create                   | Görüntü okuyucu modülü örneği oluştur                                   |
| gx_image_reader_palette_set             | Görüntü okuyucu paleti tanımlama                                           |
| gx_image_reader_start                    | Sıkıştırılmış ve dönüştürme işlemini Başlat                           |
| gx_line_chart_axis_draw                 | Çizgi grafiği x, y ekseni çiz                                              |
| gx_line_chart_create                     | GX_LINE_CHART örneği oluştur                                       |
| gx_line_chart_data_draw                 | Çizgi grafik veri satırı çiz                                             |
| gx_line_chart_draw                       | Varsayılan çizgi grafik çizimi                                            |
| gx_line_chart_update                     | Çizgi grafik verilerinin güncelleştirilmesini zorla                                       |
| gx_line_chart_y_scale_calculate        | Y ekseni veri değerlerinin ölçeğini piksel koordinatlarına göre hesaplayın.           |
| gx_menu_create                            | Menü Oluştur                                                           |
| gx_menu_draw                              | Çiz Menüsü                                                             |
| gx_menu_event_process                     | İşlem menüsü olayı                                                    |
| gx_menu_insert                                | Yeni öğe Ekle                                                               |
| gx_menu_remove                                | Bir öğeyi kaldır                                                                  |
| gx_menu_text_draw                            | Çiz menü metni                                                                  |
| gx_menu_text_offset_set                     | Menü metni çiz kaydırmayı ayarla                                                       |
| gx_multi_line_text_button_create           | Çok satırlı metin düğmesi oluştur                                                   |
| gx_multi_line_text_button_draw             | Çok satırlı metin düğmesi çiz                                                     |
| gx_multi_line_text_button_event_process   | Çok satırlı metin düğmesi için yazı tipi ayarla                                             |
| gx_multi_line_text_button_text_draw       | Çizimin metin çizim kısmı                                                 |
| gx_multi_line_text_button_text_id_set    | Sistem dizesini metin düğmesine ayarla düğmesi                                                |
| gx_multi_line_text_button_text_set        | Metin düğmesine Kullanıcı tanımlı dize ata (kullanım dışı)                          |
| gx_multi_line_text_button_text_set_ext   | Metin düğmesine Kullanıcı tanımlı dize ata düğmesi                                       |
| gx_multi_line_text_input_backspace         | Çok satırlı metin girişi imleç konumundan önce karakteri sil               |
| gx_multi_line_text_input_buffer_get       | Metin girişi pencere öğesinin arabellek bilgilerini alır                               |
| gx_multi_line_text_input_buffer_clear     | Metin girişi arabelleğindeki tüm karakterleri siler                               |
| gx_multi_line_text_input_char_insert      | Çok satırlı metin girişi imleç konumuna UTF8 biçimli dize Ekle (kullanım dışı) |
| gx_multi_line_text_input_char_insert_ext | Çok satırlı metin girişi imleç konumuna UTF8 biçimli dize Ekle              |
| gx_multi_line_text_input_create            | Çok satırlı metin girişi oluştur                                                    |
| gx_multi_line_text_input_cursor_pos_get  | Çok satırlı metin girişi imleç konumunu al                                  |
| gx_multi_line_text_input_delete            | Çok satırlı metin girişi imleç konumundan sonra karakteri sil                 |
| gx_multi_line_text_input_down_arrow       | Çok satırlı metin girişi imlecini sonraki satıra taşı                              |
| gx_multi_line_text_input_end               | Çok satırlı metin girişi imlecini geçerli satırın sonuna taşı                |
| gx_multi_line_text_input_event_process    | İşlem çok satırlı metin girişi metni                                              |
| gx_multi_line_text_input_fill_color_set  | Çok satırlı metin girişi için doldur renklerini ayarla                                       |
| gx_multi_line_text_input_home              | Çok satırlı metin girişi imlecini geçerli satırın başlangıcına taşı              |
| gx_multi_line_text_input_left_arrow       | Çok satırlı metin girişi imlecini bir karakter sola taşı                         |
| gx_multi_line_text_input_right_arrow      | Çok satırlı metin giriş imlecini bir karakter sağa taşı                        |
| gx_multi_line_text_input_style_add        | Çok satırlı metin stili bayrakları Ekle                                                 |
| gx_multi_line_text_input_style_remove     | Çok satırlı metin stili bayraklarını kaldır                                              |
| gx_multi_line_text_input_style_set        | Çok satırlı metin stili bayrakları ata                                              |
| gx_multi_line_text_input_text_color_set  | Çok satırlı metin girişi için metin renkleri atama                                    |
| gx_multi_line_text_input_text_select      | Çok satırlı metin giriş metnini seçin                                               |
| gx_multi_line_text_input_text_set         | Çok satırlı metin girişine metin atama (kullanım dışı)                               |
| gx_multi_line_text_input_text_set_ext          | Çok satırlı metin girişine metin atama                         |
| gx_multi_line_text_input_up_arrow               | Çok satırlı metin girişi imlecini önceki satıra taşı       |
| gx_multi_line_text_view_create                   | Çok satırlı metin görünümü oluştur                                  |
| gx_multi_line_text_view_event_process           | Çok satırlı metin görünümü olayını işle                           |
| gx_multi_line_text_view_font_set                | Çok satırlı metin görünümünde kullanılan yazı tipini ayarlama                        |
| gx_multi_line_text_view_line_space_set         | Çok satırlı metin görünümü satır alanını ayarla                          |
| gx_multi_line_text_view_scroll_info_get        | Çok satırlı metin görünümü kaydırma bilgisi al                         |
| gx_multi_line_text_view_text_color_set         | Taçarya çizgisi metin görünümünde metin rengi ayarla                       |
| gx_multi_line_text_view_text_id_set            | Birden çok satırlı metin görünümünde sistem metin dizesi ayarla               |
| gx_multi_line_text_view_text_set                | Kullanıcı tanımlı dizeyi çok satırlı metin görünümüne ayarla (kullanım dışı) |
| gx_multi_line_text_view_text_set_ext           | Kullanıcı tanımlı dizeyi çok satırlı metin görünümüne ayarla              |
| gx_multi_line_text_view_whitespace_set          | Çok satırlı metin görünümü boşluğu ayarla                          |
| gx_numeric_pixelmap_prompt_create                 | Sayısal pixelmap istemi oluştur                               |
| gx_numeric_pixelmap_prompt_format_ function_set | Sayısal pixelmap isteminin biçim işlevini geçersiz kıl          |
| gx_numeric_pixelmap_prompt_value_set             | Sayısal istem değeri ayarla                                     |
| gx_numeric_prompt_create                           | Sayısal istem oluştur                                        |
| gx_numeric_prompt_format_function_set            | Sayısal istem için biçim işlevini geçersiz kıl                   |
| gx_numeric_prompt_value_set                       | Sayısal istem değeri ayarla                                     |
| gx_numeric_scroll_wheel_create                    | Sayısal kaydırma tekerleği oluşturma pencere öğesi                           |
| gx_numeric_scroll_wheel_range_set                | Kaydırma tekerleği değer aralığını ata                              |
| gx_pixelmap_button_create                          | Pixelmap oluştur düğmesi                                       |
| gx_pixelmap_button_draw                            | Pixelmap çiz düğmesi                                         |
| gx_pixelmap_button_event_process                  | Pixelmap düğmesi olay işleme                             |
| gx_pixelmap_button_pixelmap_set                   | Pixelmap 'te pixelmap ayarla düğmesi                              |
| gx_pixelmap_prompt_create                          | Pixelmap istemi oluştur                                       |
| gx_pixelmap_prompt_draw                            | Pixelmap istemi çiz                                         |
| gx_pixelmap_prompt_pixelmap_set                   | Pixelmap isteminde pixelmap ayarla                              |
| gx_pixelmap_slider_create                          | Pixelmap kaydırıcı oluştur                                       |
| gx_pixelmap_slider_draw                            | Pixelmap kaydırıcısını çiz                                         |
| gx_pixelmap_slider_event_process        | Pixelmap kaydırıcı olay işleme       |
| gx_pixelmap_slider_pixelmap_set         | Pixelmap kaydırıcısının içinde pixelmap ayarla        |
| gx_progress_bar_background_draw         | Çizim ilerleme çubuğu arka planı           |
| gx_progress_bar_create                   | İlerleme çubuğu oluşturma                  |
| gx_progress_bar_draw                     | İlerleme çubuğu çiz                    |
| gx_progress_bar_event_process           | İlerleme çubuğu olayını işleme           |
| gx_progress_bar_font_set                | İlerleme çubuğu metninin yazı tipini ayarla          |
| gx_progress_bar_info_set                | İlerleme çubuğu bilgi yapısını ayarla |
| gx_progress_bar_pixelmap_set            | İlerleme çubuğu çizmek için kullanılan pixelmap 'i ayarla |
| gx_progress_bar_range_set               | İlerleme çubuğunun değer aralığını ayarla        |
| gx_progress_bar_text_color_set         | İlerleme çubuğu metin rengini ayarla            |
| gx_progress_bar_text_draw               | Çizim ilerleme çubuğu metni                 |
| gx_progress_bar_value_set               | İlerleme çubuğu değerini ayarla                 |
| gx_prompt_create                          | İstem oluştur                          |
| gx_prompt_draw                            | Çizim istemi                            |
| gx_prompt_event_process                   | İşlem istemi olayı                   |
| gx_prompt_font_set                       | İstem yazı tipini ayarla                        |
| gx_prompt_text_color_set                | İstem metni rengini ayarla                  |
| gx_prompt_text_draw                      | İstem çizmenin metin çizimi bölümü    |
| gx_prompt_text_get                       | İstem metnini al (kullanım dışı)           |
| gx_prompt_text_get_ext                  | İstem metnini al                        |
| gx_prompt_text_id_set                   | İstemi sistem metin dizesiyle ayarla     |
| gx_prompt_text_set                       | İstem metnini ayarla (kullanım dışı)           |
| gx_prompt_text_set_ext                  | İstem metnini ayarla                        |
| gx_radial_progress_bar_anchor_set      | Başlangıç açısını ayarla                     |
| gx_radial_progress_bar_background_draw | Radyal ilerleme çubuğu arka planı çiz    |
| gx_radial_progress_bar_create           | Radyal ilerleme çubuğu oluşturma           |
| gx_radial_progress_bar_draw             | Radyal ilerleme çubuğu çiz             |
| gx_radial_progress_bar_event_process   | Radyal ilerleme çubuğu olayını işle      |
| gx_radial_progress_bar_font_set        | Radyal ilerleme çubuğu yazı tipini ayarla           |
| gx_radial_progress_bar_info_set        | Radyal ilerleme çubuğu bilgilerini ayarlama    |
| gx_radial_progress_bar_text_color_set | Radyal ilerleme çubuğu metin rengini ayarla     |
| gx_radial_progress_bar_text_draw       | Radyal ilerleme çubuğu metni çiz          |
| gx_radial_progress_bar_value_set       | Radyal ilerleme çubuğu değerini ayarla          |
| gx_radio_button_create                   | Radyo düğmesi oluştur                    |
| gx_radio_button_draw                     | Çizim radyo düğmesi                      |
| gx_radio_button_pixelmap_set            | Radyo düğmesinde pixelmap ayarla           |
| gx_radial_slider_anchor_angles_set     | Radyal kaydırıcı bağlayıcı açısı listesini ayarla    |
| gx_radial_slider_angle_set              | Radyal kaydırıcı açısını ayarla                |
| gx_radial_slider_animation_set          | Radyal kaydırıcı animasyon bilgilerini ayarlama       |
| gx_radial_slider_animation_start               | Radyal kaydırıcı açısını animasyonla ayarla                      |
| gx_radial_slider_create                         | Radyal kaydırıcı oluşturma                                      |
| gx_radial_slider_draw                           | Radyal kaydırıcı çiz                                        |
| gx_radial_slider_event_process                 | Radyal kaydırıcı olayını işleme                               |
| gx_radial_slider_info_get                      | Radyal kaydırıcı bilgisi işaretçisini al                  |
| gx_radial_slider_info_set                      | Radyal kaydırıcı bilgilerini ayarlama                               |
| gx_radial_slider_pixelmap_set                  | Radyal kaydırıcı pixelmaps ayarlayın                                 |
| gx_rich_text_view_create                       | Zengin metin görünümü oluşturma                                     |
| gx_rich_text_view_draw                         | Zengin metin görünümü çiz                                         |
| gx_rich_text_view_set_fonts                    | Zengin metin görünümü yazı tiplerini ayarlama                                    |
| gx_rich_text_view_text_draw                    | Zengin metin görünümü metni çiz                                    |
| gx_screen_stack_create                          | GUX ekran yığını denetim bloğu ve bellek alanını oluşturun. |
| gx_screen_stack_pop                             | Ekran yığınından en üstteki ekranı açılır.                   |
| gx_screen_stack_push                            | Geçerli ekranı ekran yığınına gönderin.                |
| gx_screen_stack_reset                           | Ekran yığınını sıfırlama                                      |
| gx_scroll_wheel_create                          | Taban kaydırma tekerleği oluştur pencere öğesi                             |
| gx_scroll_wheel_event_process                  | Kaydırma tekerleği olay işleme                               |
| gx_scroll_wheel_gradient_alpha_set            | Kaydırma tekerleği yer paylaşımı degradesini Değiştir                        |
| gx_scroll_wheel_row_height_set                | Kaydırma tekerleği satır yüksekliğini ata                              |
| gx_scroll_wheel_selected_background_set       | Seçili satır için arka plan resmi ata                    |
| gx_scroll_wheel_selected_get                   | Seçili satır dizinini al                                 |
| gx_scroll_wheel_selected_set                   | Seçili satır dizinini ata                                   |
| gx_scroll_wheel_speed_set                      | Kaydırma hızı ata                                      |
| gx_scroll_wheel_total_rows_set                | Toplam kullanılabilir satır sayısını ata                       |
| gx_scrollbar_draw                                | Kaydırma çubuğu çiz                                              |
| gx_scrollbar_event_process                      | İşlem kaydırma çubuğu olayı                                     |
| gx_scrollbar_limit_check                        | Kaydırma çubuğu sınırını denetle                                       |
| gx_scrollbar_reset                               | Kaydırma çubuğunu Sıfırla                                             |
| gx_scrollbar_value_set                          | Kaydırma çubuğu değeri ata                                      |
| gx_single_line_text_input_backspace           | İşleç geri alma karakteri                                  |
| gx_single_line_text_input_buffer_clear       | Karakter arabelleğini temizle                                  |
| gx_single_line_text_input_buffer_get         | Arabellek işaretçisini al                                     |
| gx_single_line_text_input_character_delete   | Karakteri sil                                            |
| gx_single_line_text_input_character_insert   | Karakter ekle                                            |
| gx_single_line_text_input_create              | Tek satırlık metin girişi oluştur                               |
| gx_single_line_text_input_draw                | Tek satırlı metin girişi pencere öğesi çiz                          |
| gx_single_line_text_input_draw_position_get | Metin çizme başlangıç konumunu al                           |
| gx_single_line_text_input_end                 | İmleci sona taşı                                          |
| gx_single_line_text_input_event_process      | Metin girişi olay işleme                                 |
| gx_single_line_text_input_fill_color_set    | Tek satırlık metin girişi için doldur renklerini ayarla                  |
| gx_single_line_text_input_home                | İmleci ana sayfaya taşı                                         |
| gx_single_line_text_input_left_arrow         | Sol ok tuşunu işle                                       |
| gx_single_line_text_input_position_get       | İmleç konumunu al                                         |
| gx_single_line_text_input_right_arrow        | Sağ ok tuşunu işle                                      |
| gx_single_line_text_input_style_add          | Stil bayrakları Ekle                                             |
| gx_single_line_text_input_style_remove       | Stil bayraklarını kaldır                                          |
| gx_single_line_text_input_style_set          | Stil bayrakları ata                                          |
| gx_single_line_text_input_text_color_set  | Tek satırlı metin girişi için metin renkleri ayarlama                      |
| gx_single_line_text_input_text_select     | Tek satırlık metin giriş metnini seçin                              |
| gx_single_line_text_input_text_set        | Tek satırlı metin giriş metnini ayarla (kullanım dışı)                    |
| gx_single_line_text_input_text_set_ext    | Tek satırlık metin giriş metnini ayarla                                 |
| gx_slider_create                          | Kaydırıcı oluştur                                                   |
| gx_slider_draw                            | Çizim kaydırıcısı                                                     |
| gx_slider_event_process                   | İşlem kaydırıcı olayı                                            |
| gx_slider_info_set                        | Kaydırıcı bilgi bloğunu ayarla                                    |
| gx_slider_needle_draw                     | Çiz kaydırıcı iğne                                              |
| gx_slider_needle_position_get             | Kaydırıcı iğne konumunu al                                      |
| gx_slider_tickmarks_draw                  | Çiz kaydırıcı tickiþaretleri                                           |
| gx_slider_travel_get                      | Kaydırıcı gezmasını al                                               |
| gx_slider_value_calculate                 | Kaydırıcı değerini hesapla                                          |
| gx_slider_value_set                       | Kaydırıcı değerini ayarla                                                |
| gx_sprite_create                          | GX_SPRITE pencere öğesi oluştur                                         |
| gx_sprite_current_frame_set               | Sprite pencere öğesi için geçerli görüntüleme çerçevesini ata                  |
| gx_sprite_frame_list_set                  | Bir sprite çerçeve listesi atama veya değiştirme                            |
| gx_sprite_start                           | Bir sprite dizisi Başlat                                         |
| gx_sprite_stop                            | Bir sprite sırasını durdur                                          |
| gx_string_scroll_wheel_create             | `GX_STRING_SCROLL_WHEEL`Pencere öğesi oluştur                          |
| gx_string_scroll_wheel_event_process      | İşlem dizesi kaydırma tekerleği olayı                               |
| gx_string_scroll_wheel_string_id_list_set | Dize kimlikleri dizisi ata                                      |
| gx_string_scroll_wheel_string_list_set    | Görünen dize dizisini Değiştir                                   |
| gx_string_scroll_wheel_text_get           | Kaydırma tekerleği satırı için metin al                              |
| gx_studio_widget_create                   | Studio 'da tanımlanan pencere öğesi oluştur                             |
| gx_studio_named_widget_create             | Studio 'da tanımlanan ekran oluşturma                             |
| gx_studio_display_configure               | Oluşturma ve başlatma `GX_DISPLAY` , `GX_CANVAS` ve `GX_WINDOW_ROOT` |
| gx_system_active_language_set             | Etkin dil KIMLIĞINI ata                                       |
| gx_system_canvas_refresh                  | Kirli tuvaller olduklarından 'lerin yenilenmesini (çizimini) zorla                       |
| gx_system_dirty_mark                      | Alanı kirli olarak işaretle                                                 |
| gx_system_dirty_partial_add               | Kısmi alanı kirli olarak işaretle                                         |
| gx_system_draw_context_get                | Çizim bağlamını al                                             |
| gx_system_event_fold                      | Foldevent                                                       |
| gx_system_event_send                      | Olayı gönder                                                      |
| gx_system_focus_claim                     | Talep odaklı                                                     |
| gx_system_initialize                      | GUX 'i Başlat                                                 |
| gx_system_language_table_get              | Dil tablosunu al                                         |
| gx_system_language_table_set              | Dil tablosu ata                                           |
| gx_system_memory_allocator_set            | Bellek ayırıcı veya ayırıcı atama                            |
| gx_system_pen_configure                  | Kalem yapılandırmasını ayarla                                  |
| gx_system_screen_stack_create           | Ekran yığını denetimi oluştur                            |
| gx_system_screen_stack_get              | Ekran yığını işaretçilerini al                         |
| gx_system_screen_stack_pop              | Ekran yığınından açılan pencere ekranı                       |
| gx_system_screen_stack_push             | Ekran yığınına belirtilen ekranı gönder              |
| gx_system_screen_stack_reset            | Ekran yığınını sıfırlama                                 |
| gx_system_scroll_appearance_get         | Kaydırma görünümü al                                  |
| gx_system_scroll_appearance_set         | Kaydırma görünümünü ayarla                                  |
| gx_system_start                           | GUX 'i Başlat                                             |
| gx_system_string_get                     | Dizeyi al                                             |
| gx_system_string_table_get              | Dize tablosu al                                       |
| gx_system_string_table_set              | Dize tablosu ayarla                                       |
| gx_system_string_width_get              | Dize genişliğini al (kullanım dışı)                          |
| gx_system_string_width_get_ext         | Dize genişliğini al                                       |
| gx_system_theme_install                  | Yazı tipi/renk/pixelmap tabloları 'nı yükler                     |
| gx_system_timer_start                    | Zamanlayıcıyı Başlat                                            |
| gx_system_timer_stop                     | Zamanlayıcıyı durdur                                             |
| gx_system_version_string_get            | GUX kitaplığı sürüm dizesini al (kullanım dışı)      |
| gx_system_version_string_get_ext       | GUX kitaplığı sürüm dizesini al                   |
| gx_system_widget_find                    | Pencere öğesi bul                                            |
| gx_text_button_create                    | Metin oluştur düğmesi                                     |
| gx_text_button_draw                      | Metin çiz düğmesi                                       |
| gx_text_button_event_process             | İşlem metni düğmesi olayı                              |
| gx_text_button_font_set                 | Metin düğmesi için yazı tipi ayarla                               |
| gx_text_button_text_color_set          | Metin düğmesi rengini ayarla                                  |
| gx_text_button_text_draw                | Düğme çiziminin metin çizimi bölümü                 |
| gx_text_button_text_get                 | Metin düğmesinde kullanılan metni al (kullanım dışı)              |
| gx_text_button_text_get_ext            | Metin düğmesinde kullanılan metni Al düğmesi                           |
| gx_text_button_text_id_set             | Metin düğmesine sistem dizesi atama düğmesi                    |
| gx_text_button_text_set                 | Metin düğmesine Kullanıcı tanımlı dize ata (kullanım dışı) |
| gx_text_button_text_set_ext            | Metin düğmesine Kullanıcı tanımlı dize ata düğmesi              |
| gx_text_scroll_wheel_callback_set      | Dize alma geri araması ata (kullanım dışı)          |
| gx_text_scroll_wheel_callback_set_ext | Dize alma geri araması ata                       |
| gx_text_scroll_wheel_create             | Taban metin kaydırma tekerleği oluştur                          |
| gx_text_scroll_wheel_draw               | Metinsel kaydırma tekerleği çizim işlevi                  |
| gx_text_scroll_wheel_event_process      | Metin kaydırma tekerleği olayını işle                        |
| gx_text_scroll_wheel_font_set          | Metin kaydırma tekerleği yazı tiplerini ata                         |
| gx_text_scroll_wheel_text_color_set   | Metin kaydırma tekerleği metin renkleri ata                   |
| gx_tree_view_create                    | Bir ağaç görünümünü cretae                          |
| gx_tree_view_draw                      | Ağaç görünümünü çiz                              |
| gx_tree_view_event_process            | İşlem Ağacı Görünümü olayı                     |
| gx_tree view_indentation_set           | Ağaç görünümü girintisini ayarla                   |
| gx_tree_view_position                  | Ağaç Görünüm öğelerini Konumlandır                    |
| gx_tree_view_root_line_color_set    | Ağaç görünümü kök çizgi rengini ayarla               |
| gx_tree_view_root_pixelmap_set       | Ağaç görünümü kök pixelmaps ayarla                |
| gx_tree_view_selected_get             | Seçili öğeyi al                      |
| gx_tree_view_selected_set             | Seçili öğeyi ayarla                           |
| gx_utility_canvas_to_bmp              | Tuval belleğini bit eşlem biçimine Dönüştür      |
| gx_utility_circle_point_get           | Daire üzerinde hesaplama noktası               |
| gx_utility_gradient_create             | Bir gradyan pixelmap oluşturun                  |
| gx_utility_gradient_delete              | Bir gradyan pixelmap silme                  |
| gx_utility_ltoa                         | Uzun tamsayıyı ASCII 'ye Dönüştür               |
| gx_utility_math_acos                   | İşlem yay kosinüsü                          |
| gx_utility_math_asin                   | İşlem yay sinüsü                             |
| gx_utility_math_cos                    | İşlem kosinüsü                              |
| gx_utility_math_sin                    | İşlem sinüsü                                |
| gx_utility_math_sqrt                   | İşlem kare kökü                         |
| gx_utility_bidi_paragraph_reorder         | BiDi metnini görüntüleme sırasına göre yeniden sırala|
| gx_utility_bidi_resolved_text_info_delete | Yeniden düzenlenen BiDi metnini Sil               |
| gx_utility_pixelmap_resize             | Pixelmap 'i yeniden boyutlandır                             |
| gx_utility_pixelmap_rotate             | Pixelmap 'i rastgele bir açıda döndürün          |
| gx_utility_pixelmap_simple_rotate      | Pixelmap 'i 90, 180, 270 derece döndürün     |
| gx_utility_rectangle_center            | Dikdörtgeni başka bir dikdörtgen içinde ortala   |
| gx_utility_rectangle_center_find      | Dikdörtgenin merkezini bul                    |
| gx_utility_rectangle_combine           | İlk olarak iki dikdörtgeni birleştirin           |
| gx_utility_rectangle_compare           | İki dikdörtgeni karşılaştırın                      |
| gx_utility_rectangle_define            | Dikdörtgen tanımla                            |
| gx_utility_rectangle_resize            | Dikdörtgeni yeniden boyutlandır                            |
| gx_utility_rectangle_overlap_detect   | Dikdörtgenlerin çakışmasını Algıla                |
| gx_utility_rectangle_point_detect     | Noktanın dikdörtgende yer alıyorsa Algıla        |
| gx_utility_rectangle_shift             | Kaydırma dikdörtgeni                             |
| gx_utility_string_to_alphamap         | Metin dizesini harflerden haritaya işle (kullanım dışı) |
| gx_utility_string_to_alphamap_ext    | Metin dizesini harflerden haritaya işle              |
| gx_vertical_list_children_position    | Alt öğeleri dikey listede Konumlandır          |
| gx_vertical_list_create                | Dikey liste oluştur                        |
| gx_vertical_list_event_process        | Dikey liste olayını işle                 |
| gx_vertical_list_selected_index_get  | Seçili öğe dizinini al                     |
| gx_vertical_list_selected_widget_get | Seçili pencere öğesini al                         |
| gx_vertical_list_selected_set         | Girişi dikey listede ayarla                  |
| gx_vertical_list_total_rows_set      | Oluşturulduktan sonra liste satırlarının sayısını değiştirme   |
| gx_vertical_scrollbar_create           | Dikey kaydırma çubuğu oluştur                   |
| gx_widget_allocate                      | Dinamik olarak pencere öğesi ayırma               |
| gx_widget_attach                        | Pencere öğesini üste Ekle                     |
| gx_widget_background_draw              | Pencere öğesi arka planı çiz                      |
| gx_widget_back_attach                  | Pencere öğesini geri Ekle                       |
| gx_widget_back_move                    | Pencere öğesini arkaya taşı                         |
| gx_widget_block_move                   | Piksel bloğunu taşı                        |
| gx_widget_border_draw                  | Pencere öğesi kenarlığını çiz                          |
| gx_widget_border_style_set            | Pencere öğesi kenarlık stilini ayarla                     |
| gx_widget_border_width_get            | Pencere öğesi kenarlık genişliğini ayarla                     |
| gx_widget_canvas_get               | Pencere öğesi tuvali al                                                         |
| gx_widget_child_detect             | Pencere öğesi alt öğesini Algıla                                                       |
| gx_widget_children_draw            | Pencere öğesi alt öğeleri çiz                                                      |
| gx_widget_client_get               | Pencere öğesi istemci alanını al                                                    |
| gx_widget_color_get                | Görünür bir pencere öğesi için renk KIMLIĞINI renk değerine çözümle                      |
| gx_widget_create                    | Pencere öğesi oluştur                                                             |
| gx_widget_created_test             | Pencere öğesi oluşturulduysa test                                                    |
| gx_widget_delete                    | Pencere öğesini Sil                                                             |
| gx_widget_detach                    | Pencere öğesini üst öğeden ayır                                                 |
| gx_widget_draw                      | Pencere öğesi çiz                                                               |
| gx_widget_draw_set                 | Pencere öğesinin çizim işlevini ayarla                                               |
| gx_widget_event_generate           | Pencere öğesi olayı oluştur                                                     |
| gx_widget_event_process            | İşlem pencere öğesi olayı                                                      |
| gx_widget_event_process_set       | Pencere öğesinin olay işleme işlevini ayarla                                   |
| gx_widget_event_to_parent         | Etkinliği pencere öğesinin üst öğesine gönder                                             |
| gx_widget_fill_color_set          | Pencere öğesi dolgusu rengini ata                                                  |
| gx_widget_find                      | Pencere öğesi bul                                                               |
| gx_widget_first_child_get         | İlk alt öğeye İşaretçiyi döndür                                             |
| gx_widget_focus_next               | Giriş odağını sonraki pencere öğesine taşı                                           |
| gx_widget_focus_previous           | Giriş odağını önceki pencere öğesine taşı                                       |
| gx_widget_font_get                 | Yazı tipi KIMLIĞINI görünür pencere öğesi için yazı tipi işaretçisine çözümleme                    |
| gx_widget_free                      | Ücretsiz pencere öğesi denetim blok belleği                                          |
| gx_widget_front_move               | Pencere öğesini öne taşı                                                      |
| gx_widget_height_get               | Pencere öğesi yüksekliğini al                                                         |
| gx_widget_hide                      | Pencere öğesini gizle                                                               |
| gx_widget_last_child_get          | Son alt öğeye döndürme işaretçisi                                              |
| gx_widget_next_sibling_get        | Sonraki eşdüzey için işaretçiyi döndür                                            |
| gx_widget_parent_get               | Üst pencere öğesine işaretçi döndür                                           |
| gx_widget_pixelmap_get             | Bir görünür pencere öğesi için pixelmap KIMLIĞINI bir pixelmap işaretçisine çözümleyin            |
| gx_widget_previous_sibling_get    | İşaretçiyi önceki eşdüzey öğeye döndür                                        |
| gx_widget_resize                    | Pencere öğesini yeniden boyutlandır                                                             |
| gx_widget_shift                     | Kaydırma pencere öğesi                                                              |
| gx_widget_show                      | Pencere öğesini göster                                                               |
| gx_widget_status_add               | Pencere öğesi durumu Ekle                                                         |
| gx_widget_status_get               | Pencere öğesi durum bayraklarını al                                              |
| gx_widget_status_remove            | Pencere öğesi durumunu kaldır                                                      |
| gx_widget_string_get               | Görünür pencere öğesi için dize KIMLIĞIYLE ilişkili dizeyi al (kullanım dışı) |
| gx_widget_string_get_ext          | Görünür pencere öğesi için dize KIMLIĞIYLE ilişkili dizeyi al.             |
| gx_widget_status_test              | Test pencere öğesi durumu                                                        |
| gx_widget_style_add                | Pencere öğesi stili Ekle                                                          |
| gx_widget_style_get                | Pencere öğesi stil bayraklarını al                                               |
| gx_widget_style_remove             | Pencere öğesi stilini kaldır                                                       |
| gx_widget_style_set                | Pencere öğesi stilini ayarla                                                          |
| gx_widget_text_blend               | Karışık metni pencere öğesi üzerinde işle (kullanım dışı)                              |
| gx_widget_text_blend_ext          | Karışık metni pencere öğesi üzerinde işle                                           |
| gx_widget_text_draw                | Metni pencere öğesi üzerinde işle (kullanım dışı)                                      |
| gx_widget_text_draw_ext           | Metni pencere öğesi üzerinde işle                                            |
| gx_widget_text_id_draw            | Pencere öğesi üzerinde dize KIMLIĞIYLE tanımlanan metni işle                           |
| gx_widget_top_visible_child_find | İşaretçiyi Z sırasının en üstünde çizilen, görünür alt öğeye döndür   |
| gx_widget_type_find                | Pencere öğesi türünü bul                                                          |
| gx_widget_width_get                | Pencere öğesi genişliğini al                                                          |
| gx_window_canvas_set               | Pencere tuvali ayarla                                                         |
| gx_window_client_height_get       | Pencere istemci yüksekliğini al                                                  |
| gx_window_client_scroll            | Pencere istemcilerini kaydır                                                     |
| gx_window_client_width_get        | Pencere istemci genişliğini al                                                   |
| gx_window_close                     | Kalıcı pencere yürütmeyi Sonlandır                                          |
| gx_window_create                    | Pencere oluştur                                                             |
| gx_window_draw                      | Pencereyi çiz                                                               |
| gx_window_event_process            | İşlem penceresi olayı                                                      |
| gx_window_execute                   | Kalıcı pencere yürütme                                                    |
| gx_window_root_create              | Kök penceresi oluştur                                                        |
| gx_window_root_delete              | Kök penceresini yok et                                                       |
| gx_window_root_event_process      | Kök penceresi için işlem olayı                                             |
| gx_window_root_find                | Kök penceresini bul                                                          |
| gx_window_scroll_info_get         | Pencere kaydırma bilgisini al                                                    |
| gx_window_scrollbar_find           | Pencere kaydırma çubuğunu bul                                                     |
| gx_window_wallpaper_get            | Pencere duvar kağıdını al                                                      |
| gx_window_wallpaper_set            | Pencere duvar kağıdını ayarla                                                      |

## <a name="gx_accordion_menu_create"></a>gx_accordion_menu_create

Accordion menüsü oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_accordion_menu_create(
    GX_ACCORDION_MENU *accordion,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    ULONG style ,
    USHORT accordion_menu_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen bir Accordion menüsü oluşturur ve Accordion menüsünü sağlanan üst pencere öğesine ekler. Bir Accordion menüsü, genişleyen/daraltma menü pencere öğesi. Alt menü öğeleri olarak tüm pencere öğesi türlerini kabul eder. Accordion menüleri iç içe olabilir, yani birçok menü derinliği düzeyi oluşturulabilir.

Bir menü öğesi pencere öğesine bir alt öğe eklemek için, bir ana menü öğesi olarak GX_MENU türü pencere öğesi kullanmanız önerilir.

Tek düzeyli Accordion menüsü oluşturma ipuçları:

1.  Bir Accordion menüsü oluşturun.

2.  Accordion menüsüne GX_MENU türü pencere öğeleri ekleyin.

3.  Alt pencere öğelerini GX_MENU türü üst öğesine ekleyin. Alt öğe türü herhangi bir GUıDX pencere öğesi türü olabilir.

Çoklu düzey Accordion menüsü oluşturma ipuçları:

1.  Bir Accordion menüsü oluşturun.

2.  Accordion menüsüne GX_MENU türü pencere öğeleri ekleyin.

3.  GX_ACCORDION_MENU türü pencere öğesini GX_MENU türü üst öğesine ekleyin.

4.  GX_ACCORDION_MENU türü üst öğesine, tek düzeyli ACCORDION menü oluşturma bölümünde açıklandığı gibi menü öğeleri ekleyin.

### <a name="parameters"></a>Parametreler

- **Accordion** Accordion Menu denetim bloğu işaretçisi
- **ad** Accordion menüsünün adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **Stil** Pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **accordion_menu_id** Accordion menüsünün uygulama tanımlı KIMLIĞI
- **Boyut** Accordion menüsünün boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı Accordion menüsü oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ACCORDION_MENU my_accordion;
GX_MENU menu_1;
GX_MENU item_1;
GX_RECTANGLE size;

gx_utility_rectangle_define(&size, 100, 100, 300, 150);

status = gx_accordion_menu_create(&my_accordion, “my_accordion”,
                                  parent, GX_STYLE_ENABLED,
                                  MY_ACCORDION_ID, &size);

gx_menu_create(&menu_1, “menu_1”, &my_accordion,
               GX_STRING_ID_MENU_1, GX_ID_NONE,
               GX_STYLE_ENABLED | GX_TYLE_BORDER_THIN, 0, &size);

gx_menu_create(&item_1, “item_1”, &my_accordion,
               GX_STRING_ID_ITEM_1, GX_ID_NONE,
               GX_STYLE_ENABLED | GX_STYLE_BORDER_THIN, 0, &size);

gx_text_offset_set(&item_1, 30, 0);

gx_menu_insert(&menu_1, &item_1);

/* If status is GX_SUCCESS the accordion menu was successfully created. */

```

GUX Studio yüklemesinin bir parçası olarak sağlanan demo uygulaması demo_guix_widget_types, Accordion Menü pencere öğesini kullanma hakkında tamamen bir örnek sağlar.

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_menu_draw
- gx_accordion_menu_event_process
- gx_accordion_menu_position
- gx_menu_create
- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set

## <a name="gx_accordion_menu_draw"></a>gx_accordion_menu_draw

Accordion menüsünü çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_accordion_menu_draw(GX_ACCORDION_MENU *accordion);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen Accordion menüsünü çizer. Bu hizmet normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel Accordion Menü pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **Accordion** Accordion Menu denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Define a custom accordion menu draw function */

VOID my_accordion_menu_draw(GX_ACCORDION_MENU *accordion)
{
    /* Call default accordion menu draw. */
    gx_accordion_menu_draw(accordion);

    /* Add custom drawing here. */
}

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_menu_create
- gx_accordion_menu_event_process
- gx_accordion_menu_position
- gx_menu_create
- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set

## <a name="gx_accordion_menu_event_process"></a>gx_accordion_menu_event_process

İşlem Accordion Menü olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_accordion_menu_event_process(
    GX_ACCORDION_MENU *accordion, 
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen Accordion menüsü için bir olayı işler. Bu hizmet özel Accordion Menü olay işleme işlevleri tarafından varsayılan olay işleyicisi olarak çağrılmalıdır.

Bu hizmet, bir menü öğesini genişletmek/Kolaps için GX_EVENT_PEN_DOWN ve GX_EVENT_PEN_UP olaylarını işler.

### <a name="parameters"></a>Parametreler

- **Accordion** Accordion Menu denetim bloğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı Accordion Menü olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic accordion menu event processing as part of custom event processing function. */

UINT custom_accordion_event_process( 
    GX_ACCORDION_MENU *accordion,
    GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;

    default:
        /* Pass all other events to the default accordion menu
            event processing */
        status =
        gx_accordion_menu_event_process(accordion, event);
        break;
    }
    return status;
}

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_menu_create
- gx_accordion_menu_draw
- gx_accordion_menu_position
- gx_menu_create
- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set

## <a name="gx_accordion_menu_position"></a>gx_accordion_menu_position

Menü öğelerini Konumlandır

### <a name="prototype"></a>Prototype

```C
UINT gx_accordion_menu_position(GX_ACCORDION_MENU *accordion);
```

### <a name="description"></a>Açıklama

Bu hizmet, Accordion menüsünün Menü öğelerini konumlandırır. Bu işlev, Accordion menüsü görünür olduğunda normalde dahili olarak çağırılır. Bir Accordion menüsüne/öğeden öğe eklemek/kaldırmak veya alt öğenin genişletme stillerini değiştirmek istiyorsanız, alt öğelerin yeniden konumlandırılabilmesi için bu işlev çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **Accordion** Accordion Menu denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı Accordion Menü konumu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Position menu items in the accordion menu “my_accordion” */
status = gx_accordion_menu_position (&my_accordion);

/* If status is GX_SUCCESS the children in the accordion menu
“my_accordion” are positioned. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_menu_create
- gx_accordion_menu_draw
- gx_accordion_menu_event_process
- gx_menu_create
- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set

## <a name="gx_animation_canvas_define"></a>gx_animation_canvas_define

Animasyon denetleyicisine tuval belleği sağlama

### <a name="prototype"></a>Prototype

```C
UINT gx_animation_canvas_define(
    GX_ANIMATION *animation, 
    GX_CANVAS *canvas);
```

### <a name="description"></a>Açıklama

Bu hizmet, Animasyon sırasını uygulamak için kullanılan bir animasyon denetleyicisine bir bellek tuvali sağlar. Bu sunulan tuval animasyon hedefi pencere öğesini tutabilecek kadar büyük olmalıdır.

Bir animasyon tuvali tanımlandığında, hedef pencere öğesi bu animasyon tuvaline bir kez çizilir ve tuval boşluğu ve/veya tuval alfa değeri değiştirilerek ekran slaydı veya Soldur efekti gerçekleştirilir. Birden çok grafik katmanı için donanım desteği sağlandığında, bir donanım grafik kaplama katmanına bağlanan bir animasyon tuvali tanımlamak, slayt ve Soldur animasyonların performansını ***önemli ölçüde*** iyileştirebilir.

Animasyon Yöneticisi bir animasyon tuvalinin, renk derinliğinde 16 BPP bir daha az çalışıyorsa soluklaştırma ve soluklaştırma animasyon türlerini yürütmesini gerektirir.

### <a name="parameters"></a>Parametreler

- **animasyon** Animasyon denetim bloğu işaretçisi
- **tuval** Çeviri animasyonunu uygulamak için kullanılan bellek tuvali.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) animasyon tuvali başarıyla tanımlandı
- **GX_INVALID_STATUS** (0x10) geçersiz animasyon durumu
- **GX_INVALID_MEMORY_SIZE** (0x29) belirtilen bellek bloğu tuvali oluşturmak için yeterince büyük değil
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ANIMATION animation;
GX_CANVAS animation_canvas;
GX_ROOT_WINDOW animation_root;
/* Create animation canvas. */
status = gx_canvas_create(
        &animation_canvas, /* Canvas control block. */
        “animation_canvas”, /* Name of canvas. */
        display, /* Display control block. */
        GX_ANIMATION_MANAGED, /* Type of canvas. */
        width, /* Width of canvas. */
        height, /* Height of canvas. */
        memory_area, /* Memory area of canvas. */
        memory_size /* Size of canvas memory. */
        );
if (status == GX_SUCCESS)
{
    /* Create the root window for the canvas. */
    status = gx_window_root_create(
        &animation_root, /* Root window control block. */
        “animation_root”, /* Name of root window. */
        &animation_canvas, /* Canvas of the root window. */ GX_STYLE_NONE, /* Style of the window. */
        GX_ID_NONE, /* Root window ID. */
        &root_size /* Window size. */
        );
}
if (status == GX_SUCCESS)
{
    /* Define canvas for the animation. */
    status = gx_animation_canvas_define(&animation,
                &animation_canvas);
}
/* If status is GX_SUCCESS the new canvas was successfully set to the animation manager. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_animation_create,
- gx_animation_delete
- gx_animation_drag_disable,
- gx_animation_drag_enable
- gx_animation_landing_speed_set,
- gx_animation_start
- gx_animation_stop

## <a name="gx_animation_create"></a>gx_animation_create

Animasyon denetleyicisi oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_animation_create(GX_ANIMATION *animation);
```

### <a name="description"></a>Açıklama

Bu hizmet bir animasyon denetleyicisi oluşturur. Denetleyici boşta durumuna başlatılır. BOŞTA durumunda olmadığı takdirde bir animasyon başlatamaz. GX_ANIMATION denetim bloğu işaretçisi gx_system_animation_get () kullanılarak elde edilebilir veya statik olarak tanımlanmış bir denetim bloğu olabilir.

### <a name="parameters"></a>Parametreler

- **animasyon** Animasyon denetim bloğu işaretçisi


### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) animasyon denetleyicisi başarıyla oluşturuldu
- **GX_ALREADY_CREATED** (0x13) denetim bloğu zaten başlatılmış
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ANIMATION *animation;

/* Allocate an animaton control from system pool */
gx_system_animation_get(&animation);

/* Initialize the control block */

if (animation)
{
    status = gx_animation_create(&animation);
}

/* If status is GX_SUCCESS the new animation controller was successfully created and initialized. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_animation_canvas_define,
- gx_animation_delete
- gx_animation_drag_disable,
- gx_animation_drag_enable
- gx_animation_start
- gx_animation_landing_speed_set,
- gx_animation_stop
- gx_system_animation_get
- gx_system_animation_free

## <a name="gx_animation_drag_disable"></a>gx_animation_drag_disable

Ekran Sürükle animasyon kancasını devre dışı bırak

### <a name="prototype"></a>Prototype

```C
UINT gx_animation_drag_disable(
    GX_ANIMATION *animation, 
    GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesinin varsayılan olay işlemi işlevinden ekran sürükleme animasyon kanca yordamını kaldırır ve animasyon sırasını durduruyor. Ekran sürükleme animasyon kanca yordamı bir ekran sürükleme animasyonuna yönelik olayları işler.

### <a name="parameters"></a>Parametreler

- **animasyon** Animasyon denetim bloğu işaretçisi
- **pencere öğesi** Pencere öğesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ANIMATION animation;
GX_WIDGET *animation_parent;

/* Disable screen drag animation of “animation_parent”. */
status = gx_animation_drag_disable(&animation, animation_parent);

/* If status is GX_SUCCESS the screen drag hook has been removed
    from the event process of “animation_parent”. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_animation_canvas_define,
- gx__animation_create
- gx_animation_drag_enable
- gx_animation_landing_speed_set,
- gx__animation_start
- gx_animation_stop
- gx_system_animation_get,
- gx__system_animation_free

## <a name="gx_animation_drag_enable"></a>gx_animation_drag_enable

Ekran Sürükle animasyon kancasını etkinleştir

### <a name="prototype"></a>Prototype

```C
UINT gx_animation_drag_enable(
    GX_ANIMATION *animation,
    GX_WIDGET *widget, 
    GX_ANIMATION_INFO *info);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir pencere öğesinin varsayılan olay işlemi işlevinin kanca yordamı olarak dahili olarak tanımlanmış ekran sürükleme animasyonu olay işlem işlevini ayarlar. Ekran sürükleme animasyonu olay işlem işlevi bir ekran sürükleme animasyonu için olayları işler.

Ekran Sürükle kanca yordamı, hedef pencere öğesine gönderilen kalem girişi olayları için varsayılan işleyici olur. Özgün pencere öğesi olay işleme işlevi, ekran sürükleme girişi olay türlerini denetledikten sonra bir zincirleme olarak çağrılır.

### <a name="parameters"></a>Parametreler

- **animasyon** Animasyon denetim bloğu işaretçisi
- **pencere öğesi** Pencere öğesi denetim bloğu işaretçisi
- **bilgi** Animasyon bilgileri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı
- **GX_INVALID_STATUS** (0x26) geçersiz animasyon durumu
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE** (0x22) geçersiz değer
- **GX_INVALID_WIDGET** (0x12) slayt ekran listesi sağlanmadı

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ANIMATION animation;
GX_ANIMATION_INFO info;
GX_WIDGET *animation_parent;
GX_WIDGET *screen_list[] = {
    screen_1,
    screen_2,
    screen_3,
    GX_NULL
}

memset(&info, 0, sizeof(GX_ANIMATION_INFO);
info.gx_animation_parent = animation_parent;

/* If GX_STYLE_ANIMATION_WRAP is set, the screen list will wrap itself. */
info.gx_animation_style = GX_ANIMATION_SCREEN_DRAG |
                          GX_ANIMATION_HORIZONTAL |
                          GX_STYLE_ANIMATION_WRAP;
info.gx_animation_frame_interval = 1;
info.gx_animation_slide_screen_list = screen_list;

status = gx_animation_drag_enable(&animation, animation_parent,
                                  info);

/* If status is GX_SUCCESS the screen slide animinatin event
    process function has been set as a hook procedure of
    “animation_parent”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_animation_canvas_define,
- gx__animation_create
- gx_animation_drag_disable,
- gx__animation_landing_speed_set
- gx_animation_start,
- gx__animation_stop,
- gx__system_animation_get
- gx_system_animation_free

## <a name="gx_animation_landing_speed_set"></a>gx_animation_landing_speed_set

Ekran sürükleme animasyonu için giriş hızını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_animation_landing_speed_set(
    GX_ANIMATION *animation, 
    USHORT shift_per_step);
```

### <a name="description"></a>Açıklama

Bu hizmet, ekran sürükleme animasyonu için giriş hızını ayarlar.

### <a name="parameters"></a>Parametreler

- **animasyon** Animasyon denetim bloğu işaretçisi
- **shift_per_step** Her adım için kaydırma uzaklığı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı
- **GX_INVALID_VALUE** (0x22) geçersiz parametre

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set landing speed of “my_animation” to 20. */
status = gx_animation_landing_peed_set(&my_animation, 20);

/* If status is GX_SUCCESS the landing speed is successfully set to 20. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_animation_canvas_define,
- gx__animation_create
- gx_animation_slide_disable,
- gx__animation_slide_enable
- gx_animation_start,
- gx__animation_stop,
- gx__system_animation_get
- gx_system_animation_free

## <a name="gx_animation_start"></a>gx_animation_start

Zamanlayıcı temelli bir animasyon başlatma

### <a name="prototype"></a>Prototype

```C
UINT gx_animation_start(
    GX_ANIMATION *animation, 
    GX_ANIMATION_INFO *params);
```

### <a name="description"></a>Açıklama

Bu hizmet, önceden oluşturulmuş bir animasyon örneği ve yeni bir animasyon parametreleri kümesi kullanan bir animasyon sırası başlatır. Bu işlev parametrelerin yerel bir kopyasını oluşturur, yani parametre yapısının statik olarak tanımlanması gerekmez.

GX_ANIMATION denetim yapısı uygulama tarafından statik olarak tanımlanabilir veya gx_system_animation_get () API 'SI kullanılarak elde edilebilir.

GX_ANIMATION_INFO yapısı yürütülecek animasyonun parametrelerini tanımlar. Bu yapının ve her alanın anlamını açıklayan bir açıklama için, bu kılavuzun Bölüm 3 ' teki Gux animasyon bileşeni bölümüne bakın.

### <a name="parameters"></a>Parametreler

- **animasyon** Animasyon denetim bloğu işaretçisi
- **params** Parametre yapısına yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı
- **GX_INVALID_VALUE** (0x22) geçersiz parametre
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz animasyon hedefi
- **GX_INVALID_STATUS** (0x26) geçersiz animasyon durumu
- **GX_INVALID_CANVAS** (0x20) geçersiz animasyon tuvali

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ANIMATION_INFO params;
GX_ANIMATION *animation;

/* obtain an animation control block pointer */
gx_system_animation_get(&animation);
if (animation)
{
    /* define a slide down and to the right */
    params.gx_animation_start_position.gx_point_x = 0;
    params.gx_animation_start_position.gx_point_y = 0;
    params.gx_animation_end_position.gx_point_x = 100;
    params.gx_animation_end_position.gx_point_y = 200;
    params.gx_animation_style= GX_ANIMATION_TRANSLATE;
    params.gx_animation_target = &my_window;
    params.gx_animation_parent = root_window;
    params.gx_animation_start_alpha = 255;
    params.gx_animation_end_alpha = 255;

    params.gx_animation_delay_before = 0;
    params.gx_animation_steps = 10;
    params.gx_animation_tick_rate = 2;

    status = gx_animation_start(&animation, &params);
}

/* If status is GX_SUCCESS the animation is initiated. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_animation_canvas_define,
- gx__animation_create
- gx_animation_slide_disable,
- gx__animation_slide_enable
- gx_animation_landing_speed_set,
- gx__animation_stop
- gx_system_animation_get,
- gx__system_animation_free

## <a name="gx_animation_stop"></a>gx_animation_stop

Etkin Zamanlayıcı temelli bir animasyonu durdur

### <a name="prototype"></a>Prototype

```C
UINT gx_animation_stop(GX_ANIMATION *animation);
```

### <a name="description"></a>Açıklama

Daha önce başlatılan bir animasyonu durdurun. Animasyon denetim bloğu işaretçisi gx_system_animation_get kullanılarak ayrılmışsa, uygulama denetim bloğunu yeniden kullanabilir veya gx_system_animation_free () kullanarak sistem havuzuna döndürebilir.

### <a name="parameters"></a>Parametreler

- **animasyon** Animasyon denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı GX_PTR_ERROR (0X07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_STATUS** (0x26) geçersiz denetleyici durumu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ANIMATION animation;

status = gx_animation_stop(&animation);

/* If status is GX_SUCCESS the animation is stopped */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_animation_canvas_define,
- gx__animation_create
- gx_animation_drag_disable,
- gx__animation_drag_enable
- gx_animation_start,
- gx__system_animation_get
- gx_system_animation_free

## <a name="gx_binres_language_count_get"></a>gx_binres_language_count_get

İkili kaynak verilerinde mevcut dillerin sayısını döndür

### <a name="prototype"></a>Prototype

```C
UINT gx_binres_language_count_get(
    GX_UBYTE *root_address, 
    GX_VALUE *returned_count);
```

### <a name="description"></a>Açıklama

Bu hizmet, ikili verilerde bulunan dillerin sayısını döndürmek için bir ikili kaynak veri üst bilgisini ayrıştırır. Bu, kullanıcının bir dil seçiminden seçim yapmasına izin veren kullanıcı için bir seçim listesi görüntülemesi gereken uygulamalar için yararlıdır.

### <a name="parameters"></a>Parametreler

- **root_address** Bellekteki ikili kaynak verilerinin adresi
- **return_count** Döndürülen dil sayısını depolayacak konum

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı
- **GX_INVALID_FORMAT** (0x24) geçersiz ikili kaynak
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_VALUE language_count = 0;

/* Specify address that binary resource data is located. */
GX_UBYTE    *root_address = 0x60000000;

status = gx_binres_language_count_get(root_address,
    &language_count);

/* If status is GX_SUCCESS, the language table was successfully loaded. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_binres_language_info_load

## <a name="gx_binres_language_info_load"></a>gx_binres_language_info_load

Dil tablosu bilgilerini yükle

### <a name="prototype"></a>Prototype

```C
UINT gx_binres_language_info_load(
    GX_UBYTE *root_address, 
    GX_LANGUAGE_HEDAER *put_info);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir dizi GX_LANGUAGE_HEADER yapıyı doldurmak için bir ikili kaynak veri blobu ayrıştırır ve bu, ikili verilerde bulunan her dilin dil adlarının ve dize tablo boyutunun uygulamasını bilgilendirmenizi sağlar. Uygulama, ikili verilerdeki dillerin sayısını öğrenmek için önce gx_binres_language_count_get () öğesini çağırmalıdır ve bu işlev noktalarına put_info işaretçisinin language_count GX_LANGUAGE_HEADER yapıları dizisine geçtiğini sağlar.

Bu hizmet, çalışma zamanında bir ikili kaynak veri öbeğinin içeriğini öğrenmek için uygulama tarafından kullanılır.

GX_LANGUAGE_HEADER yapısı şu şekilde tanımlanır:

```c
typedef struct GX_LANGUAGE_HEADER_STRUCT{
    USHORT gx_language_header_magic_number;
    USHORT gx_language_header_index;
    UCHAR gx_language_header_name[GX_LANGUAGE_HEADER_NAME_SIZE];
    ULONG  gx_language_header_data_size;
} GX_LANGUAGE_HEADER;
```

- *Magic_number* alanı, ikili kaynak veri biçiminin iç doğrulaması için kullanılır.
- *Header_index* alanı, ikili verilerde dillerin tanımlandığı sırayı gösterir.
- *Header_name* alanı dil adını içerir.
- *Header_data_size* alanı, dil dize tablosunun veri boyutunu içerir.

### <a name="parameters"></a>Parametreler

- **root_address** Bellekteki ikili kaynak verilerinin adresi
- **put_info** GX_LANGUAGE_HEADER yapılarının dizisine yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı
- **GX_INVALID_FORMAT** (0x24) geçersiz ikili kaynak
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_LANGUAGE_HEADER language_info[4];

/* Specify address that binary resource data is located. */
GX_UBYTE    *root_address = 0x60000000;

status = gx_binres_language_info_load(root_address,
    language_info);
/* If status is GX_SUCCESS, the language table was successfully loaded. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_binres_language_count_get

## <a name="gx_binres_language_table_load"></a>gx_binres_language_table_load

Dil tablosu kaynağını yükle (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_binres_language_table_load(
    GX_UBYTE *root_address, 
    GX_UBYTE **returned_language_table);
```

### <a name="description"></a>Açıklama

Kullanım dışı bırakılan bu API, uygulamaların dize tablosu verilerini eski (sürüm 5,6 ' den önceki) ikili kaynak veri dosyalarından yüklemesine olanak tanır.

Yeni uygulamalar gx_binres_language_table_load_ext () kullanmalıdır.

Bu hizmet, tablo kaynaklarına işaretçiler içeren bir dil tablosu yapısı oluşturur, oluşturulan veri yapıları "yerinde" kaynak verilerine işaret ediyor, kaynak verileri kopyalamaz. Kaynak verileri bir genel erişim belleği konumuna yerleştirilmelidir ve bu bellek konumunun taban adresi bu API 'ye geçirilir.

Bu hizmet, dil tablosu yapısını tutmak için boyutu yeterli olan bir çalışma zamanına ayrılan bellek bloğunu gerektirir ve bu nedenle, bu hizmet istenene kadar gx_system_memory_allocator_set API 'sinin çağrılması gerekir.

Döndürülen dil tablosu, kaynak veri belleğindeki dize kaynaklarına işaretçiler içeren her dize tablosu, bir veya daha fazla dize tablosunu tanımlar.

### <a name="parameters"></a>Parametreler

- **root_address** Bellekteki ikili kaynak verilerinin adresi
- **_language_table döndürüldü** Yüklü dil tablosu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı
- **GX_INVALID_FORMAT** (0x24) geçersiz ikili kaynak
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_SYSTEM_MEMPRY_ERROR** (0x30) bellek ayırıcısı veya Free işlevi tanımlı değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_UBYTE ***language_table = GX_NULL;

/* Specify address that binary resource data is located. */
GX_UBYTE *root_address = 0x60000000;

status = gx_binres_language_table_load(root_address,
                                        &language_table);

/* If status is GX_SUCCESS, the language table was successfully loaded. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_binres_language_table_load_ext

## <a name="gx_binres_language_table_load_ext"></a>gx_binres_language_table_load_ext

Dil tablosu kaynağını yükle

### <a name="prototype"></a>Prototype

```C
UINT gx_binres_language_table_load_ext(
    GX_UBYTE *root_address, 
    GX_STRING **returned_language_table);
```

### <a name="description"></a>Açıklama

Bu hizmet, tablo kaynaklarına işaretçiler içeren bir dil tablosu yapısı oluşturur, oluşturulan veri yapıları "yerinde" kaynak verilerine işaret ediyor, kaynak verileri kopyalamaz. Kaynak verileri bir genel erişim belleği konumuna yerleştirilmelidir ve bu bellek konumunun taban adresi bu API 'ye geçirilir.

Bu hizmet, dil tablosu yapısını tutmak için boyutu yeterli olan bir çalışma zamanına ayrılan bellek bloğunu gerektirir ve bu nedenle, bu hizmet istenene kadar gx_system_memory_allocator_set API 'sinin çağrılması gerekir.

Döndürülen dil tablosu, kaynak veri belleğindeki dize kaynaklarına işaretçiler içeren her dize tablosu, bir veya daha fazla dize tablosunu tanımlar.

### <a name="parameters"></a>Parametreler

- **root_address** Bellekteki ikili kaynak verilerinin adresi
- **_language_table döndürüldü** Yüklü dil tablosu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı
- **GX_INVALID_FORMAT** (0x24) geçersiz ikili kaynak
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_SYSTEM_MEMPRY_ERROR** (0x30) bellek ayırıcısı veya Free işlevi tanımlı değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING **language_table = GX_NULL;

/* Specify address that binary resource data is located. */
GX_UBYTE *root_address = 0x60000000;

status = gx_binres_language_table_load_ext(root_address,
                                            &language_table);

/* If status is GX_SUCCESS, the language table was successfully loaded. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_binres_theme_load

## <a name="gx_binres_theme_load"></a>gx_binres_theme_load

Tema kaynağı yükle

### <a name="prototype"></a>Prototype

```C
UINT gx_binres_theme_load(
    GX_UBYTE *root_address, 
    INT theme_id, GX_THEME **returned_theme);
```

### <a name="description"></a>Açıklama

Bu hizmet, istenen temanın kaynak tablolarına yönelik işaretçiler içeren bir GX_THEME yapısı oluşturur. Oluşturulan veri yapıları "yerinde" kaynak verilerine işaret ediyor, kaynak verileri kopyalamaz. Bu nedenle, kaynak verilerinin bir genel erişim belleği konumuna yerleştirilmesi ve bu bellek konumunun temel adresi bu API 'ye geçirilmesi gerekir.

Bu hizmet, tema tablosu yapısını tutmak için boyutu yeterli olan bir çalışma zamanına ayrılan bellek bloğunu gerektirir ve bu nedenle, bu hizmet istenene kadar gx_system_memory_allocator_set API 'sinin çağrılması gerekir.

### <a name="parameters"></a>Parametreler

- **root_address** Bellekteki ikili kaynak verilerinin adresi
- **theme_id** Temanın tanımlayıcısı
- **returned_theme** Yüklü Tema işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı
- **GX_INVALID_FORMAT** (0x24) geçersiz ikili kaynak
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE** (0x22) GEÇERSIZ Tema kimliği
- **GX_SYSTEM_MEMORY_ERROR** (0x30) bellek ayırıcısı veya Free işlevi tanımlı değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR *theme = GX_NULL;
GX_UBYTE *root_address = 0x60000000;
INT theme_id = 0;

status = gx_binres_theme_load(root_address, theme_id, &theme);

/* If status is GX_SUCCESS, the theme was successfully loaded. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_binres_language_table_read

## <a name="gx_brush_default"></a>gx_brush_default
Varsayılan fırçayı ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_brush_default(GX_BRUSH *brush);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli bağlam için fırçayı sistem varsayılan değerine ayarlar.

### <a name="parameters"></a>Parametreler
- **fırça** Fırça denetim bloğu işaretçisi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı fırça tanımı
- **GX_PTR_ERROR** (0x07) geçersiz fırça işaretçisi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/*Reset the brush to its default value. */
status = gx_brush_default(&my_brush);

/* If status is GX_SUCCESS the brush was successfully reset to its default value. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_brush_define


## <a name="gx_brush_define"></a>gx_brush_define
Fırça Tanımla

### <a name="prototype"></a>Prototype

```C
UINT gx_brush_define(
    GX_BRUSH *brush, 
    GX_COLOR line_color, 
    GX_COLOR fill_color, 
    UINT style);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen çizgi rengine, Fill rengine ve stile sahip bir fırça tanımlar.

### <a name="parameters"></a>Parametreler

- **fırça** Fırça denetim bloğu işaretçisi
- **line_color** Fırça hattının rengi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.
- **fill_color** Fırça dolgusunun rengi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.
- **Stil** Fırça stili. **Ek D** desteklenen fırça stillerini açıklar. Fırça stilleri, bit düzeyinde OR işlemi kullanarak bir değişkende birleştirilebilir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı fırça tanımı
- **GX_PTR_ERROR** (0x07) geçersiz fırça işaretçisi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define a brush. */
status = gx_brush_define(&my_brush, GX_COLOR_BLACK, GX_COLOR_BLACK,
                         GX_STYLE_BORDER_NONE);

/* If status is GX_SUCCESS the brush was successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_brush_default

## <a name="gx_button_background_draw"></a>gx_button_background_draw

 Düğme arka planı çiz

###<a name="prototype"></a>Prototype

```C
VOID gx_button_background_draw(GX_BUTTON *button);
```

### <a name="description"></a>Açıklama

Bu hizmet, düğme arka planını çizer. Bu işlev genellikle gx_button_draw işlevi tarafından dahili olarak çağrılır, ancak özel çizim işlevleri yazma konusunda yardımcı olmak için uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **düğme** Düğme denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
VOID custom_button_draw(GX_BUTTON *button)
{
    /* Draw button background. */
    gx_button_background_draw(button);

    /* Add custom drawing here. */

    /* Draw child widgets. */
    gx_widget_children_draw((GX_WIDGET *)button);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_create,
- gx__button_deselect,
- gx__button_draw
- gx_button_event_process,
- gx__button_select
- gx_icon_button_create,
- gx__pixelmap_button_create
- gx_pixelmap_button_draw,
- gx__radio_button_create
- gx_radio_button_draw,
- gx__text_button_create
- gx_text_button_color_set,
- gx__text_button_draw

## <a name="gx_button_create"></a>gx_button_create

Oluştur düğmesi

### <a name="prototype"></a>Prototype

```C
UINT gx_button_create(
    GX_BUTTON *button, 
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent, 
    ULONG style, 
    USHORT button_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen bir düğme oluşturur ve düğmeyi sağlanan üst pencere öğesiyle ilişkilendirir.

### <a name="parameters"></a>Parametreler

- **düğme** Düğme denetim bloğu işaretçisi
- **ad** Düğmenin mantıksal adı
- **üst öğe** Düğmenin üst pencere öğesi işaretçisi
- **Stil** Düğme stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **button_id** Düğmenin uygulama tanımlı KIMLIĞI
- **Boyut** Düğmenin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı düğme oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_BUTTON my_top_button;

/* Create a stop button. */
status = gx_button_create(&my_stop_button, "my stop button",
                            &my_parent_window,
                            GX_STYLE_BUTTON_TOGGLE,
                            MY_STOP_BUTTON_ID, &size);

/* If status is GX_SUCCESS the stop button was successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw,
- gx_button_deselect,
- gx_button_draw
- gx_button_event_process,
- gx_button_select
- gx_radio_button_create,
- gx_radio_button_draw
- gx_icon_button_create,
- gx_pixelmap_button_create
- gx_pixelmap_button_draw,
- gx_text_button_create
- gx_text_button_color_set,
- gx_text_button_draw

## <a name="gx_button_deselect"></a>gx_button_deselect


Seçimi Kaldır düğmesi

### <a name="prototype"></a>Prototype

```C
UINT gx_button_deselect(
    GX_BUTTON *button, 
    GX_BOOL gen_event);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen düğmeyi kaldırır ve düğme stillerine bağlı olarak bir sinyal olayı oluşturur.


| Düğme stili              | Sinyalinin                     |
|---------------------------|----------------------------|
| Yok                      | GX_EVENT_CLICKED         |
| GX_STYLE_BUTTON_RADIO  | GX_EVENT_RADIO_DESELECT |
| GX_STYLE_BUTTON_TOGGLE | GX_EVENT_TOGGLE_OFF     |



### <a name="parameters"></a>Parametreler

- **düğme** Düğme denetim bloğu işaretçisi
- **gen_event** GX_TRUE, düğme, düğme stiline bağlı olarak bir GX_EVENT_CLICKED, GX_EVENT_DESELECT veya GX_EVENT_TOGGLE_OFFSET olayı oluşturacaktır. GX_FALSE, düğme normalde yapabilse bile daha yüksek düzey bir olay oluşturmaz.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı düğme seçimi kaldır
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Deselect button. */
status = gx_button_deselect(&my_stop_button, GX_TRUE);

/* If status is GX_SUCCESS the stop button was successfully deselected. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw,
- gx_button_create,
- gx_button_draw
- gx_button_event_process,
- gx_button_select
- gx_radio_button_create,
- gx_radio_button_draw
- gx_icon_button_create,
- gx_pixelmap_button_create
- gx_pixelmap_button_draw,
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_button_draw"></a>gx_button_draw

Çiz düğmesi

### <a name="prototype"></a>Prototype

```C
VOID gx_button_draw(GX_BUTTON *button);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen düğmeyi çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel düğme pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **düğme** Düğme denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom button draw function. */
VOID custom_button_draw(GX_BUTTON *button)
{
    /* Call default button draw. */
    gx_button_draw(button);

    /* Add custom drawing here. */
}

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw,
- gx_button_create
- gx_button_deselect,
- gx_button_event_process,
- gx_button_select
- gx_radio_button_create,
- gx_radio_button_draw
- gx_icon_button_create,
- gx_pixelmap_button_create
- gx_pixelmap_button_draw,
- gx_text_button_create
- gx_text_button_color_set,
- gx_text_button_draw

## <a name="gx_button_event_process"></a>gx_button_event_process


İşlem düğmesi olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_button_event_process(
    GX_BUTTON *button, 
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen düğme için bir olayı işler.

### <a name="parameters"></a>Parametreler

- **düğme** Düğme denetim bloğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı düğme olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic button event processing as part of custom event processing function. */

UINT custom_button_event_process(GX_BUTTON *button,
                                 GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;
    default:
        /* Pass all other events to the default button
            event processing */
        status = gx_button_event_process(button, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw,
- gx_button_create
- gx_button_deselect,
- gx_button_draw,
- gx_button_select
- gx_radio_button_create,
- gx_radio_button_draw
- gx_icon_button_create,
- gx_pixelmap_button_create
- gx_pixelmap_button_draw,
- gx_text_button_create
- gx_text_button_color_set,
- gx_text_button_draw

## <a name="gx_button_select"></a>gx_button_select

Düğme Seç

### <a name="prototype"></a>Prototype

```C
UINT gx_button_select(GX_BUTTON *button);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen düğmeyi seçer ve düğme stillerine bağlı olarak bir sinyal olayı oluşturur.

Radyo düğmesi grubu için eşdüzey öğeleri kaldırır.

| Düğme stili                       | Sinyalinin                   |
|------------------------------------|--------------------------|
| GX_STYLE_BUTTON_RADIO           | GX_EVENT_RADIO_SELECT |
| GX_STYLE_BUTTON_EVENT_ON_PUSH | GX_EVENT_CLICKED       |
| GX_STYLE_BUTTON_TOGGLE          | GX_EVENT_TOGGLE_ON    |


### <a name="parameters"></a>Parametreler

- **düğme** Düğme denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı düğme seçme
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Select button. */
status = gx_button_select(&my_stop_button);

/* If status is GX_SUCCESS the stop button was successfully selected. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw,
- gx_button_create
- gx_button_deselect,
- gx_button_draw,
- gx_button_event_process
- gx_radio_button_create,
- gx_radio_button_draw
- gx_icon_button_create,
- gx_pixelmap_button_create
- gx_pixelmap_button_draw,
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_canvas_alpha_set"></a>gx_canvas_alpha_set

Tuval için alfa Blend değeri ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_alpha_set(
    GX_CANVAS *canvas, 
    GX_UBYTE alpha);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen tuval için alfa Blend değerini ayarlar. Tuval alfa değerleri 0 (saydam) ile 255 (tamamen donuk) arasında değişebilir.

Birleşik kaplama canvalarını karıştırma, bir bileşik tuval oluşturma yoluyla donanım grafik katmanı desteği veya yazılım desteği gerektirir.

Tuval Alpha değeri ayarlamadan önce gx_canvas_hardware_layer_bind () API 'sini çağırarak tuval karışımı için donanım desteği etkinleştirilir. Bir tuval bir donanım grafik katmanına bağlandığında, gx_canvas_alpha_set () API 'sini çağırmak doğrudan donanım grafik katmanı karıştırma hizmetlerini çağırır.

Uygulama, tuval karıştırma için yazılım desteğini kullanmak amacıyla, tüm diğer yönetilen canların son görüntü öncesinde oluşturulduğu GX_CANVAS_COMPOSITE stiliyle bir tuval oluşturması gerekir. Tuval karıştırma için yazılım desteği yalnızca 16 BPP veya daha yüksek renk derinliğinde bir ekran sürücüsüyle çalışırken sağlanır.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi
- **Alfa** Alfa Blend değeri, 0 (saydam) ile 255 (donuk) arasındadır.

### <a name="return--values"></a>Dönüş değerleri

- **GX_SUCCESS** (0x00) başarılı Alfa Blend değer kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_ERROR** (0x20) geçersiz tuval

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the alpha-blend value of “my_canvas”. */
status = gx_canvas_alpha_set(&my_canvas, GX_ALPHA_VALUE_OPAQUE);

/* If status is GX_SUCCESS the alpha-blend value was successfully set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_create,
- gx_canvas_drawing_complete
- gx_canvas_drawing_initiate,
- gx_canvas_offset_set
- gx_canvas_shift,
- gx_canvas_hardware_layer_bind,
- gx_canvas_show
- gx_canvas_hide

## <a name="gx_canvas_arc_draw"></a>gx_canvas_arc_draw

Yay çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_arc_draw(
    INT xcenter, 
    INT ycenter, 
    UINT r,
    INT start_angle, 
    INT end_angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli fırçayı kullanarak tuvalde bir daire yay çizer. Daire yay tuvalde geçersiz bölge olarak kırpıldı. Bu hizmet için GX_ARC_DRAWING_SUPPORT tanımlanması gerekir.

### <a name="parameters"></a>Parametreler

- daire yay merkezinin **xcenter** x konumu
- **yılmerkez** y-daire yay merkezinin konumu
- Daire yaya **r** yarıçapı
- **start_angle** Daire yay başlangıç açısı
- **end_angle** Daire yay bitiş açısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yay çizimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_VALUE** (0x22) geçersiz değer
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw a circle arc from 0 degree to 90 degree in clockwise. */
status = gx_canvas_arc_draw(100, 100, 50, 0, 90);

/* If status is GX_SUCCESS the arc has been drawn on “my_canvas”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_block_move,
- gx_canvas_circle_draw
- gx_display_create,
- gx_canvas_ellipse_draw
- gx_canvas_line_draw,
- gx_canvas_pie_draw
- gx_canvas_pixelmap_draw,
- gx_canvas_pixelmap_tile
- gx_canvas_polygon_draw
- gx_canvas_rectangle_draw,
- gx_canvas_text_draw

## <a name="gx_canvas_block_move"></a>gx_canvas_block_move

Tuval piksel bloğunu taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_block_move(GX_RECTANGLE *block,
    GX_VALUE x_shift, GX_VALUE y_shift, GX_RECTANGLE *dirty);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir tuval piksel verisi bloğunu belirtilen yönde taşır. Bu hizmet, hızlı kaydırma gerçekleştirmek üzere Gux tarafından dahili olarak kullanılır, ancak uygulama yazılımı tarafından da kullanılabilir.

### <a name="parameters"></a>Parametreler

- **blok** Taşınacak alanın koordinatları
- **x_shift** X ekseninde kaydırma yapılacak piksel sayısı
- **y_shift** Y ekseninde kaydırma yapılacak piksel sayısı
- **kirli** Blok taşıma başarılı olursa, bu işlev kaynak dikdörtgenin bu parametresindeki çağırana hala kirli olan bölümünü döndürür.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı blok taşıma
- **GX_FAILURE** (0x10) başarısız blok taşıma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
GX_RECTANGLE invalid;
GX_RECTANGLE move;

/* define 100 x 100 pixel rectangle */
gx_utility_rectangle_define(&move, 0, 0, 99, 99);

/* Move this rectangle 10 pixels to the right”. */
status = gx_canvas_block_move(&move, 10, 0, &invalid);

/* If status is GX_SUCCESS, then ‘invalid’ marks the area that needs to be redrawn after the block move. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_arc_draw,
- gx_canvas_circle_draw,
- gx_display_create
- gx_canvas_ellipse_draw,
- gx_canvas_line_draw
- gx_canvas_pie_draw,
- gx_canvas_pixelmap_draw
- gx_canvas_pixelmap_tile,
- gx_canvas_polygon_draw
- gx_canvas_rectangle_draw,
- gx_canvas_text_draw

## <a name="gx_canvas_circle_draw"></a>gx_canvas_circle_draw

Daire çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_circle_draw(
    INT xcenter, 
    INT ycenter, 
    UINT r);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli fırçayı kullanarak tuvalde bir daire çizer. Daire tuval için geçersiz bölgeye kırpıldı. Bu hizmet için GX_ARC_DRAWING_SUPPORT tanımlanması gerekir.

### <a name="parameters"></a>Parametreler

- Dairenin ortasında **xcenter** x-cozı
- **incenter** y-cirof dili
- dairenin **r** yarıçapı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı daire çiz
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_VALUE** (0x22) geçersiz daire yarıçapı
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C

/* Draw a circle of radius 10 centered at (100, 100). */
status = gx_canvas_circle_draw(100, 100, 50);

/* If status is GX_SUCCESS the circle has been drawn on “my_canvas”. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_arc_draw,
- gx_canvas_block_move,
- gx_display_create
- gx_canvas_ellipse_draw,
- gx_canvas_line_darw
- gx_canvas_pie_draw,
- gx_canvas_pixelmap_draw
- gx_canvas_pixelmap_tile,
- gx_canvas_polygon_draw
- gx_canvas_rectangle_draw,
- gx_canvas_text_draw


## <a name="gx_canvas_create"></a>gx_canvas_create

Tuval oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_create(
    GX_CANVAS *canvas, 
    GX_CONST GX_CHAR *name,
    GX_DISPLAY *display, 
    UINT type, 
    UINT width, 
    UINT height,
    GX_COLOR *memory_area, 
    ULONG memory_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen özelliklerle ve ilişkili bellekle tuvalde oluşturur.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi
- **ad** Tuval için mantıksal ad
- **görüntüleme** Önceden oluşturulmuş görüntü işaretçisi
- **tür** Canvau tuval türlerinin türü şunları içerir:
- **GX_CANVAS_SIMPLE:** Ekran çizimini devre dışı bırakmak için kullanılan bir bellek tuvali.
- **GX_CANVAS_MANAGED:** Bileşik yapı sürecinin bir parçası olarak veya tek tuvalli mimarilere yönelik arabellek geçiş işleminin bir parçası olarak etkin ekranı otomatik olarak temizlenen bir tuval.
- **GX_CANVAS_VISIBLE:** Bu bayrak tuval çizim içeriğini kaybetmeden bir tuvali açmak ve kapatmak için kullanılabilir.
- **GX_CANVAS_MODIFIED:** Gelecekte kullanılmak üzere ayrılmıştır.
- **GX_CANVAS_COMPOSITE:** Bu bayrak, birden çok yönetilen ve bileşik tuvalde bileşik bir sistem olan birden çok tuval sistemi yapılandırırken uygulama tarafından kullanılır ve bileşik donanım çerçeve arabelleğine dayalıdır.
- **Genişlik** Piksel cinsinden genişlik
- **Yükseklik** Piksel cinsinden yükseklik
- **memory_area** Tuval için bellek alanı. Bu değer,
- Tuval oluşturma sırasında **GX_NULL**
- **ve** daha sonra gx_canvas_memory_define kullanılarak başlatıldı
- **memory_size** Tuval oluşturulduktan sonra tuval belleği tanımlıysa, bayt cinsinden bellek alanının boyutu veya 0.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tuval oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_CANVAS_SIZE** (0x1C) geçersiz tuval denetimi blok boyutu
- **GX_INVALID_TYPE** (0x1B) geçersiz tuval türü

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define global canvas memory area. */
GX_COLOR my_canvas_memory[272*480];

…

/* Create “my_canvas”. */
status = gx_canvas_create(&my_canvas, "my canvas", &my_display,
                    (GX_CANVAS_MANAGED | GX_CANVAS_VISIBLE),
                    272, 480,
                    my_canvas_memory,
                    sizeof(default_canvas_memory));

/* If status is GX_SUCCESS the 272 x 480 canvas was successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_delete,
- gx_canvas_hardware_layer_bind
- gx_canvas_memory_define

## <a name="gx_canvas_delete"></a>gx_canvas_delete

Tuvali Sil

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_delete(GX_CANVAS *canvas);
```

### <a name="description"></a>Açıklama

Bu hizmet tuvali siler. Tuval, GUıDX tarafından tutulan iç bağlantılı tuval listesinden kaldırılır.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tuval oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CANVAS** (0x20) geçersiz tuval

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Delete “my_canvas”. */
status = gx_canvas_delete (&my_canvas);

/* If status is GX_SUCCESS my_canvas was deleted. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_alpha_set,
- gx_canvas_drawing_complete
- gx_canvas_create,
- gx_canvas_drawing_initiate
- gx_canvas_offset_set,
- gx_canvas_shift

## <a name="gx_canvas_drawing_complete"></a>gx_canvas_drawing_complete

Tuval çizimini tamamen doldurun

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_drawing_complete(
    GX_CANVAS *canvas, 
    GX_BOOL flush);
```

### <a name="description"></a>Açıklama

Bu hizmet, Gux 'in belirtilen tuvalde uygulama çiziminin tamamlandığını bilmesini sağlar.

Uygulama bu hizmeti kullanarak tuvalde hemen çizim yapılmasını zorlayabilir. Bu, tuvali görünür çerçeve arabelleğine boşaltır ve/veya sistem belleği mimarisine bağlı olarak bir hata atma geçiş işlemi tetikler.

Bu hizmet yalnızca uygulama tarafından, gx_canvas_drawing_initiate () ile başlatılan bir çizim dizisinin kapatılmasını sağlamak için çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi
- **Temizleme** **_GX_TRUE_**, tuval değişiklikleri ekranda temizlenir

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çizim tamamlama
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Complete drawing on “my_canvas” and flush to display. */
status = gx_canvas_drawing_complete(&my_canvas, GX_TRUE);

/* If status is GX_SUCCESS the canvas drawing was successfully completed. */
```


### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_alpha_set,
- gx_canvas_create
- gx_canvas_drawing_initiate,
- gx_canvas_offset_set
- gx_canvas_shift

## <a name="gx_canvas_drawing_initiate"></a>gx_canvas_drawing_initiate

Tuval çizimini Başlat

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_drawing_initiate(
    GX_CANVAS *canvas,
    GX_WIDGET *who, 
    GX_RECTANGLE *dirty_area);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen tuvalde çizim başlatır. Bu hizmet, bir tuvalin güncelleştirilmesi gerektiğinde Gux tarafından otomatik olarak gerçekleştirilen ertelenmiş çizim işleminin bir parçası olarak dahili olarak çağrılır. Bununla birlikte, uygulamanın Gux ertelenmiş çizim algoritmasını atlayıp, önce gx_canvas_drawing_inititate çağırarak ve sonra istenen çizim işlevlerini çağırarak ve sonra da gx_canvas_drawing_complete () çağırarak bir tuvalde anında ve doğrudan çizim yapmaya izin verilir.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi
- **kim** Çağıranın pencere öğesi denetim bloğuna yönelik işaretçi. Bu parametre, çizim kırpmasını başlatmak ve sonraki çizim işlemlerine yönelik parametreleri görüntülemek için kullanılır.
- **dirty_area** İçinde çizilecek alan. Bu parametre çağıran tarafından çağıranın tüm çizim işlemlerinin kırpıldığı alanı belirtmek için geçirilir. Bu genellikle daha önce kirli olarak işaretlenen alandır, ancak çağıran kırpma alanını genişletmek veya sözleşmeye göre ücretsizdir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarıyla çizim başlatma
- **GX_DRAW_NESTING_EXCEEDED** (0x05) iç içe geçme sayısı üst sınırını aşıyor
- **GX_NO_VIEW** (0x03) arayan için Viewport yok
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CANVAS** (0x20) geçersiz tuval

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Initiate drawing on “my_canvas”, my_widget.gx_widget_size
specify the area the application wants GUIX to redraw. */
status = gx_canvas_drawing_initiate(&my_canvas, &my_widget,
    &my_widget.gx_widget_size);

/* If status is GX_SUCCESS the canvas drawing was successfully initiated. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_alpha_set,
- gx_canvas_create
- gx_canvas_drawing_complete,
- gx_canvas_offset_set
- gx_canvas_shift


## <a name="gx_canvas_ellipse_draw"></a>gx_canvas_ellipse_draw

Elips çizme

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_ellipse_draw(
    INT xcenter, 
    INT ycenter, 
    INT a, 
    dINT b);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli fırçayı kullanarak tuvalde bir elips çizer. Elips tuval için geçersiz bölgeye kırpıldı. Bu hizmet için GX_ARC_DRAWING_SUPPORT tanımlanması gerekir.

### <a name="parameters"></a>Parametreler

- Elips merkezinin **xcenter** x-cozı
- Elips merkezinin **Orta ortası**
- yarı birincil **eksenin uzunluğu**
- **b** yarı küçük eksenin uzunluğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı daire çiz
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_VALUE** (0x22) geçersiz değer
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw an ellipse of semi-major radius 100, semi-minor radius 50
    and centered at (200, 200). */
status = gx_canvas_ellipse_draw(200, 200, 100, 50);

/* If status is GX_SUCCESS the ellipse has been drawn on
    “my_canvas”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_arc_draw,
- gx_canvas_block_move
- gx_canvas_circle_draw,
- gx_display_create,
- gx_canvas_line_darw
- gx_canvas_pie_draw,
- gx_canvas_pixelmap_draw
- gx_canvas_pixelmap_tile,
- gx_canvas_polygon_draw
- gx_canvas_rectangle_draw,
- gx_canvas_text_draw

## <a name="gx_canvas_hardware_layer_bind"></a>gx_canvas_hardware_layer_bind

Tuvali donanım grafik katmanına bağlama

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_hardware_layer_bind(
    GX_CANVAS *canvas, 
    INT layer);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir Gux çizim tuvalini bir donanım grafik katmanına bağlar. Bu hizmet yalnızca birden çok donanım grafik katmanını destekleyen donanım cihazları için gereklidir.

Bir tuvali bir donanım grafik katmanına bağlamak, donanım görüntü sürücüsü Hizmetleri tarafından doğrudan uygulanan gx_canvas_show (), gx_canvas_hide (), gx_canvas_alpha_set () ve gx_canvas_offset_set () API 'Lerinin sonucunu elde ediyor.

Donanım görüntü sürücüsü birden çok grafik katmanını desteklemiyorsa, bu hizmet GX_INVALID_DISPLAY döndürmeyecektir.

### <a name="parameters"></a>Parametreler

- donanımda uygulanacak **tuval** tuvali
- **Katman** donanımı grafik katmanı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlama
- **GX_INVALID_DISPLAY** (0x1d) görüntüleme katmanı hizmeti tanımlı değil
- **GX_PTR_ERROR** (0x17) geçersiz işaretçiler
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_CANVAS** (0x20) geçersiz tuval
- **GX_NOT_SUPPORTED** (0x28) desteklenmez

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Binds the canvas to the hardware graphics layer 1. */
status = gx_canvas_hardware_layer_bind(&my_canvas, 1);

/* If status is GX_SUCCESS, the drawing canvas is bound to the
    hardware graphics. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_create,
- gx_canvas_memory_define

## <a name="gx_canvas_hide"></a>gx_canvas_hide

Tuvali gizleme, görünmez hale getirme

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_hide(GX_CANVAS *canvas);
```

### <a name="description"></a>Açıklama

Bu hizmet bir Gux tuvali gizler. Tuval, gx_canvas_hardware_layer_bind () kullanılarak bir donanım grafik katmanına bağlanmışsa, bu hizmet donanım desteği kullanılarak uygulanır.

### <a name="parameters"></a>Parametreler

- **tuval** tuvali gizli olacak şekilde

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı gizleme
- **GX_INVALID_CANVAS** (0x20) geçersiz tuval
- **GX_PTR_ERROR** (0x17) geçersiz işaretçiler
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Make my_canvas invisible. */
status = gx_canvas_hide(&my_canvas);

/* If status is GX_SUCCESS, the canvas has been hidden. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_create,
- gx_canvas_drawing_complete
- gx_canvas_drawing_initiate,
- gx_canvas_offset_set
- gx_canvas_shift,
- gx_canvas_hardware_layer_bind,
- gx_canvas_show
- gx_canvas_hide

## <a name="gx_canvas_line_draw"></a>gx_canvas_line_draw

Çizgi çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_line_draw(
    GX_VALUE x_start, 
    GX_VALUE y_start,
    GX_VALUE x_end, 
    GX_VALUE y_end);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli fırçayı kullanarak tuvalde bir çizgi çizer. Çizgi, tuval geçersiz bölgesine kırpıldı.

### <a name="parameters"></a>Parametreler

- **x_start** Çizginin x konumu başlatılıyor
- **y_end** Satırın y konumu başlatılıyor
- **x_start** Çizginin x konumunu sonlandırma
- **y_end** Satırın y konumu bitiriliyor

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çizgi çiz
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok
- **GX_INVALID_WIDTH** (0x1E) geçersiz fırça genişliği

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw line on canvas. */
status = gx_canvas_line_draw(0, 1, 320, 480);

/* If status is GX_SUCCESS, the line has been drawn to canvas. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_arc_draw,
- gx_canvas_block_move
- gx_canvas_circle_draw,
- gx_display_create
- gx_canvas_ellipse_draw,
- gx_canvas_pie_draw
- gx_canvas_pixelmap_draw,
- gx_canvas_pixelmap_tile
- gx_canvas_polygon_draw,
- gx_canvas_rectangle_draw
- gx_canvas_text_draw

## <a name="gx_canvas_memory_define"></a>gx_canvas_memory_define

Tuval belleğini tanımlama

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_memory_define(
    GX_CANVAS *canvas, 
    GX_COLOR *memory,
    ULONG memsize);
```

### <a name="description"></a>Açıklama

Bu hizmet, tuval oluşturulduktan sonra tuval bellek adresini atamak için kullanılabilir.

### <a name="parameters"></a>Parametreler

- **tuval** Daha önce oluşturulmuş tuval işaretçisi
- **bellek** Tuval bellek adresi
- **memsize** Tuval bellek bloğunun bayt cinsinden boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı atama
- **GX_INVALID_CANVAS** (0x20) geçersiz denetim bloğu
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Assign canvas memory block. */
status = gx_canvas_memory_define(canvas,
    (GX_COLOR *) DRAM_MEMORY,
    (640 * 480 * 2));

/* If status is GX_SUCCESS, the canvas memory pointer has be
reassigned. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_create,
- gx_canvas_hardware_layer_bind

## <a name="gx_canvas_mouse_define"></a>gx_canvas_mouse_define

Fare imleç resmini tanımlama

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_mouse_define(GX_CANVAS *canvas,
    GX_MOUSE_CURSOR_INFO *info);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen tuval için fare bilgilerini tanımlar. Bu hizmet için GX_MOUSE_SUPPORT tanımlanması gerekir.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi
- **bilgi** Fare imleç bilgilerine yönelik işaretçi. **Ek ı** GX_MOUSE_CURSOR_INFO yapısına yönelik tanımı içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı fare bilgi kümesi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set mouse cursor info. */
GX_MOUSE_CURSOR_INFO mouse_cursor;
mouse_cursor.gx_mouse_cursor_image_id = GX_PIXELMAP_ID_MOUSE;
mouse_cursor.gx_mouse_cursor_hotspot_x = 0;
mouse_cursor.gx_mouse_cursor_hotspot_y = 0;

status = gx_canvas_mouse_define(&my_canvas, &mouse_cursor);

/* If status is GX_SUCCESS the mouse info of “my_canvas” has been
set successfully. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_mouse_show,
- gx_canvas_mouse_hide

## <a name="gx_canvas_mouse_hide"></a>gx_canvas_mouse_hide


Fare imlecini kapat

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_mouse_hide(GX_CANVAS *canvas);
```

### <a name="description"></a>Açıklama

Bu hizmet, fare imlecini belirtilen tuvalden gizli hale getirir. Bu hizmet için GX_MOUSE_SUPPORT tanımlanması gerekir.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı fare imleci gizle
- **GX_FAILURE** (0x10) fare Imleci gizleme başarısız oldu
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran


### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Hide the mouse cursor. */
status = gx_canvas_mouse_hide(&my_canvas);

/* If status is GX_SUCCESS the mouse cursor of “my_canvas” has been
hidden successfully. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_mouse_show,
- gx_canvas_mouse_define

## <a name="gx_canvas_mouse_show"></a>gx_canvas_mouse_show


Fare imlecini aç

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_mouse_show(GX_CANVAS *canvas);
```

### <a name="description"></a>Açıklama

Bu hizmet, fare imlecini belirtilen tuval için görünür hale getirir. Bu hizmet için GX_MOUSE_SUPPORT tanımlanması gerekir. Bu hizmet istenmediği için fare imleci görüntüsünü tanımlamak üzere gx_canvas_mouse_define API çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı fare bilgi kümesi
- **GX_FAILURE** (0x10) fare Imlecinin gösterilmesi başarısız oldu
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Make mouse cursor hidden ”. */
status = gx_canvas_mouse_show(&my_canvas);

/* If status is GX_SUCCESS the mouse of “my_canvas” has been
hidden successfully. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_mouse_show,
- gx_canvas_mouse_define

## <a name="gx_canvas_offset_set"></a>gx_canvas_offset_set


Tuval x, y görüntüleme boşluğu ata

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_offset_set(
    GX_CANVAS *canvas,
    GX_VALUE x, 
    GX_VALUE y);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen tuval için bir x, y görüntüleme boşluğu atar. Bu, tuvalin görünür çerçeve arabelleğine yerleştirme konumunu denetler ve genellikle tuval fiziksel görünenden küçük olduğunda kullanılır.

Tuval, gx_canvas_hardware_layer_bind () API 'sini kullanarak bir donanım grafik katmanına bağlanmışsa, gx_canvas_offset_set hizmeti doğrudan donanım desteği kullanılarak uygulanır.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi
- **x** x konum koordinatı
- uzaklığa göre **y** y koordinatı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı Aralık ataması
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CANVAS** (0x20) geçersiz tuval

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set display offset for “my_canvas”. */
status = gx_canvas_offset_set(&my_canvas, 20, 30);

/* If status is GX_SUCCESS the canvas drawing is now offset from
position 20,30. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_alpha_set,
- gx_canvas_create
- gx_canvas_drawing_complete,
- gx_canvas_initiate,
- gx_canvas_shift
- gx_canvas_show,
- gx_canvas_hide,
- gx_canvas_hardware_layer_bind

## <a name="gx_canvas_pie_draw"></a>gx_canvas_pie_draw


Pasta çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_pie_draw(
    INT xcenter, 
    INT ycenter,
    UINT r, 
    INT start_angle, 
    INT end_angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamı fırçasını kullanarak tuvalde bir pasta çizer. Pasta tuval için geçersiz bölgeye kırpıldı. Bu hizmet, GX_ARC_DRAWING_SUPPORT yapılandırma seçeneğinin tanımlanmasını gerektirir.

### <a name="parameters"></a>Parametreler

- pasta merkezinin **xcenter** x konumu
- **yılmerkez** y-pasta merkezinin konumu
- Pastanın **r** yarıçapı
- **start_angle** Pastanın başlangıç açısı
- **end_angle** Pastanın bitiş açısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yay çizimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_VALUE** (0x22) geçersiz değer
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw a pie from 0 degree to 90 degree in clockwise. */
status = gx_canvas_pie_draw(100, 100, 50, 0, 90);

/* If status is GX_SUCCESS the pie has been drawn to canvas. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_arc_draw,
- gx_canvas_block_move
- gx_canvas_circle_draw,
- gx_display_create
- gx_canvas_ellipse_draw,
- gx_canvas_line_draw
- gx_canvas_pixelmap_draw,
- gx_canvas_pixelmap_tile
- gx_canvas_polygon_draw,
- gx_canvas_rectangle_draw
- gx_canvas_text_draw

## <a name="gx_canvas_pixel_draw"></a>gx_canvas_pixel_draw


Piksel çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_pixel_draw(GX_POINT position);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamı fırçasının çizgi rengini kullanarak tuvalde bir piksel çizer. Yapılandırma seçeneği GX_BRUSH_ALPHA_SUPPORT tanımlanmışsa, pikseli, tersi şekilde Blend, piksel tamamen opak olarak çizin.

- **noktanın** x, y konumunu çizmek için

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pixelmap çizimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_POINT point; /* the x,y position you want to draw to */
GX_RECTANGLE drawto; /* the rectangle bounding your drawing */
GX_CANVAS *mycanvas; /* the canvas you want to draw to */

/* calculate 1x1 pixel drawing area: */
gx_utility_rectangle_define(&drawto,
    point.gx_point_x, point.gx_point_y,
    point.gx_point_x, point.gx_point_y);

/* get my canvas: */
gx_widget_canvas_get(win, &mycanvas);

/* open my canvas for drawing: */
gx_canvas_drawing_initiate(mycanvas, win, &drawto);

/* setup my brush colors. Use any color ID in your resources: */
gx_context_line_color_set(GX_COLOR_ID_WINDOW_BORDER);

/* draw a pixel: */
status = gx_canvas_pixel_draw(point);

/* close the canvas: */
gx_canvas_drawing_complete(mycanvas, GX_TRUE);

/* If status is GX_SUCCESS, the pixel was successfully drawn to mycanvas. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_block_move,
- gx_canvas_pixelmap_tile
- gx_canvas_pixelmap_blend

## <a name="gx_canvas_pixelmap_blend"></a>gx_canvas_pixelmap_blend

Blend, pixelmap

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_pixelmap_blend(
    GX_VALUE x_position,
    GX_VALUE y_position, 
    GX_PIXELMAP *pixelmap, 
    GX_UBYTE alpha);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir pixelmap 'i tuval arka planıyla karıştırır. Karıştırma oranı çağıran tarafından belirtilir. Alfa değeri 0 (tamamen saydam) ile 255 (tamamen opak) arasında değişebilir. Pixelmap Ayrıca, gelen karıştırma değeriyle birleştirilmiş bir iç alfa kanalını da içerebilir. Bu hizmet yalnızca 16 BPP renk derinliği ve üzeri sürümlerde çalışan ekran sürücüleri tarafından desteklenir.

### <a name="parameters"></a>Parametreler

- **x_start** Pixelmap 'in x-Position ' i başlatılıyor
- **y_end** Pixelmap 'in y konumu başlatılıyor
- **pixelmap** Pixelmap işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pixelmap çizimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_NOT_SUPPORTED** (0x28) desteklenmez
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw pixelmap on active canvas */

GX_PIXELMAP *map;
gx_system_pixelmap_get(ID_MY_PIXELMAP, &map);

status = gx_canvas_pixelmap_blend(10, 20, map, 128);

/* If status is GX_SUCCESS the pixelmap has been blended onto the current canvas. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_block_move,
- gx_canvas_pixelmap_get
- gx_canvas_pixelmap_tile
- gx_canvas_pixelmap_draw

## <a name="gx_canvas_pixelmap_draw"></a>gx_canvas_pixelmap_draw

Pixelmap çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_pixelmap_draw(
    GX_VALUE x_position, 
    GX_VALUE y_position,
    GX_PIXELMAP *pixelmap);
```

### <a name="description"></a>Açıklama

Bu hizmet, tuvalde bir pixelmap çizer.

### <a name="parameters"></a>Parametreler

- **x_start** Pixelmap 'in x-Position ' i başlatılıyor
- **y_end** Pixelmap 'in y konumu başlatılıyor
- **pixelmap** Pixelmap işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pixelmap çizimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw pixelmap on canvas. */
status = gx_canvas_pixelmap_draw(10, 20, &my_pixelmap);

/* If status is GX_SUCCESS the pixelmap “my_pixelmap” has been drawn. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_block_move,
- gx_canvas_pixelmap_get
- gx_canvas_pixelmap_tile
- gx_canvas_pixelmap_blend

## <a name="gx_canvas_pixelmap_get"></a>gx_canvas_pixelmap_get

Tuval pixelmap 'i al

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_pixelmap_get(GX_PIXELMAP *pixelmap);
```

### <a name="description"></a>Açıklama

Bu hizmet, tuval verilerine işaret eden bir GX_PIXELMAP yapısı döndürür. Pixelmap biçimi geçerli görüntüleme rengi biçimine ayarlanır.

### <a name="parameters"></a>Parametreler

- **pixelmap** Döndürülen pixelmap

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pixelmap al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw pixelmap on active canvas */

GX_PIXELMAP *map;

status = gx_canvas_pixelmap_get(map);

/* If status is GX_SUCCESS the pixelmap has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_pixelmap_blend,
- gx_canvas_pixelmap_tile
- gx_canvas_pixelmap_draw

## <a name="gx_canvas_pixelmap_rotate"></a>gx_canvas_pixelmap_rotate


Döndürülen pixelmap 'i çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_pixelmap_rotate(
    GX_VALUE x_position, 
    GX_VALUE y_position,
    GX_PIXELMAP *pixelmap, 
    INT angle,
    INT rot_cx, 
    INT rot_cy);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen açıyla bir pixelmap döndürür ve döndürme gerçekleştirildiğinde doğrudan bir pixelmap 'i tuvale işler. Bu hizmet, döndürme çıktısının doğrudan tuval belleğine işlendiğine ve döndürülen pixelmap 'in çağırana döndürüldüğünden gx_utility_pixelmap_rotate farklıdır.

Bu hizmetin gx_utility_pixelmap_rotate üzerinden avantajı, döndürülen pixelmap 'i barındırmak için ek bellek gerektirmeyecek. Dezavantajı, her pixelmap çizililişinde döndürme kodunun yürütülmesi gerekir.

Kırpma ve Görünüm penceresi doğrulama, döndürülen pixelmap 'in işlenmesi sırasında zorlanır.

### <a name="parameters"></a>Parametreler

- **x_position** Pixelmap 'in x-Position ' i başlatılıyor
- **y_position** Pixelmap 'in y konumu başlatılıyor
- **pixelmap** Pixelmap işaretçisi
- **açı** Döndürme açısı
- **rot_cx** Döndürme merkezinin X-cozı. Bu değer-1 olarak ayarlanırsa, görüntünün Merkezi döndürme merkezi olarak kullanılır.
- **rot_cy** Dönüş merkezinin Y-cozı. Bu değer-1 olarak ayarlanırsa, görüntünün Merkezi döndürme merkezi olarak kullanılır.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pixelmap çizimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* rotate “src_pixelmap” by 30 degree in clockwise direction and draw in on canvas. */
status = gx_canvas_pixelmap_rotate(10, 20, &my_pixelmap, 30,
    -1, -1);

/* If status is GX_SUCCESS the rotated pixelmap “my_pixelmap” has been drawn. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_block_move,
- gx_canvas_pixelmap_get
- gx_canvas_pixelmap_tile,
- gx_canvas_pixelmap_blend

## <a name="gx_canvas_pixelmap_tile"></a>gx_canvas_pixelmap_tile

Kutucuk pixelmap

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_pixelmap_tile(
    GX_RECTANGLE *fill,
    GX_PIXELMAP *pixelmap);
```

### <a name="description"></a>Açıklama

Bu hizmet, istenen pixelmap ile tuval içindeki bir dikdörtgeni doldurur.

### <a name="parameters"></a>Parametreler

- **doldur** Pixelmap ile döşeme alanı
- **pixelmap** Pixelmap işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pixelmap kutucuğu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok
- **GX_INVALID_VALUE** (0x22) geçersiz Fill boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Tile pixelmap on canvas */
status = gx_canvas_pixelmap_tile(&tile_area, &my_pixelmap);

/* If status is GX_SUCCESS the pixelmap “my_pixelmap” has been tiled on canvas */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_block_move,
- gx_canvas_pixelmap_get
- gx_canvas_pixelmap_blend,
- gx_canvas_pixelmap_draw

## <a name="gx_canvas_polygon_draw"></a>gx_canvas_polygon_draw


Çokgen Çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_polygon_draw(
    GX_POINT *point_array,
    INT number_of_points);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamı fırçasını kullanarak tuvalde bir çokgen çizer.

### <a name="parameters"></a>Parametreler

- **point_array** Poligonun noktaları dizisi
- **number_of_points** Çokgen noktası sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı Çokgen Çiz
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_POINT my_polygon[4] =
{
    { 208, 63 },
    { 274, 63 },
    { 274, 163 },
    { 208, 163 }
};

/* Draw polygon “my_polygon” on canvas. */
status = gx_canvas_polygon_draw(&my_polygon, 4);

/* If status is GX_SUCCESS the polygon “my_polygon” has been drawn. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_arc_draw,
- gx_canvas_block_move
- gx_canvas_circle_draw,
- gx_display_create
- gx_canvas_ellipse_draw,
- gx_canvas_line_draw
- gx_canvas_pie_draw,
- gx_canvas_pixelmap_draw
- gx_canvas_pixelmap_tile,
- gx_canvas_rectangle_draw
- gx_canvas_text_draw

## <a name="gx_canvas_rectangle_draw"></a>gx_canvas_rectangle_draw


Dikdörtgen çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_rectangle_draw(GX_RECTANGLE *rectangle);
```

### <a name="description"></a>Açıklama

Bu hizmet, tuvalde bir dikdörtgen çizer.

### <a name="parameters"></a>Parametreler

- **dikdörtgen** Çizilecek dikdörtgen

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı dikdörtgen çiz
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw rectangle “my_rectangle” on canvas. */
status = gx_canvas_rectangle_draw(&my_rectangle);

/* If status is GX_SUCCESS the rectangle “my_rectangle” has been drawn. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_arc_draw,
- gx_canvas_block_move
- gx_canvas_circle_draw,
- gx_display_create
- gx_canvas_ellipse_draw,
- gx_canvas_line_draw
- gx_canvas_pie_draw,
- gx_canvas_pixelmap_draw
- gx_canvas_pixelmap_tile,
- gx_canvas_polygon_draw
- gx_canvas_text_draw

## <a name="gx_canvas_rotated_text_draw"></a>gx_canvas_rotated_text_draw


Bir orta nokta ile döndürülen metin çiz (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_rotated_text_draw(
    const GX_CHAR *text,
    GX_VALUE xCenter, 
    GX_VALUE yCenter, 
    INT angle);
```

### <a name="description"></a>Açıklama

Bu API kullanım dışı bırakıldı veya gx_canvas_rotated_text_draw_ext (). Hala desteklenirken, yeni uygulamalar bu API 'YI kullanmamalıdır ve bunun yerine gx_canvas_rotated_text_draw_ext () kullanmalıdır.

Bu hizmet, tuvale metin çizer. Metin, istenen merkez noktası hakkında döndürülmüş olarak çizilir. Metni işlemek için geçerli çizim bağlamı yazı tipi ve çizim bağlam çizgisi rengi kullanılır.

Bu hizmet, metin dizesini yalnızca alfa değeri içeren geçici bir 8bpp pixelmap 'e işlemek için gx_utility_string_to_alphamap işlevini kullanır. Daha sonra hizmet, gx_utility_pixelmap_rotate işlevini kullanarak harflerden eşlemeyi döndürür. Son alfamap tuvalde işlendikten sonra, bu hizmet geçici harfler eşlemesini ve ilişkili belleği serbest bırakır.

Döndürülen metni işlemek için geçici bir alfamap gerektiğinden, döndürülen metni çizmeyi denemeden önce uygulamanın gx_system_memory_allocator çağıran gx_system_memory_allocator_set () API 'siyle yapılandırması gerekir.

Bu hizmet yalnızca "bir kez" döndürülen metni işlemek için kullanılmalıdır. Aynı metin dizesi farklı konumlarda veya farklı döndürme açılarında birden çok kez çizilip, bir kez metin harfler oluşturmak için gx_utility_string_to_alphamap () yardımcı program işlevini kullanmak daha verimlidir, sonra sonuçta elde edilen bir üst bilgi eşlemini sürekli olarak döndürmek için gx_utility_pixelmap_rotate birden çok kez kullanın.

### <a name="parameters"></a>Parametreler

- **metin** Çizilecek metin dizesi
- **Xcenter** Metnin döndürüleceği, ortaya dönmüş ton.
- **Yılmerkez** Metnin çevresinde döndürüleceği konumu Ortala.
- **açı** İstenen metin döndürme açısı (derece cinsinden).

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı metin işleme
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_SYSTEM_MEMORY_ERROR** (0x30) yeterli kullanılabilir bellek yok veya gx_system_memory_allocator atanmadı
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
void my_window_draw(GX_WINDOW *window)
{

    GX_VALUE xpos = 100;
    GX_VALUE ypos = 100;
    INT dynamic_count = 1234567;
    GX_CHAR dynamic_text[10];

    /* Call default window draw routine. */
    gx_window_draw(window);

    /* Set font. */
    gx_context_font_set(GX_FONT_ID_SMALL_BOLD);

    /* Convert int value to string. */
    gx_utility_ltoa(dynamic_count, dynamic_text, 20);

    /* Draw rotate text. */
    gx_canvas_rotated_text_draw(dynamic_text, xpos, ypos, 45);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_alpha_set,
- gx_canvas_drawing_complete
- gx_canvas_create,
- gx_canvas_drawing_initiate
- gx_canvas_offset_set,
- gx_canvas_shift

## <a name="gx_canvas_rotated_text_draw_ext"></a>gx_canvas_rotated_text_draw_ext


Bir orta nokta ile döndürülen metin çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_rotated_text_draw_ext(
    GX_CONST GX_STRING *text,
    GX_VALUE xCenter, 
    GX_VALUE yCenter, 
    INT angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, tuvale metin çizer. Metin, istenen merkez noktası hakkında döndürülmüş olarak çizilir. Metni işlemek için geçerli çizim bağlamı yazı tipi ve çizim bağlam çizgisi rengi kullanılır.

Bu hizmet, metin dizesini yalnızca alfa değeri içeren geçici bir 8bpp pixelmap 'e işlemek için gx_utility_string_to_alphamap işlevini kullanır. Daha sonra hizmet, gx_utility_pixelmap_rotate işlevini kullanarak harflerden eşlemeyi döndürür. Son alfamap tuvalde işlendikten sonra, bu hizmet geçici harfler eşlemesini ve ilişkili belleği serbest bırakır.

Döndürülen metni işlemek için geçici bir alfamap gerektiğinden, döndürülen metni çizmeyi denemeden önce uygulamanın gx_system_memory_allocator çağıran ***gx_system_memory_allocator_set*** API 'siyle yapılandırması gerekir.

Bu hizmet yalnızca "bir kez" döndürülen metni işlemek için kullanılmalıdır. Aynı metin dizesi farklı konumlarda veya farklı döndürme açılarında birden çok kez çizilip, bir kez metin harfler oluşturmak için gx_utility_string_to_alphamap () yardımcı program işlevini kullanmak daha verimlidir, sonra sonuçta elde edilen bir üst bilgi eşlemini sürekli olarak döndürmek için gx_utility_pixelmap_rotate birden çok kez kullanın.

### <a name="parameters"></a>Parametreler

- **metin** Çizilecek metin dizesi
- **Xcenter** Metnin döndürüleceği, ortaya dönmüş ton.
- **Yılmerkez** Metnin çevresinde döndürüleceği konumu Ortala.
- **açı** İstenen metin döndürme açısı (derece cinsinden).

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı metin işleme
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_CONTEXT** (0x06) geçersiz çizim bağlamı
- **GX_SYSTEM_MEMORY_ERROR** (0x30) yeterli kullanılabilir bellek yok veya gx_system_memory_allocator atanmadı.
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
void my_window_draw(GX_WINDOW *window)
{

    GX_VALUE xpos = 100;
    GX_VALUE ypos = 100;
    INT dynamic_count = 1234567;
    GX_CHAR dynamic_text[10];
    GX_STRING string;

    /* Call default window draw routine. */
    gx_window_draw(window);

    /* Set font. */
    gx_context_font_set(GX_FONT_ID_SMALL_BOLD);

    /* Convert int value to string. */
    gx_utility_ltoa(dynamic_count, dynamic_text, 20);

    string.gx_string_ptr = dynamic_text;
    string.gx_string_length = strlen(dynamic_text);

    /* Draw rotate text. */
    gx_canvas_rotated_text_draw_ext(&string, xpos, ypos, 45);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_alpha_set,
- gx_canvas_drawing_complete
- gx_canvas_create,
- gx_canvas_drawing_initiate
- gx_canvas_offset_set,
- gx_canvas_shift

## <a name="gx_canvas_shift"></a>gx_canvas_shift


X, y için tuval kaydır

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_shift(
    GX_CANVAS *canvas, 
    GX_VALUE x, GX_VALUE y);
```

### <a name="description"></a>Açıklama

Bu hizmet belirtilen tuval sapmasını belirtilen miktara kaydırır. Bu, tuvalin görünür çerçeve arabelleği içinde işlendiği konumu etkiler.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi
- X ekseninde SHIFT 'e **x** piksel
- Y ekseninde kaydırmak için **y** pikselleri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tuval kaydırma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CANVAS** (0x20) geçersiz tuval

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Shift canvas “my_canvas”. */
status = gx_canvas_shift(&my_canvas, 10, 15);

/* If status is GX_SUCCESS the canvas has been shifted by 10 pixels
    on the X axis and 15 on the Y axis. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_drawing_complete,
- gx_canvas_initiate
- gx_canvas_alpha_set,
- gx_canvas_create
- gx_canvas_offset_set

## <a name="gx_canvas_show"></a>gx_canvas_show


Tuvali görünür yapma

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_show(GX_CANVAS *canvas);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir tuvali görünür hale getirir. Tuval daha önce gx_canvas_hardware_layer_bind () API 'sini kullanarak bir donanım grafik katmanına bağlanmışsa, gx_canvas_show () hizmeti doğrudan donanım desteği kullanılarak uygulanır.

### <a name="parameters"></a>Parametreler

- **tuval** Tuval denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı Aralık ataması
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CANVAS** (0x20) geçersiz tuval

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Make this canvas visible. */
status = gx_canvas_show(&my_canvas);

/* If status is GX_SUCCESS the canvas drawing is now visible */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_alpha_set,
- gx_canvas_create
- gx_canvas_drawing_complete,
- gx_canvas_initiate,
- gx_canvas_shift,
- gx_canvas_hide,
- gx_canvas_hardware_layer_bind

## <a name="gx_canvas_text_draw"></a>gx_canvas_text_draw

Metin çiz (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_text_draw(
    GX_VALUE x_start, 
    GX_VALUE y_start,
    GX_CONST GX_CHAR *string, 
    INT length);
```

### <a name="description"></a>Açıklama

Bu hizmet, tuvalde metin çizer. Bu API hala desteklenirken kullanım dışıdır ve yeni uygulamalar bunun yerine gx_canvas_text_draw_ext () kullanmalıdır.

### <a name="parameters"></a>Parametreler

- **x_start** Metin için x koordinatı başlatılıyor
- **y_start** Metin için y koordinatı başlatılıyor
- **dize** Çizilecek dize işaretçisi
- **uzunluk** Length >= 0 ise, sıfıra çizilen karakter sayısını sınırlandırır. Length 0 <, NULL Sonlandırıcı çizilene kadar dizenin tamamı çizilmez.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı metin çiz
- **GX_FAILURE** (0x1E) metin çizme başarısız oldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw text “example” on current canvas”. */
status = gx_canvas_text_draw(10, 20, “example”, 7);

/* Draw all of a string of unknown length on the current canvas */
status = gx_canvas_text_draw(10, 40, string_ptr, -1);

/* If status is GX_SUCCESS the text “example” has been drawn. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_arc_draw,
- gx_canvas_block_move
- gx_canvas_circle_draw,
- gx_display_create
- gx_canvas_ellipse_draw,
- gx_canvas_line_draw
- gx_canvas_pie_draw,
- gx_canvas_pixelmap_draw
- gx_canvas_pixelmap_tile
- gx_canvas_polygon_draw,
- gx_canvas_rectangle_draw

## <a name="gx_canvas_text_draw_ext"></a>gx_canvas_text_draw_ext


Metin çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_canvas_text_draw_ext(
    GX_VALUE x_start, 
    GX_VALUE y_start,
    GX_CONST GX_STRING *string);
```

### <a name="description"></a>Açıklama

Bu hizmet, tuvalde metin çizer.

### <a name="parameters"></a>Parametreler

- **x_start** Metin için x koordinatı başlatılıyor
- **y_start** Metin için y koordinatı başlatılıyor
- **dize** Çizilecek dize işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı metin çiz
- **GX_FAILURE** (0x1E) metin çizme başarısız oldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_CONTEXT** (0x06) açık çizim bağlamı yok
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu
- **GX_INVALID_FONT** (0x16) geçersiz Yazı tipi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING string;
string.gx_string_ptr = “example”;
string.gx_string_length = 7;

/* Draw text “example” on current canvas”. */
status = gx_canvas_text_draw_ext(10, 20, &string);

/* If status is GX_SUCCESS the text “example” has been drawn. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_arc_draw,
- gx_canvas_block_move
- gx_canvas_circle_draw,
- gx_display_create
- gx_canvas_ellipse_draw,
- gx_canvas_line_draw
- gx_canvas_pie_draw,
- gx_canvas_pixelmap_draw
- gx_canvas_pixelmap_tile
- gx_canvas_polygon_draw,
- gx_canvas_rectangle_draw

## <a name="gx_checkbox_create"></a>gx_checkbox_create


Onay kutusu oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_checkbox_create(
    GX_CHECKBOX *checkbox, 
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent, 
    GX_RESOURCE_ID text_id,
    ULONG style, 
    USHORT checkbox_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen özelliklerle bir CheckBox pencere öğesi oluşturur. GX_CHECKBOX GX_TEXT_BUTTON türetilir ve tüm gx_text_button Hizmetleri GX_CHECKBOX pencere öğeleri ile kullanılabilir.

### <a name="parameters"></a>Parametreler

- **onay kutusu** CheckBox denetimin blok adı onay kutusu pencere öğesinin mantıksal adı işaretçisi
- **üst öğe** Üst pencere öğesi işaretçisi
- **text_id** CheckBox metninin kaynak KIMLIĞI
- **Stil** Onay kutusunun stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **checkbox_id** Uygulama tanımlı onay kutusunun KIMLIĞI
- **Boyut** CheckBox 'ın boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı onay kutusu oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz boyut

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_checkbox”. */
status = gx_checkbox_create(&my_checkbox, “my_checkbox”,
    &my_parent,
    MY_CHECKBOX_TEXT_RESOURCE_ID, GX_STYLE_BORDER_RAISED,
    MY_CHECKBOX_ID,
    &size);

/* If status is GX_SUCCESS the checkbox “my_checkbox” has been created. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_checkbox_draw,
- gx_checkbox_event_process,
- gx_checkbox_select

## <a name="gx_checkbox_draw"></a>gx_checkbox_draw

Çiz onay kutusu

### <a name="prototype"></a>Prototype

```C
VOID gx_checkbox_draw(GX_CHECKBOX *checkbox);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen onay kutusunu çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel onay kutusu pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **onay kutusu** CheckBox denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom checkbox draw function. */
VOID custom_checkbox_draw(GX_CHECKBOX *checkbox)
{
    /* Call default checkbox draw. */
    gx_checkbox_draw(checkbox);

    /* Add custom drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_checkbox_create,
- gx_checkbox_event_process,
- gx_checkbox_select

## <a name="gx_checkbox_event_process"></a>gx_checkbox_event_process


İşlem onay kutusu olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_checkbox_event_process(
    GX_CHECKBOX *checkbox, 
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen onay kutusu için bir olayı işler. Bu hizmet, özel onay kutusu olay işleme işlevleri tarafından varsayılan olay işleyicisi olarak çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **onay kutusu** CheckBox denetim bloğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı onay kutusu olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic checkbox event processing as part of custom event processing function. */

UINT custom_checkbox_event_process(GX_CHECKBOX *checkbox,
    GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;

    default:
        /* Pass all other events to the default checkbox
            event processing */
        status = gx_checkbox_event_process(checkbox, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_checkbox_create,
- gx_checkbox_draw,
- gx_checkbox_select

## <a name="gx_checkbox_pixelmap_set"></a>gx_checkbox_pixelmap_set


Onay kutusu için pixelmap ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_checkbox_pixelmap_set(
    GX_CHECKBOX *checkbox,
    GX_RESOURCE_ID unchecked_id, 
    GX_RESOURCE_ID checked_id,
    GX_RESOURCE_ID unchecked_disabled_id, 
    GX_RESOURCE_ID checked_disabled_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, her onay kutusu durumu için belirtilen onay kutusu tarafından görüntülenecek pixelmaps 'ı atar. Kaynak kimlikleri yinelenebilir.

### <a name="parameters"></a>Parametreler

- **onay kutusu** CheckBox denetim bloğu işaretçisi
- **unchecked_id** İşaretlenmemiş durum için pixelmap kullanıldı
- **checked_id** Denetlenen durum için pixelmap kullanıldı
- **unchecked_disabled_id** Devre dışı bırakılmış ve işaretlenmemiş onay kutusu için pixelmap kullanıldı
- **checked_disabled_id** Bir devre dışı ve işaretli onay kutusu için pixelmap kullanıldı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı onay kutusu seçme
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Select “my_checkbox”. */
status = gx_checkbox_pixelmap_set(&my_checkbox,
    PIXELMAP_UNCHECKED_ID,
    PIXELMAP_CHECKED_ID, PIXELMAP_UNCHECKED_DISABLED_ID,
    PIXELMAP_CHECKED_SIABLED_ID));

/* If status is GX_SUCCESS the pixelmaps are assigned to the checkbox “my_checkbox” */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_checkbox_create,
- gx_checkbox_draw,
- gx_checkbox_event_process

## <a name="gx_checkbox_select"></a>gx_checkbox_select


Onay kutusunu seçin

### <a name="prototype"></a>Prototype

```C
UINT gx_checkbox_select(GX_CHECKBOX *checkbox);
```

### <a name="description"></a>Açıklama

Bu hizmet, seçili duruma bir onay kutusu zorlar.

### <a name="parameters"></a>Parametreler

- **onay kutusu** CheckBox denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı onay kutusu seçme
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Select “my_checkbox”. */
status = gx_checkbox_select(&my_checkbox);

/* If status is GX_SUCCESS the checkbox “my_checkbox” has been toggled. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_checkbox_create,
- gx_checkbox_draw,
- gx_checkbox_event_process

## <a name="gx_circular_gauge_angle_get"></a>gx_circular_gauge_angle_get


Geçerli açıyı al

### <a name="prototype"></a>Prototype

```C
UINT gx_circular_gauge_angle_get(
    GX_CIRCULAR_GAUGE *gauge, 
    INT *angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, dairesel ölçer pencere öğesinin geçerli iğne açısını alır.

### <a name="parameters"></a>Parametreler

- **ölçer** Dairesel ölçer denetim bloğu işaretçisi
- **açı** Alınacak geçerli iğne açısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı dairesel ölçer açısı al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
INT current_angle;

/* Retrieve the current needle angle of “my_gauge”. */
status = gx_circular_gauge_angle_get(&my_gauge, &current_angle);

/* If status is GX_SUCCESS the current needle angle of “my_gauge” has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_circular_gauge_angle_set,
- gx_circular_gauge_animation_set
- gx_circular_gauge_background_draw,
- gx_circular_gauge_create
- gx_circular_gauge_draw,
- gx_circular_gauge_event_process

## <a name="gx_circular_gauge_angle_set"></a>gx_circular_gauge_angle_set


Hedef açısını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_circular_gauge_angle_set(
    GX_CIRCULAR_GAUGE *gauge,
    INT angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, dairesel ölçer pencere öğesinin hedef açısını ayarlar.

### <a name="parameters"></a>Parametreler

- **ölçer** Dairesel ölçer denetim bloğu işaretçisi
- **açı** Hedef iğne açısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı açı kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set target angle of “my_gauge” to 180. */
status = gx_circular_gauge_angle_set(&my_gauge, 180);

/* If status is GX_SUCCESS the circular gauge of “my_gauge” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_circular_gauge_angle_get,
- gx_circular_gauge_animation_set
- gx_circular_gauge_background_draw,
- gx_circular_gauge_create
- gx_circular_gauge_draw,
- gx_circular_gauge_event_process

## <a name="gx_circular_gauge_animation_set"></a>gx_circular_gauge_animation_set


Animasyon parametrelerini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_circular_gauge_animation_set(
    GX_CIRCULAR_GAUGE *gauge,
    INT steps, 
    INT delay);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir dairesel ölçer pencere öğesi için animasyon adımlarını ve gecikme süresini ayarlar.

### <a name="parameters"></a>Parametreler

- **ölçer** Dairesel ölçer denetim bloğu işaretçisi
- **adımlar** Tek bir döndürme için toplam adım sayısı
- **gecikme** Her adım için gecikme süresi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı onay kutusu seçme
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE** (0x22) geçersiz değer

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set animation steps and delay time of circular gauge “my_gauge”
    to 30 and 1, the needle of “my_gauge” will rotate from
    current angle to target angle by 30 steps with 1 tick delay between every step. */
status = gx_circular_gauge_animation_set(&my_gauge, 30, 1);

/* If status is GX_SUCCESS the steps and delay time of “my_gauge” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_circular_gauge_angle_get,
- gx_circular_gauge_angle_set
- gx_circular_gauge_background_draw,
- gx_circular_gauge_create
- gx_circular_gauge_draw,
- gx_circular_gauge_event_process

## <a name="gx_circular_gauge_background_draw"></a>gx_circular_gauge_background_draw


Dairesel ölçer arka planı çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_circular_gauge_background_draw(GX_CIRCULAR_GAUGE *gauge);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen dairesel ölçerin arka planını çizer. Bu hizmet, genellikle gx_circular_gauge_draw işlevi tarafından dahili olarak çağrılır, ancak özel çizim işlevleri yazma konusunda yardımcı olmak için uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **ölçer** Dairesel ölçer denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw circular gauge background. */
gx_circular_gauge_background_draw(&my_circular_gauge);
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_circular_gauge_angle_get,
- gx_circular_gauge_angle_set
- gx_circular_gauge_animation_set,
- gx_circular_gauge_create
- gx_circular_gauge_draw,
- gx_circular_gauge_event_process

## <a name="gx_circular_gauge_create"></a>gx_circular_gauge_create


Dairesel ölçer oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_circular_gauge_create(
    GX_CIRCULAR_GAUGE *gauge,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_CIRCULAR_GAUGE_INFO *info,
    GX_RESOURCE_ID background_id,
    ULONG style,
    USHORT circular_gauge_id,
    GX_VALUE xpos,
    GX_VALUE ypos);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen özelliklerle bir dairesel ölçer pencere öğesi oluşturur.

### <a name="parameters"></a>Parametreler

- **ölçer** Dairesel ölçer denetim bloğu işaretçisi
- **ad** Dairesel ölçer pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **bilgi** Ölçer bilgi yapısına yönelik işaretçi. **Ek ı** GX_CIRCULAR_GAUGE_INFO yapısına tanım içeriyor
- **background_id** Döngüsel ölçer arka plan pixelmap kaynak KIMLIĞI
- **Stil** Dairesel ölçerin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **circular_gauge_id** Uygulama tanımlı dairesel ölçer KIMLIĞI
- **XPos** Ölçer x koordinatı konumu
- **yılkonumu** Ölçer y-koordinat konumu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı onay kutusu seçme
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_SIZE** (0x19) geçersiz denetim bloğu boyutu
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CIRCULAR_GAUGE gauge_info;

gauge_info.gx_circular_gauge_info_animation_steps = 30;
gauge_info.gx_circular_gauge_info_animation_delay = 1;
gauge_info.gx_circular_gauge_info_needle_xpos = 140;
gauge_info.gx_circular_gauge_info_needle_ypos = 140;
gauge_info.gx_circular_gauge_info_neelde_xcor = 20;
gauge_info.gx_circular_gauge_info_neelde_ycor = 88;
gauge_info.gx_circular_gauge_info_needle_pixelmap = GX_PIXELMAP_ID_NEEDLE;

/* Create “my_gauge”. */
status = gx_circular_gauge_create(&my_gauge, “my_gauge”,
            &my_parent,
            &gauge_info, MY_PIXELMAP_RESOURCE_ID, GX_NULL,
            MY_ICON_ID, 5, 30);

/* If status is GX_SUCCESS the circular gauge “my_gauge” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_circular_gauge_angle_get,
- gx_circular_gauge_angle_set
- gx_circular_gauge_animation_set
- gx_circular_gauge_background_draw,
- gx_circular_gauge_draw
- gx_circular_gauge_event_process

## <a name="gx_circular_gauge_draw"></a>gx_circular_gauge_draw

Dairesel ölçer çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_circular_gauge_draw(GX_CIRCULAR_GAUGE *gauge);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen dairesel ölçer çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel ölçer pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **ölçer** Dairesel ölçer denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom circular gauge draw function. */
VOID custom_gauge_draw(GX_CIRCULAR_GAUGE *gauge)
{
    /* Call default circular gauge draw. */
    gx_circular_gauge_draw(gauge);

    /* Add custom drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_circular_gauge_angle_get,
- gx_circular_gauge_angle_set
- gx_circular_gauge_animation_set
- gx_circular_gauge_background_draw
- gx_circular_gauge_create,
- gx_circular_gauge_event_process

## <a name="gx_circular_gauge_event_process"></a>gx_circular_gauge_event_process


Döngüsel ölçer olayını işle

### <a name="prototype"></a>Prototype

```C
UINT gx_circular_gauge_event_process(
    GX_CIRCULAR_GAUGE *gauge,
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen döngüsel ölçer için bir olayı işler.

### <a name="parameters"></a>Parametreler

- **ölçer** Ölçer denetim bloğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ölçer olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic circular gauge event processing as part of custom event processing function. */
UINT custom_gauge_event_process(GX_CIRCULAR_GAUGE *gauge,
    GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;

    default:
        /* Pass all other events to the default circular gauge
             event processing */
        status = gx_circular_gauge_event_process(gauge, event);
        break;
}
return status;
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_circular_gauge_angle_get,
- gx_circular_gauge_angle_set
- gx_circular_gauge_animation_set
- gx_circular_gauge_background_draw,
- gx_circular_gauge_create
- gx_circular_gauge_draw

## <a name="gx_context_brush_default"></a>gx_context_brush_default


Geçerli çizim bağlamının fırça kümesini ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_context_brush_default(GX_DRAW_CONTEXT *context);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen çizim bağlamının fırçasını varsayılan olarak ayarlar.

### <a name="parameters"></a>Parametreler

- **bağlam** Bağlam denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı oluşturma
- **GX_PTR_ERROR** (0x07) geçersiz bağlam işaretçisi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the brush of “my_context” to default. */
status = gx_context_brush_default(&my_context);

/* If status is GX_SUCCESS the brush of “my_context” has been set to default. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_define,
- gx_context_brush_get
- gx_context_brush_set,
- gx_context_brush_style_set
- gx_context_brush_pattern_set,
- gx_context_brush_width_set
- gx_context_fill_color_set,
- gx_context_font_set
- gx_context_line_color_set,
- gx_context_pixelmap_set
- gx_context_raw_brush_define,
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_brush_define"></a>gx_context_brush_define


Geçerli çizim bağlamının kapsamını tanımlayın

### <a name="prototype"></a>Prototype

```C
UINT gx_context_brush_define(
    GX_RESOURCE_ID line_color_id,
    GX_RESOURCE_ID fill_color_id, 
    UINT style);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamının fırçasını tanımlar.

### <a name="parameters"></a>Parametreler

- **line_color_id** Çizgi renginin kaynak KIMLIĞI. **Ek B** önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **fill_color_id** Fill Color kaynak KIMLIĞI. **Ek B** önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **Stil** Fırçanın stili. **Ek D** desteklenen fırça stillerini açıklar. Fırça stilleri, bit düzeyinde OR işlemi kullanarak bir değişkende birleştirilebilir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam fırçası tanımlama
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı tanımlama
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define the brush of the current context. */
status = gx_context_brush_define(GX_COLOR_BLACK_ID,
    GX_COLOR_BLACK_ID,
    GX_STYLE_BORDER_NONE);

/* If status is GX_SUCCESS the brush of the current context has been defined. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default,
- gx_context_brush_get
- gx_context_brush_set,
- gx_context_brush_pattern_set
- gx_context_brush_style_set,
- gx_context_brush_width_set
- gx_context_fill_color_set,
- gx_context_font_set
- gx_context_line_color_set,
- gx_context_pixelmap_set
- gx_context_raw_brush_define,
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_brush_get"></a>gx_context_brush_get


Geçerli çizim bağlamının fırçasını al

### <a name="prototype"></a>Prototype

```C
UINT gx_context_brush_get(GX_BRUSH **return_brush);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamındaki etkin fırçaya bir işaretçi döndürür. Etkin çizim bağlamı yoksa, hizmet başarısız olur ve NULL bir işaretçi döndürür.

### <a name="parameters"></a>Parametreler

- **return_brush** Fırçanın hedefi işaretçisi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) bağlam fırçası başarıyla alındı
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_BRUSH *my_brush;

/* Get the brush of the current context. */
status = gx_context_brush_get(&my_brush);

/* If status is GX_SUCCESS the brush of the current context has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_set,
- gx_context_brush_style_set
- gx_context_brush_default,
- gx_context_brush_define
- gx_context_brush_pattern_set,
- gx_context_brush_width_set
- gx_context_fill_color_set,
- gx_context_font_set
- gx_context_line_color_set,
- gx_context_pixelmap_set
- gx_context_raw_brush_define,
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_brush_pattern_set"></a>gx_context_brush_pattern_set


Geçerli çizim bağlamının fırça düzenlerini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_context_brush_pattern_set(ULONG pattern);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamının fırça modelini ayarlar.

Fırça deseninin kesik çizgili yatay ve kesik çizgili dikey çizgiler çizmek için kullanılır. Gx_canvas_line_draw () çağrıldığında ve çizgi yatay veya dikey olduğunda ve brush.gx_brush_line_pattern alanı sıfır değilse, bir kalıp çizgisi çizilir.

Fırça deseninin maskesi Şu anda yalnızca yatay ve dikey çizgiler için desteklenir.

### <a name="parameters"></a>Parametreler

- **örüntü** Fırça için kullanılacak model. Bu, kalıp çizgisi çiziminde kullanılacak basit bir onaltılık açık/kapalı örüntü.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam fırçası kümesi
- **GX_INVALID_CONTEXT** (0x06) geçersiz çizim bağlamı

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the brush pattern for the current contex. */
status = gx_context_brush_pattern_set(0x80808080);

/* If status is GX_SUCCESS the brush pattern of the current context
has been set to the specified pattern. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default,
- gx_context_brush_define
- gx_context_brush_get,
- gx_context_brush_style_set
- gx_context_brush_width_set,
- gx_context_fill_color_set
- gx_context_font_set,
- gx_context_line_color_set
- gx_context_pixelmap_set,
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set,
- gx_context_raw_line_color_set

## <a name="gx_context_brush_set"></a>gx_context_brush_set


Geçerli çizim bağlamının fırça kümesini ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_context_brush_set(GX_BRUSH *brush);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamının fırçasını ayarlar.

### <a name="parameters"></a>Parametreler

- **fırça** Geçerli bağlam için kullanılacak fırça işaretçisi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam fırçası kümesi
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_BRSUH my_brush;
GX_FONT *font;
GX_COLOR fill_color;
GX_COLOR line_color;

/* Retrieve the font that associated with the specified font ID. */
gx_context_font_get(MY_FONT_ID, &font);

/* Retrieve the color that associated with the specified color ID. */
gx_context_color_get(MY_FILL_COLOR_ID, &fill_color);
gx_context_color_get(MY_LINE_COLOR, &line_color);

my_brush.gx_brush_pixelmap = MY_PIXELMAP_ID;
my_brush.gx_brush_font = font;
my_brush.gx_brush_line_pattern = 0x80808080;
my_brush.gx_brush_pattern_mask = 0x80000000;
my_brush.gx_brush_fill_color = fill_color;
my_brush.gx_brush_line_color = line_color;
my_brush.gx_brush_style = GX_BRSUH_SOLID_FILL | GX_BRUSH_ALIAS |
                          GX_BRUSH_PIXELMAP_FILL | GX_BRUSH_ROUND
my_brush.gx_brush_width = 2;
my_brush.gx_brush_alpha = 255;

/* Set the brush of the current context. */
status = gx_context_brush_set(my_brush);

/* If status is GX_SUCCESS the brush of the current context has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default,
- gx_context_brush_define
- gx_context_brush_get,
- gx_context_brush_pattern_set
- gx_context_brush_style_set,
- gx_context_brush_width_set
- gx_context_fill_color_set,
- gx_context_font_set
- gx_context_line_color_set,
- gx_context_pixelmap_set
- gx_context_raw_brush_define,
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_brush_style_set"></a>gx_context_brush_style_set


Geçerli çizim bağlamının Fırça stilini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_context_brush_style_set(UINT style);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamının Fırça stilini ayarlar.

### <a name="parameters"></a>Parametreler

- **Stil** Geçerli bağlamın fırça stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam fırçası stil kümesi
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the brush style of the current context. */
status = gx_context_brush_style_set(GX_BRUSH_ALIAS);

/* If status is GX_SUCCESS the brush style of the current context has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default,
- gx_context_brush_define
- gx_context_brush_get,
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_width_set,
- gx_context_fill_color_set
- gx_context_font_set,
- gx_context_line_color_set
- gx_context_pixelmap_set,
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set,
- gx_context_raw_line_color_set

## <a name="gx_context_brush_width_set"></a>gx_context_brush_width_set


Geçerli çizim bağlamının fırça genişliğini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_context_brush_width_set(UINT width);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamındaki etkin fırçanın genişliğini ayarlar.

### <a name="parameters"></a>Parametreler

**Genişlik** Geçerli bağlamın piksel cinsinden fırça genişliği

### <a name="return-values"></a>Dönüş Değerleri

**GX_SUCCESS** (0x00) başarılı bağlam fırçası genişlik kümesi

**GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the brush width of the current context to 10 pixels. */
status = gx_context_brush_width_set(10); /*

If status is GX_SUCCESS the brush width of the current context has been set to 10. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_fill_color_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_color_get"></a>gx_context_color_get


Geçerli çizim bağlamındaki renk KIMLIĞIYLE ilişkili renk değerini Al

### <a name="prototype"></a>Prototype

```C
UINT gx_context_color_get(
    GX_RESOURCE_ID color_id,
    GX_COLOR *return_color);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen renk KIMLIĞIYLE ilişkili renk değerini alır. Renk değeri, etkin bağlam görüntüsüne ait Color biçiminde döndürülür. Bu hizmet yalnızca etkin bir çizim işleminin içinden çağrılmalıdır.

### <a name="parameters"></a>Parametreler

**color_id** İstenen rengin kaynak KIMLIĞI.

**return_color** Döndürülen renk değerini tutacak değişkenin adresi.

### <a name="return-values"></a>Dönüş Değerleri

**GX_SUCCESS** (0x00) başarılı renk değeri Al

**GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği

**GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

**GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_COLOR color_value;

/* Get the color vaue. */
status = gx_context_color_get(MY_BLACK_COLOR_ID, &color_value);
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_fill_color_set"></a>gx_context_fill_color_set

Geçerli çizim bağlamının Fill rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_context_fill_color_set(GX_RESOURCE_ID fill_color_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamındaki etkin fırçanın dolgusu rengini ayarlar.

### <a name="parameters"></a>Parametreler

- **fill_color_id** Geçerli bağlamın Fill renginin kaynak KIMLIĞI. **Ek B** önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam dolgusu renk kümesi
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the fill color of the current context to black. */
status = gx_context_fill_color_set(MY_BLACK_COLOR_ID);

/* If status is GX_SUCCESS the fill color of the current context has been set to black. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_font_get"></a>gx_context_font_get

Geçerli çizim bağlamındaki yazı tipi KIMLIĞIYLE ilişkili yazı tipini al

### <a name="prototype"></a>Prototype

```C
UINT gx_context_font_get(
    GX_RESOURCE_ID font_id,
    GX_FONT **return_font);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen yazı tipi KIMLIĞIYLE ilişkili yazı tipi işaretçisini alır. Bu hizmet yalnızca etkin bir çizim işleminin içinden çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **font_id** İstenen yazı tipinin kaynak KIMLIĞI.
- **return_font** Döndürülen yazı tipi işaretçisini tutacak değişkenin adresi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) yazı tipi başarıyla alındı
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_FONT *my_font;

/* Get the font pointer. */
status = gx_context_font_get(MY_MIDSIZE_FONT, &my_font);

/* If status is GX_SUCCESS, the font that indicated with MY_MIDSIZE_FONT has been successfully retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_font_set"></a>gx_context_font_set

Geçerli çizim bağlamının yazı tipini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_context_font_set(GX_RESOURCE_ID font_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamının etkin fırçasının yazı tipini ayarlar.

### <a name="parameters"></a>Parametreler

- **font_id** Geçerli bağlamın yazı tipi kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam yazı tipi kümesi
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the font of the current context to MY_FONT_ID. */
status = gx_context_font_set(MY_FONT_ID);

/* If status is GX_SUCCESS the font of the current context has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_fill_color_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_line_color_set"></a>gx_context_line_color_set

Geçerli çizim bağlamının çizgi rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_context_line_color_set(GX_RESOURCE_ID line_color_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamındaki etkin fırçanın çizgi rengini ayarlar.

### <a name="parameters"></a>Parametreler

- **line_color_id** Geçerli bağlamın çizgi rengi. **Ek B** önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam çizgisi renk kümesi
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the line color of the current context to black. */
status = gx_context_line_color_set(GX_COLOR_BLACK_ID);

/* If status is GX_SUCCESS the line color of the current context has been set to black. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_fill_color_set
- gx_context_font_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_pixelmap_get"></a>gx_context_pixelmap_get

Geçerli çizim bağlamındaki pixelmap KIMLIĞIYLE ilişkili pixelmap 'i al

### <a name="prototype"></a>Prototype

```C
UINT gx_context_pixelmap_get(
    GX_RESOURCE_ID pixelmap_id,
    GX_PIXELMAP **return_map);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pixelmap KIMLIĞIYLE ilişkili pixelmap işaretçisini alır.

### <a name="parameters"></a>Parametreler

- **pixelmap_id** Pixelmap kaynak KIMLIĞI istendi.
- **return_map** Geri döndürülen pixelmap adresini tutacak değişkenin adresi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00), pixelmap başarıyla alındı
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok
- **GX_PTR_ERROR** (0x07) geçersiz pixelmap işaretçisi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_PIXELMAP *map;

/* Get the pixelmap pointer. */
status = gx_context_pixelmap_get(MY_PIXELMAP_ID, &map);

/* If status is GX_SUCCESS, the pixelmap was successfully retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_pixelmap_set"></a>gx_context_pixelmap_set

Geçerli çizim bağlamının pixelmap 'i ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_context_pixelmap_set(GX_RESOURCE_ID pixelmap_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, etkin fırçanın pixelmap 'i geçerli çizim bağlamına atar.

### <a name="parameters"></a>Parametreler

- **pixelmap_id** Geçerli bağlam için kullanılacak pixelmap kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam pixelmap kümesi
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVLAID_CONTEXT** (0x06) geçersiz bağlam

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set pixelmap of the current context to MY_PIXELMAP_ID. */
status = gx_context_pixelmap_set(MY_PIXELMAP_ID);

/* If status is GX_SUCCESS the pixelmap of the current context has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_fill_color_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_raw_brush_define"></a>gx_context_raw_brush_define

Geçerli çizim bağlamının ham fırçasını tanımlayın

### <a name="prototype"></a>Prototype

```C
UINT gx_context_raw_brush_define(
    GX_COLOR line_color,
    GX_COLOR fill_color, 
    UINT style);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli ekran bağlamının ham fırçasını tanımlar. Ham tanımlar, 32 bitlik ARGB renk değerleri renk kimlikleri yerine fırçaya geçirilene zaman kullanılır. Ham renk tanımları, istenen renk geçerli sistem renk tablosunda yoksa veya RGB renk değeri çalışma zamanında hesaplanmışsa yararlıdır.

### <a name="parameters"></a>Parametreler

- **line_color** 32 bitlik ham ARGB renk biçimindeki çizginin rengi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.
- **fill_color** 32-bit ham ARGB renk biçimindeki dolgunun rengi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.
- **Stil** Fırçanın stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam ham fırçası tanımlama
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define the raw brush of the current context. */
status = gx_context_raw_brush_define(GX_COLOR_BLACK,
    GX_COLOR_BLACK, GX_STYLE_BORDER_NONE);

/* If status is GX_SUCCESS the raw brush of the current context has been defined. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_fill_color_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_fill_color_set
- gx_context_raw_line_color_set

## <a name="gx_context_raw_fill_color_set"></a>gx_context_raw_fill_color_set

Geçerli çizim bağlamının ham dolgusu rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_context_raw_fill_color_set(GX_COLOR line_color);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli ekran bağlamının ham dolgusu rengini ayarlar. Line_color parametresi, renk KIMLIĞI değeri yerine 32 bitlik bir ARGB formatı ham renk değeridir. Ham renk tanımları, istenen renk geçerli sistem renk tablosunda yoksa veya RGB renk değeri çalışma zamanında hesaplanmışsa yararlıdır.

### <a name="parameters"></a>Parametreler

- **line_color** Çizgi rengi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam ham dolgusu renk kümesi
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the raw fill color of the current context. */
status = gx_context_raw_fill_color_set(GX_COLOR_BLACK);

/* If status is GX_SUCCESS the raw fill color of the current context has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_fill_color_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_line_color_set

## <a name="gx_context_raw_line_color_set"></a>gx_context_raw_line_color_set

Geçerli çizim bağlamının ham çizgi rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_context_raw_line_color_set(GX_COLOR line_color);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamındaki etkin fırçanın çizgi rengini ayarlar. Line_color parametresi, renk KIMLIĞI değeri yerine 32 bitlik bir ARGB formatı ham renk değeridir. Ham renk tanımları, istenen renk geçerli sistem renk tablosunda yoksa veya RGB renk değeri çalışma zamanında hesaplanmışsa yararlıdır.

### <a name="parameters"></a>Parametreler

- **line_color** Çizgi değerinin rengi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam ham çizgi renk kümesi
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

```C
/* Set the raw line color of the current context. */
status = gx_context_raw_line_color_set(GX_COLOR_BLACK);

/* If status is GX_SUCCESS the raw line color of the current context has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_fill_color_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set

## <a name="gx_context_string_get"></a>gx_context_string_get

Dize KIMLIĞIYLE ilişkili dizeyi al (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_context_string_get(GX_RESOURCE_ID string_id,
    GX_CONST GX_CHAR **return_string);
```

### <a name="description"></a>Açıklama

Kullanım dışı bırakılan bu API, belirtilen dize KIMLIĞIYLE ilişkili dizeyi döndürür. Yeni uygulamalar gx_context_string_get_ext () kullanmalıdır.

### <a name="parameters"></a>Parametreler

- **string_id** GUX Studio uygulaması tarafından oluşturulan dize KIMLIĞI.
- **return_string** Dize işaretçisinin döndürülme değişkeninin adresi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam ham çizgi renk kümesi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR *text;

status = gx_context_string_get(GX_ID_ERROR, &text);

/* If status is GX_SUCCESS the string pointer has been returned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_string_get_ext

## <a name="gx_context_string_get_ext"></a>gx_context_string_get_ext

Verilen dize KIMLIĞIYLE ilişkili dizeyi al.

### <a name="prototype"></a>Prototype

```C
UINT gx_context_string_get_ext(
    GX_RESOURCE_ID string_id, 
    GX_STRING *return_string);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirli bir dize KIMLIĞIYLE ilişkili dizeyi döndürür. Bu hizmet yalnızca etkin bir çizim bağlamı olduğunda (örneğin, pencere öğesinin çizim işlevinin içinden) çağrılabilir. Bu hizmet etkin tuvali tanımlar ve bulunan görüntü örneğinden dizeyi görüntüler ve alır.

### <a name="parameters"></a>Parametreler

- **string_id** Uygulama kaynak üstbilgi dosyasında GUıDX Studio tarafından oluşturulan dizeyi tanımlamak için kullanılan dize KIMLIĞI.
- **return_string** Dize işaretçisinin ve dize uzunluğunun döndürüleceği GX_STRING değişkenin adresi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlam ham çizgi renk kümesi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_CONTEXT** (0x06) etkin çizim bağlamı yok

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek


```C
GX_STRING string;

/* Set the raw line color of the current context. */
status = gx_context_string_get_ext(ID_ERROR, &string);

/* If status is GX_SUCCESS the string.gx_string_ptr and
string.gx_string_length values have been returned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_context_brush_default
- gx_context_brush_define
- gx_context_brush_get
- gx_context_brush_set
- gx_context_brush_pattern_set
- gx_context_brush_style_set
- gx_context_brush_width_set
- gx_context_fill_color_set
- gx_context_font_set
- gx_context_line_color_set
- gx_context_pixelmap_set
- gx_context_raw_brush_define
- gx_context_raw_fill_color_set

## <a name="gx_display_active_language_set"></a>gx_display_active_language_set

Etkin görüntüleme dilini ata

### <a name="prototype"></a>Prototype

```C
UINT gx_display_active_language_set(
    GX_DISPLAY *display, 
    GX_UBYTE language);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen görünüm için şu anda etkin olan dili atar. Dil dizini, görüntüleme dili tablosunda tanımlanan dillere karşılık gelir ve ANSI dil tanımlayıcısı değildir.

Birden çok görüntü sisteminde farklı ekranlar, her biri farklı etkin diller çalıştırabilir. Bu API kullanılmadan önce görüntüleme dili tablosu atanmalıdır. Bir ekran gx_studio_display_configure kullanılarak başlatıldığında, dil tablosu otomatik olarak yüklenir ve uygulama etkin dil dizininde geçirilir.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **dil** Etkin dil dizini

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı dil ataması
- **GX_PTR_ERROR** (0x07) geçersiz görüntüleme işaretçisi
- **GX_INVALID_VALUE** (0x22) geçersiz dil dizini

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Change value of color MY_COLOR_ID. */
status = gx_display_active_language_set(&my_display,
    LANGUAGE_ENGLISH);

/* If status is GX_SUCCESS the active language has been assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_language_table_set
- gx_studio_display_configure

## <a name="gx_display_color_set"></a>gx_display_color_set

Bir renk değerini yeniden ata

### <a name="prototype"></a>Prototype

```C
UINT gx_display_color_set(
    GX_DISPLAY *display,
    GX_RESOURCE_ID color_id, 
    GX_COLOR new_color);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen renk KIMLIĞIYLE ilişkili renk değerini yeniden atar. Bu, tamamen yeni bir renk tablosu sağlamadan bir görüntünün renk tablosunu değiştirmek için kullanılabilir. Belirtilen renk değeri, görüntü tarafından desteklenen yerel biçimde olmalıdır.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **color_id** Yeniden atanacak renk KIMLIĞI
- **new_color** Bu color_id yuvasına atanacak renk değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı renk yeniden atama
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ renk kimliği
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_DISPLAY** (0x1d) geçersiz görüntüleme

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Change value of color MY_COLOR_ID. */
status = gx_display_color_set(&my_display, MY_COLOR_ID, 0x5454);

/* If status is GX_SUCCESS the color has been reassigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_color_table_set

## <a name="gx_display_color_table_set"></a>gx_display_color_table_set

Görüntü renk tablosu ata

### <a name="prototype"></a>Prototype

```C
UINT gx_display_color_table_set(
    GX_DISPLAY *display,
    GX_COLOR *color_table, 
    INT color_count);
```

### <a name="description"></a>Açıklama

Bu hizmet, ekran tarafından kullanılacak renk tablosunu yeniden atar. Bu hizmet normalde Gux Studio tarafından üretilen görüntüleme yapılandırma işlevi tarafından çağrılır, ancak uygulama yazılımı tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **Color_Table** Yerel görüntü biçimindeki renk değerleri dizisi.
- **color_count** Renk tablosundaki giriş sayısını gösterir

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı renk tablosu kümesi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_DISPLAY** (0x1d) geçersiz görüntüleme

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_COLOR default_table[32] = { … };

/* Change the color table */
status = gx_display_color_table_set(&my_display, default_table, 32);

/* If status is GX_SUCCESS the color table has been reassigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_color_set

## <a name="gx_display_create"></a>gx_display_create

Görüntü oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_display_create(
    GX_DISPLAY *display, 
    GX_CONST CHAR *name,
    UINT (*display_driver_setup)(GX_DISPLAY *),
    GX_VALUE width, 
    GX_VALUE height);
```

### <a name="description"></a>Açıklama

Bu hizmet bir görüntü oluşturur ve görüntü sürücüsü kurulum işlevini çağırır. GUX bu görüntüyü alır ve kendi iç ekran listesine ekler.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **ad** Ekran adı
- **display_driver_setup** Görüntü sürücüsü kurulum işlevi işaretçisi
- **optional_driver_info** İsteğe bağlı sürücü bilgisi işaretçisi
- **color_format** **Ek C** 'de tanımlandığı şekilde renk biçimi
- **Genişlik** X eksenindeki piksel sayısı
- **Yükseklik** Y eksenindeki piksel sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı görüntü oluşturma
- **GX_SYSTEM_ERROR** (0xFE), ekran kurulumunu gerçekleştiremeyecek
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_SIZE** (0x23) geçersiz görüntüleme denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_DISPLAY my_display;

UINT my_driver_setup_callback(GX_DISPLAY *display)
{
    …
}

/* Create screen “my_display”. */
status = gx_display_create(&my_display, “my display”,
    my_driver_setup_callback, 320, 480);

/* If status is GX_SUCCESS, the screen “my_display” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_delete

## <a name="gx_display_delete"></a>gx_display_delete


Ekranı yok et

### <a name="prototype"></a>Prototype

```C
UINT gx_display_delete(
    GX_DISPLAY *display,
    VOID (*display_driver_cleanup)(GX_DISPLAY *));
```

### <a name="description"></a>Açıklama

Bu hizmet bir ekranı kapatır ve ayrılan kaynakları temizler.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **display_driver_cleanup** Görüntü sürücüsü Temizleme işlevinin işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı görüntüleme silme
- **GX_FAILURE** (0x10) oluşturulan görüntüleme listesi null
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
VOID driver_cleanup_callback(GX_DISPLAY *display)
{
    …
}

/* Delete a display “my_display”. */
status = gx_display_delete(&my_display, driver_cleanup_callback);

/* If status is GX_SUCCESS the screen “my_display” has been destroyed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_canvas_block_move
- gx_canvas_line_draw
- gx_canvas_pixelmap_draw
- gx_canvas_pixelmap_tile
- gx_canvas_polygon_draw
- gx_canvas_rectangle_draw
- gx_canvas_text_draw
- gx_display_create

## <a name="gx_display_font_table_set"></a>gx_display_font_table_set

Görüntüleme yazı tipi tablosu ata

### <a name="prototype"></a>Prototype

```C
UINT gx_display_font_table_set(
    GX_DISPLAY *display,
    GX_FONT **font_table, 
    INT table_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, ekran tarafından kullanılacak yazı tipi tablosunu yeniden atar. Bu hizmet normalde Gux Studio tarafından üretilen görüntüleme yapılandırma işlevi tarafından çağrılır, ancak uygulama yazılımı tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **font_table** GX_FONT işaretçileri dizisi.
- **table_size** Tablodaki yazı tipi sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yazı tipi tablo kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_FONT *font_table[32] = { … };

/* Assign font table */
status = gx_display_font_table_set(&my_display, font_table, 32);

/* If status is GX_SUCCESS, the font table has been reassigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_color_set
- gx_display_color_table_set
- gx_display_pixelmap_table_set

## <a name="gx_display_language_table_get"></a>gx_display_language_table_get

Görüntüleme dili tablosunu al (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_display_language_table_get(
    GX_DISPLAY *display,
    GX_CHAR **table, 
    GX_UBYTE *language_count,
    UINT *string_table_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen görüntülenen dil tablosunu alır. Bu hizmet, bir uygulama tarafından, çalışma zamanında dinamik olarak tanımlanan dizeler kullanılarak görüntüleme dili tablosunu değiştirmek üzere kullanılabilir.

Bu API kullanım dışıdır ve yalnızca eski stil dili tablosunu kullanan uygulamalar için desteklenir (yani, sürüm 5,6 ' den önceki kitaplık sürümü için Studio tarafından oluşturulan kaynak dosyası oluşturulur). Yeni uygulamalar gx_display_language_table_get_ext () kullanmalıdır.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **tablo** Tablo işaretçisinin alınacağı adres
- **language_count** Dil sayısını alacak adres
- **string_table_size** Dize tablosu boyutunu alma adresi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yazı tipi tablo kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR **language_table;
GX_UBYTE language_count;
UINT string_count;

/* Retrieve language table */
status = gx_display_language_table_get(&my_display,
        &language_table, &language_count, &string_count);

/* If status is GX_SUCCESS, the language table has been retrieved.
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_language_table_set
- gx_display_active_langauge_set
- gx_display_string_get
- gx_display_language_table_get_ext

## <a name="gx_display_language_table_get_ext"></a>gx_display_language_table_get_ext

Görüntüleme dili tablosunu al

### <a name="prototype"></a>Prototype

```C
UINT gx_display_language_table_get_ext(
    GX_DISPLAY *display,
    GX_STRING **table, 
    GX_UBYTE *language_count, 
    UINT *string_table_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen görüntülenen dil tablosunu alır. Bu hizmet, bir uygulama tarafından, çalışma zamanında dinamik olarak tanımlanan dizeler kullanılarak görüntüleme dili tablosunu değiştirmek üzere kullanılabilir.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **tablo** Tablo işaretçisinin alınacağı adres
- **language_count** Dil sayısını alacak adres
- **string_table_size** Dize tablosu boyutunu alma adresi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yazı tipi tablo kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING **language_table;
GX_UBYTE language_count;
UINT string_count;

/* Retrieve language table */
status = gx_display_language_table_get_ext(&my_display,
    &language_table, &language_count, &string_count);

/* If status is GX_SUCCESS, the language table has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_language_table_set_ext
- gx_display_active_langauge_set
- gx_display_string_get_ext

## <a name="gx_display_language_table_set"></a>gx_display_language_table_set

Görüntüleme dili tablosu ata (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_display_language_table_set(
    GX_DISPLAY *display,
    GX_CHAR **table, 
    GX_UBYTE number_of_languages, 
    UINT number_of_strings);
```

### <a name="description"></a>Açıklama

Bu hizmet kullanımdan kaldırılmıştır ve yeni uygulamalar gx_display_language_table_set_ext () kullanmalıdır. Bu hizmet yalnızca sürüm 5,6 ' den önceki kitaplık sürümlerini hedefleyen Studio tarafından oluşturulan kaynak dosyalarıyla uyumluluk için desteklenir.

Bu hizmet, görüntü tarafından kullanılacak dil tablosunu atar. Bu hizmet normalde Gux Studio tarafından oluşturulan işlev gx_studio_display_configure tarafından çağrılır, ancak uygulama yazılımı tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **tablo** Dil tablosu
- **number_of_languages** Belirtilen tablodaki sütun sayısı
- **number_of_strings** Her tablo sütunundaki dize sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yazı tipi tablo kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR ***language_table= my_app_language_table;

/* Assign language table */
status = gx_display_language_table_set(&my_display, language_table,
5, 232);

/* If status is GX_SUCCESS, the language table has been reassigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_active_language_set
- gx_display_string_get

## <a name="gx_display_language_table_set_ext"></a>gx_display_language_table_set_ext

Görüntüleme dili tablosu ata

### <a name="prototype"></a>Prototype

```C
UINT gx_display_language_table_set_ext(
    GX_DISPLAY *display,
    GX_STRING **table, 
    GX_UBYTE number_of_languages,
    UINT number_of_strings);
```

### <a name="description"></a>Açıklama

Bu hizmet, görüntü tarafından kullanılacak dil tablosunu atar. Bu hizmet normalde Gux Studio tarafından oluşturulan işlev gx_studio_display_configure tarafından çağrılır, ancak uygulama yazılımı tarafından da çağrılabilir.

Çalışma zamanı dil tablosu ataması genellikle gx_binres_language_table_load () kullanılarak bir ikili kaynak dosyasından diller yüklendiğinde yapılır.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **tablo** Dil tablosu
- **number_of_languages** Belirtilen tablodaki sütun sayısı
- **number_of_strings** Her tablo sütunundaki dize sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yazı tipi tablo kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING **language_table = my_app_language_table;

/* Assign the language table */
status = gx_display_language_table_set_ext(&my_display,
    language_table, 5, 132);

/* If status is GX_SUCCESS, the language table has been reassigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_active_language_set
- gx_display_string_get

## <a name="gx_display_pixelmap_table_set"></a>gx_display_pixelmap_table_set

Görüntüleme yazı tipi tablosu ata

### <a name="prototype"></a>Prototype

```C
UINT gx_display_pixelmap_table_set(
    GX_DISPLAY *display,
    GX_PIXELMAP **pixelmap_table, 
    INT table_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, ekran tarafından kullanılacak pixelmap tablosunu yeniden atar. Bu hizmet normalde, Studio tarafından oluşturulan görüntü yapılandırma işlevi tarafından çağrılır, ancak uygulama yazılımı tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **pixelmap_table** GX_PIXELMAP işaretçileri dizisi.
- **table_size** Tablodaki pixelmaps sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bir pixelmap tablosu ayarla
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_PIXELMAP *pixelmap_table[32] = { … };

/* Assign pixelmap table */
status = gx_display_pixelmap_table_set(&my_display, pixelmap_table, 32);

/* If status is GX_SUCCESS the pixelmap table has been reassigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_color_set
- gx_display_color_table_set
- gx_display_font_table_set

## <a name="gx_display_string_get"></a>gx_display_string_get

Etkin dize tablosundan bir dize al (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_display_string_get(
    GX_DISPLAY *display,
    GX_RESOURCE_ID string_id, 
    GX_CONST GX_CHAR **string);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_display_string_get_ext () kullanımı için kullanım dışıdır.

Bu hizmet, belirtilen görüntü için etkin dize tablosundan bir dize alır. Etkin dil, görüntülemeye atanan dil tablosundan dizeyi seçmek için kullanılır.

Dize kimlikleri, GUıDX Studio tarafından oluşturulur ve uygulama kaynakları. h üstbilgi dosyasında bulunur.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **string_id** , GUıDX Studio tarafından oluşturulan dize KIMLIĞI.
- **dize** Dize işaretçisi değişkeninin adresi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı dize alımı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_RESOURCE_ID** (0x33) geçersiz dize kimliği
- **GX_PTR_ERROR** (0x07) geçersiz görüntüleme işaretçisi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR *string;

/* Retrieve string value */
status = gx_display_string_get(&my_display,
    GX_STRING_ID_MONDAY, &string);

/* If status is GX_SUCCESS, the string has been retrieved. */
```


### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_active_language_set
- gx_display_language_table_set

## <a name="gx_display_string_get_ext"></a>gx_display_string_get_ext

Etkin dize tablosundan bir dize al

### <a name="prototype"></a>Prototype

```C
UINT gx_display_string_get_ext(
    GX_DISPLAY *display,
    GX_RESOURCE_ID string_id,
    GX_STRING *string);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen görüntü için etkin dize tablosundan bir dize alır. Etkin dil, görüntülemeye atanan dil tablosundan dizeyi seçmek için kullanılır.

Dize kimlikleri, GUıDX Studio tarafından oluşturulur ve uygulama kaynakları. h üstbilgi dosyasında bulunur.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **string_id** , GUıDX Studio tarafından oluşturulan dize KIMLIĞI.
- **dize** GX_STRING değişkenin adresi
- **String.gx_string_ptr ve**
- **String.gx_string_length** döndürülecek.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı dize alımı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_RESOURCE_ID** (0x33) geçersiz dize kimliği
- **GX_PTR_ERROR** (0x07) geçersiz görüntüleme işaretçisi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING string;

/* Retrieve string value */
status = gx_display_string_get_ext(&my_display,
    GX_STRING_ID_MONDAY, &string);

/* If status is GX_SUCCESS, the string has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_active_language_set
- gx_display_language_table_set


## <a name="gx_display_string_table_get"></a>gx_display_string_table_get


Etkin dize tablosunu alma (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_display_string_table_get(
    GX_DISPLAY *display,
    GX_UBYTE language, 
    GX_CHAR ***table,
    UINT *table_size);
```

### <a name="description"></a>Açıklama

Bu hizmet kullanım dışıdır ve gx_display_string_table_get_ext () ile değiştirilmiştir.

Bu hizmet, etkin dille ilişkili dize tablosunu alır. Bu hizmet sıklıkla kullanılmaz, ancak dize tablosunda çalışma zamanı değişiklikleri yapması gerekebilecek uygulamalar için bu uygulamalar için de verilmiştir.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **dil** Alınacak tablo sütunu.
- **tablo** İşaretçiye döndürülecek değişkenin adresi.
- **table_size** Tablo boyutunun döndürdüğü değişkenin adresi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yazı tipi tablo kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_NOT_FOUND** (0x09) geçersiz dil dizini
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR **string_table;
UINT table_size;

/* Retrieve string table */
status = gx_display_string_table_get(&my_display, LANGUAGE_ENGLISH,
    &string_table, &table_size);

/* If status is GX_SUCCESS, the string table has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_color_set
- gx_display_color_table_set
- gx_display_pixelmap_table_set

## <a name="gx_display_string_table_get_ext"></a>gx_display_string_table_get_ext


Etkin dize tablosunu alma

### <a name="prototype"></a>Prototype

```C
UINT gx_display_string_table_get(
    GX_DISPLAY *display,
    GX_UBYTE language, 
    GX_STRING **table, 
    UINT *table_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, etkin dille ilişkili dize tablosunu alır. Bu hizmet sıklıkla kullanılmaz, ancak dize tablosunda çalışma zamanı değişiklikleri yapması gerekebilecek uygulamalar için bu uygulamalar için de verilmiştir.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **dil** Alınacak tablo sütunu.
- **tablo** İşaretçiye döndürülecek değişkenin adresi.
- **table_size** Tablo boyutunun döndürdüğü değişkenin adresi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yazı tipi tablo kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_NOT_FOUND** (0x09) geçersiz dil dizini
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING *string_table;
UINT table_size;

/* Retrieve string table */
status = gx_display_string_table_get_ext(&my_display,
    LANGUAGE_ENGLISH, &string_table, &table_size);

/* If status is GX_SUCCESS, the string table has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_color_set
- gx_display_color_table_set
- gx_display_pixelmap_table_set

## <a name="gx_display_theme_install"></a>gx_display_theme_install


Temaları belirtilen görüntüsüne yükler

### <a name="prototype"></a>Prototype

```C
UINT gx_display_theme_install(
    GX_DISPLAY *display, 
    GX_THEME *theme_table);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen ekranda temaları yükler. Bu hizmet normalde, Studio tarafından oluşturulan görüntü yapılandırma işlevi tarafından çağrılır, ancak uygulama yazılımı tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Görüntüleme denetimi bloğunun işaretçisi
- **theme_table** Yüklenecek Tema tablosu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) Tema tablosu başarıyla yüklendi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz Tema tablosu işaretçisi
- **GX_INVALID_DISPLAY** (0x1d) geçersiz görüntüleme

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_THEME theme_1;

&theme_table[1] = {
    &theme_1,
    …
}

/* Define resource tables. */
GX_COLOR color_table[32] = {…};
GX_FONT *font_table[32] = {…};
GX_PIXELMAP *pixelmap_table[32] = { … };

/* Define scroll appearance. */
GX_SCROLLBAR_APPEARANCE scroll_appearance;

memset(&scroll_appearance, 0, sizeof(GX_SCROLLBAR_APPEARANCE));

scroll_appearance.gx_scroll_width = 20;
scroll_appearance.gx_scroll_thumb_width = 18;
scroll_appearance.gx_scroll_thumb_color =
    GX_COLOR_ID_SCROLL_BUTTON;
scroll_appearance.gx_scroll_thumb_border_color =
    GX_COLOR_ID_SCROLL_BUTTON;
scroll_appearance.gx_scroll_button_color =
    GX_COLOR_ID_SCROLL_BUTTON;
scroll_appearance.gx_scroll_thumb_travel_min = 20;
scroll_appearance.gx_scroll_thumb_travel_max = 20;
scroll appearance.gx_scroll_thumb_border_style =
    GX_STYLE_BORDER_THIN;

theme_1.theme_color_table = color_table;
theme_1.theme_font_table = font_table;
theme_1.theme_pixlemap_table = pixelmap_table;
theme_1.theme_palette = GX_NULL;
theme_1.theme_vertical_scrollbar_appearance = scroll_appearance;
theme_1.theme_horizontal_scrollbar_appearance = scroll_appearance;
theme_1.theme_vertical_scroll_style = GX_SCROLLBAR_RELATIVE_THUMB;
theme_1.theme_horizontal_scroll_style =
    GX_SCROLLBAR_RELATIVE_THUMB;
theme_1.theme_color_table_size = 32;
theme_1.theme_font_table_size = 32;
theme_1.theme_pixelmap_table_size = 32;
theme_1.theme_palette_size = 0;

/* Install theme table. */
status = gx_display_theme_install(&my_display, theme_table);

/* If status is GX_SUCCESS the theme table has been installed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_color_set
- gx_display_color_table_set
- gx_display_font_table_set

## <a name="gx_drop_list_close"></a>gx_drop_list_close


Bırakma listesini kapat

### <a name="prototype"></a>Prototype

```C
UINT gx_drop_list_close(GX_DROP_LIST *drop_list);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen bırakma listesinin açılan listesini kapatır.

### <a name="parameters"></a>Parametreler

- **drop_list** Bırakma listesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bırakma listesi kapatıldı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Close a drop list. */
status = gx_drop_list_close(&drop_list);

/* If status is GX_SUCCESS, the drop list is closed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_drop_list_create
- gx_drop_list_event_process
- gx_drop_list_open

gx_drop_list_pixelmap_set, gx_drop_list_popup_get

## <a name="gx_drop_list_create"></a>gx_drop_list_create


Bırakma listesi oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_drop_list_create(
    GX_DROP_LIST *drop_list, 
    GX_CONST
    GX_CHAR *name, 
    GX_WIDGET *parent,
    INT total_rows, 
    INT open_height,
    VOID (*callback)(GX_VERTICAL_LIST *, 
    GX_WIDGET *, INT),
    ULONG style, 
    USHORT drop_list_id,
    GX_CONST GX_RECTANGLE *size)
```

### <a name="description"></a>Açıklama

Bu hizmet bir bırakma listesi oluşturur. Bırakma listesi, bırakma listesi pencere öğesinin bir birleşimidir ve açılan liste açıldığında görüntülenen bir açılan dikey liste. Açılan liste pencere öğesi oluşturulduğunda açılan dikey liste otomatik olarak oluşturulur ve sırasıyla, açılan liste pencere öğesi açıldığında veya kapandığında görüntülenir veya gizlenir.

Bırakma listesi pencere öğesi iki ilişkili pixelmaps 'ı destekler. İlk olarak, Studio Özellikler görünümünde "duvar kağıdı Listele" olarak açıklanan, açılan liste pencere öğesi açıldığında görüntülenen dikey listenin arka planı olarak görüntülenen isteğe bağlı duvar kağıdı. Studio özellikleri görünümünde "arka plan görüntüsü" olarak tanımlanan ikinci pixelmap, açılan listenin arka planı olarak görüntülenecek isteğe bağlı bir görüntüdür.

Bırakma listesi pencere öğesinin, bırakma listesini açmak ve kapatmak için kullanılan bir alt pencere öğesi olabilir (ancak olması gerekmez). Bu bir simge ya da düğme pencere öğesi geleneksel, ancak üst bırakma listesi için açık/kapatma geçişi olarak özel bir pencere öğesi kullanılabilir. Bu alt pencere öğesinin bırakma listesini işlemesini sağlayan anahtar ayarı, bu alt pencere öğesinin ID_DROP_LIST_BUTTON önceden tanımlanmış pencere öğesi kimliğine sahip olması gerekir.

Bırakma listesine açılan liste, firhazırlama ve alt pencere öğesini açıp kapatan bir alt pencere öğesi tanımlamak için, bu alt öğesini istenen şekilde bırakma listesinde konumlandırın:

![Bırakma listesinin ekran görüntüsü.](./media/guix/image6.jpg)

Daha sonra bu alt pencere öğesini, üst bırakma listesi tarafından tanınan bir iç tanımlı KIMLIK değeri olan ID_DROP_LIST_BUTTON ID değerini atamak için Studio özellikleri görünümünü kullanın:

![Studio özellikleri görünümünün ekran görüntüsü.](./media/guix/image7.jpg)

### <a name="parameters"></a>Parametreler
- **drop_list** Bırakma listesi denetim bloğu işaretçisi
- **ad** Bırakma listesinin adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **total_rows** Bırakma listesindeki toplam satır sayısı
- **open_height** Bırakma listesi açıldığında görünen dikey listenin yüksekliği.
- **geri arama** Liste kaydırıldığında dikey liste tarafından çağrılan işlev. Daha fazla bilgi için GX_VERTICAL_LIST belgelerine bakın.
- **Stil** Açılan liste kenarlığı stili.
- **drop_list_id** Bırakma listesinin uygulama tanımlı KIMLIĞI
- **Boyut** Bırakma listesinin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bırakma listesi oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_DROP_LIST my_drop_list;
VOID list_row_create(GX_VERTICAL_LIST *list,
                     GX_WIDGET *row, INT index);
{
    …
}

GX_RECTANGLE size;

gx_utility_rectangle_define(&size, 10, 10, 80, 40);

status = gx_drop_list_create(&my_drop_list,
    "my drop list", GX_NULL,
    10, 100, list_row_create,
    GX_STYLE_BORDER_RECESSED | GX_STYLE_ENABLED,
    ID_DROP_LIST, &size)

/* Is status is GX_SUCCESS, the drop list was successfully created. */
```

### <a name="see-also"></a>Ayrıca bkz:

- gx_drop_list_close
- gx_drop_list_event_process
- gx_drop_list_open
- gx_drop_list_pixelmap_set
- gx_drop_list_popup_get

## <a name="gx_drop_list_event_process"></a>gx_drop_list_event_process


Bırakma listesi olayını işle

### <a name="prototype"></a>Prototype

```C
UINT gx_drop_list_event_process(
    GX_DROP_LIST *list, 
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet bırakma listesi için bir olayı işler.

### <a name="parameters"></a>Parametreler

- **drop_list** Bırakma listesi pencere öğesi denetim bloğu
- **olay** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) bırakma listesi olayını başarıyla işledi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic drop list event processing as part of custom event processing function. */

UINT custom_drop_list_event_process(GX_DROP_LIST *drop_list,
    GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;
    default:
        /* Pass all other events to the default drop list
            event processing */
        status = gx_drop_list_event_process(drop_list, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_drop_list_close
- gx_drop_list_create
- gx_drop_list_open
- gx_drop_list_pixelmap_set
- gx_drop_list_popup_get

## <a name="gx_drop_list_open"></a>gx_drop_list_open


Bırakma listesi açma

### <a name="prototype"></a>Prototype

```C
UINT gx_drop_list_open(GX_DROP_LIST *drop_list);
```

### <a name="description"></a>Açıklama

Bu hizmet önceden oluşturulmuş bir bırakma listesini açar.

### <a name="parameters"></a>Parametreler

- **drop_list** Bırakma listesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bırakma listesi oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_DROP_LIST mylist;

/* Open the popup list of “mylist”. */
status = gx_drop_list_open(&mylist);

/* If status == GX_SUCCESS, the popup list of “mylist” has been displayed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_drop_list_close
- gx_drop_list_create
- gx_drop_list_event_process
- gx_drop_list_pixelmap_set
- gx_drop_list_popup_get

## <a name="gx_drop_list_pixelmap_set"></a>gx_drop_list_pixelmap_set


Bırakma listesine bir arka plan görüntüsü atama

### <a name="prototype"></a>Prototype

```C
UINT gx_drop_list_pixelmap_set(
    GX_DROP_LIST *drop_list,
    GX_RESOURCE_ID id);
```

### <a name="description"></a>Açıklama

Bırakma listesine bir arka plan görüntüsü atayın. Bu pixelmap, liste açıldığında görüntülenen açılan dikey liste için değil, bırakma listesi pencere öğesinin kendisi için arka plan olarak kullanılır. Açılan liste açılır listesine bir pixelmap atamak için, önce açılan listeye bir işaretçi almak üzere gx_drop_list_popup_get çağırmanız ve sonra bu açılan listeye bir pixelmap atamak için gx_window_wallpaper_set () kullanmanız gerekir.

### <a name="parameters"></a>Parametreler

- **drop_list** Bırakma listesi denetim bloğu işaretçisi
- piksellimap 'e ait **kimlik** kaynak kimliği

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bırakma listesi pixelmap kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_RESOURCE_ID** (0x33) geçersiz pikseltamap kimliği

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_DROP_LIST mylist;

/* create the drop list here */

/* Assign a pixelmap id, which will turn on the list button */
status = gx_drop_list_pixelmap_set(&mylist,
    GX_PIXELMAP_ID_DROP_LIST_BACKGROND);

/* If status is GX_SUCCESS, the pixelmap was successfully set. */
```

### <a name="see-also"></a>Ayrıca bkz:

- gx_drop_list_close
- gx_drop_list_create
- gx_drop_list_event_process
- gx_drop_list_open
- gx_drop_list_popup_get

## <a name="gx_drop_list_popup_get"></a>gx_drop_list_popup_get


Açılan dikey listeye yönelik işaretçiyi al

### <a name="prototype"></a>Prototype

```C
UINT gx_drop_list_popup_get(
    GX_DROP_LIST *drop_list,
    GX_VERTICAL_LIST **return_list);
```

### <a name="description"></a>Açıklama

Bir bırakma listesi pencere öğesi, açılan liste pencere öğesinin kendisinden oluşur ve açılan liste pencere öğesi açıldığında görüntülenen bir açılan pencere dikey listesidir. Bu hizmet, bırakma listesinin dikey liste bileşenine bir işaretçi alır ve uygulamanın API hizmetlerini doğrudan bu dikey listede çağırmasına izin verir.

### <a name="parameters"></a>Parametreler

- **drop_list** Bırakma listesi denetim bloğu işaretçisi
- **return_list** Bırakma listesinde depolanan dikey liste işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) açılır dikey liste başarıyla alındı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_DROP_LIST drop_list;
GX_VERTICAL_LIST *vertical_list;

/* Retrieve the popup list of “drop_list”. */
status = gx_drop_list_popup_get(&drop_list, &vertical_list)

/* If status is GX_SUCCESS, the popup list was successfully retrieved. */
```

### <a name="see-also"></a>Ayrıca bkz:

- gx_drop_list_close
- gx_drop_list_create
- gx_drop_list_open
- gx_drop_list_pixelmap_set

## <a name="gx_horizontal_list_children_position"></a>gx_horizontal_list_children_position


Yatay liste için alt öğe Konumlandır

### <a name="prototype"></a>Prototype

```C
UINT gx_horizontal_list_children_position(GX_HORIZONTAL_LIST *horizontal_list);
```

### <a name="description"></a>Açıklama

Bu işlev, yatay listenin alt öğelerini konumlandırır. Liste GX_EVENT_SHOW olayını aldığında bu işlev otomatik olarak çağrılır, ancak liste görünür yapıldıktan sonra değiştirilirse doğrudan çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **horizontal_list** Yatay liste denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) yatay listenin alt öğeleri başarıyla yerleştirildi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Position children in the horizontal list */
status = gx_horizontal_list_children_position (&horizontal_list);

/* If status is GX_SUCCESS the children in the horizontal list are positioned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_list_create
- gx_horizontal_list_event_process
- gx_horizontal_list_page_index_set
- gx_horizontal_list_selected_index_get
- gx_horinzontal_list_selected_widget_get
- gx_horizontal_list_selected_set
- gx_horizontal_list_total_columns_set

## <a name="gx_horizontal_list_create"></a>gx_horizontal_list_create


Yatay liste oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_horizontal_list_create(
    GX_HORIZONTAL_LIST *horizontal_list,
    GX_CONST GX_CHAR *name, 
    GX_WIDGET *parent,
    INT total_columns,
    VOID (*callback)(GX_HORIZONTAL_LIST *, 
    GX_WIDGET *, INT),
    ULONG style, 
    USHORT horizontal_list_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet yatay bir liste oluşturur.

### <a name="parameters"></a>Parametreler

- **horizontal_list** Yatay liste pencere öğesi denetim bloğu
- **ad** Yatay listenin adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **total_columns** Yatay listedeki toplam comumns sayısı
- **geri arama** Bu, uygulama tarafından sağlanmış bir geri çağırma işlevine yönelik bir işaretçidir. Yeni görünür liste öğelerini oluşturmak için yatay liste kaydırıldığında geri çağırma işlevi çağrılır. Bu şekilde yatay liste, Kullanıcı tanımlı pencere öğesi türünü liste öğeleri olarak görüntüleyebilir.
- **Stil** ScrollBar pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **horizontal_list_id** Yatay listenin uygulama tanımlı KIMLIĞI
- **Boyut** Horitzgen listesinin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) yatay liste başarıyla oluşturuldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_VALUE** (0x22) sütun sayısı geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create horizontal list “my_list” with 5 columns. */
status = gx_horizontal_list_create(&my_list, “my_list”, &my_parent,
    5, callback, GX_STYLE_WRAP, MY_LIST_ID, &size);

/* If status is GX_SUCCESS the horizontal list “my_list” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_list_children_position
- gx_horizontal_list_event_process
- gx_horizontal_list_page_index_set
- gx_horizontal_list_selected_index_get
- gx_horinzontal_list_selected_widget_get
- gx_horizontal_list_selected_set
- gx_horizontal_list_total_columns_set

## <a name="gx_horizontal_list_event_process"></a>gx_horizontal_list_event_process


Yatay liste olayını işle

### <a name="prototype"></a>Prototype

```C
UINT gx_horizontal_list_event_process(
    GX_HORIZONTAL_LIST *list,
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet, yatay liste için bir olayı işler.

### <a name="parameters"></a>Parametreler

- **liste** Yatay liste pencere öğesi denetim bloğu
- **olay** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) yatay liste olayı başarıyla işlendi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic horizontal list event processing as part of custom event processing function. */

UINT custom_list_event_process(
    GX_HORIZONTAL_LIST *list,
    GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;
    default:
        /* Pass all other events to the default horizontal
        list event processing */
        status =
        gx_horizontal_list_event_process(list, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_list_children_position
- gx_horizontal_list_create
- gx_horizontal_list_page_index_set
- gx_horizontal_list_selected_index_get
- gx_horinzontal_list_selected_widget_get
- gx_horizontal_list_selected_set
- gx_horizontal_list_total_columns_set

## <a name="gx_horizontal_list_page_index_set"></a>gx_horizontal_list_page_index_set


Başlangıç sayfası dizinini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_horizontal_list_page_index_set(
    GX_HORIZONTAL_LIST *list,
    INT *index);
```

### <a name="description"></a>Açıklama

Bu hizmet, yatay listenin başlangıç dizinini ayarlar.

### <a name="parameters"></a>Parametreler

- **liste** Yatay liste pencere öğesi denetim bloğu
- **Dizin** Yeni üst Dizin

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) yatay liste için başlangıç sayfası dizinini başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE** (0x22) geçersiz değer

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Sets the starting page index of horizontal list “my_list” as 1. */
status = gx_horizontal_list_page_index_set(&my_list, 1);

/* If status is GX_SUCCESS the starting page index of “my_list” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_list_children_position
- gx_horizontal_list_create
- gx_horizontal_list_event_process
- gx_horizontal_list_selected_index_get
- gx_horinzontal_list_selected_widget_get
- gx_horizontal_list_selected_set
- gx_horizontal_list_total_columns_set

## <a name="gx_horizontal_list_selected_index_get"></a>gx_horizontal_list_selected_index_get


Seçili giriş dizinini yatay listeden Al

### <a name="prototype"></a>Prototype

```C
UINT gx_horizontal_list_selected_index_get(
    GX_horizobntal_LIST *horizontal_list,
    INT *return_index);
```

### <a name="description"></a>Açıklama

Bu hizmet, yatay listenin seçili liste girişi dizinini döndürür.

### <a name="parameters"></a>Parametreler

- **horizontal_list** Yatay liste pencere öğesi denetim bloğu
- **return_index** Dönüş listesi dizini hedefi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı oldu yatay liste girişi alındı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
INT current_index_entry;

/* Get the list entry at the current index of horizontal list “my_list”. */
status = gx_horizontal_list_selected_index_get(&my_list,
    &current_index_entry);

/* If status is GX_SUCCESS, “current_index_entry” contains the current list selection index. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_list_children_position
- gx_horizontal_list_create
- gx_horizontal_list_event_process
- gx_horizontal_list_page_index_set
- gx_horinzontal_list_selected_widget_get
- gx_horizontal_list_selected_set
- gx_horizontal_list_total_columns_set

## <a name="gx_horizontal_list_selected_set"></a>gx_horizontal_list_selected_set


Seçili girişi yatay bir listede ata

### <a name="prototype"></a>Prototype

```C
UINT gx_horizontal_list_selected_set(
    GX_HORIZONATAL_LIST *horizontal_list,
    INT index);
```

### <a name="description"></a>Açıklama

Bu hizmet seçili girişi yatay bir listede atar. Gerekirse, yatay liste kaydırılacak ve seçili girişin görünür hale getirir.

### <a name="parameters"></a>Parametreler

- **horizontal_list** Yatay liste pencere öğesi denetim bloğu
- **Dizin** Yeni liste girişinin dizin tabanlı konumu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) yatay liste girişini başarıyla ayarladı
- **GX_FAILURE** (0x10) dizini geçersiz aralıkta değil
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the list entry of “my_list” to the child in line 12. */
status = gx_horizontal_list_selected_set(&my_list, 12);

/* If status is GX_SUCCESS, the list entry of “my_list” has been successfully set to 12. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_list_children_position
- gx_horizontal_list_create
- gx_horizontal_list_event_process
- gx_horizontal_list_page_index_set
- gx_horizontal_list_selected_index_get
- gx_horinzontal_list_selected_widget_get
- gx_horizontal_list_total_columns_set

## <a name="gx_horizontal_list_selected_widget_get"></a>gx_horizontal_list_selected_widget_get


Seçili girişi yatay listeden Al

### <a name="prototype"></a>Prototype

```C
UINT gx_horizontal_list_selected_widget_get(
    GX_horizobntal_LIST *horizontal_list,
    GX_WIDGET **return_list_entry);
```

### <a name="description"></a>Açıklama

Bu hizmet, yatay listenin seçili liste girişini döndürür. Yatay listede alt pencere öğelerinin daha fazla satır varsa ve seçili giriş görünümden kaydırıldığında, bu API GX_NULL döndürür çünkü alt pencere öğeleri liste içeriği kaydırıldığında yeniden kullanılır. Bu öğe görünümden kaydırıldığında bile gx_horizontal_list_selected_index_get işlevi, seçili öğenin dizinini güvenilir bir şekilde döndürür.

### <a name="parameters"></a>Parametreler

- **horizontal_list** Yatay liste pencere öğesi denetim bloğu
- **return_list_entry** Dönüş listesi girdisi pencere öğesi hedefi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı oldu yatay liste girişi alındı
- **GX_FAILURE** (0x10) seçili pencere öğesi, istemci alt öğelerinden daha fazla satır içeren bir listede görünümden kaydırıldı.
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Get the list entry at the current index of horizontal list “my_list”. */
status = gx_horizontal_list_selected_widget_get(&my_list, &current_list_entry);

/* If status is GX_SUCCESS, “current_list_entry” contains a pointer to the currently selected widget. */

    
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_list_children_position
- gx_horizontal_list_create
- gx_horizontal_list_event_process
- gx_horizontal_list_page_index_set
- gx_horizontal_list_selected_index_get
- gx_horizontal_list_selected_set
- gx_horizontal_list_total_columns_set

## <a name="gx_horizontal_list_total_columns_set"></a>gx_horizontal_list_total_columns_set


Liste sütunlarının toplam sayısını ata

### <a name="prototype"></a>Prototype

```C
UINT gx_horizontal_list_total_columns_set(
    GX_HORIZONTAL_LIST *horizontal_list,
    INT count);
```

### <a name="description"></a>Açıklama

Bu hizmet, yatay liste tarafından görüntülenecek toplam sütun sayısını atar.

### <a name="parameters"></a>Parametreler

- **horizontal_list** Yatay liste pencere öğesi denetim bloğu
- **sayı** Görüntülenecek sütun sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı atanan sütun sayısı
- **GX_CALLER_ERROR** (0x10) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE** (0x22) geçersiz sayı değeri

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Tell my list to display 20 total columns. */
status = gx_horizontal_list_total_columns_set(&my_list, 20);

/* If status is GX_SUCCESS, the total colums of “my_list” was successfully set to 20. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_list_children_position
- gx_horizontal_list_create
- gx_horizontal_list_event_process
- gx_horizontal_list_page_index_set
- gx_horizontal_list_selected_index_get
- gx_horinzontal_list_selected_widget_get
- gx_horizontal_list_selected_set

## <a name="gx_horizontal_scrollbar_create"></a>gx_horizontal_scrollbar_create


Yatay kaydırma çubuğu oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_horizontal_scrollbar_create(
    GX_SCROLLBAR *scrollbar,
    GX_CONST GX_CHAR *name,
    GX_WINDOW *parent,
    GX_SCROLLBAR_APPEARANCE *appearance ULONG style);
```

### <a name="description"></a>Açıklama

Bu hizmet yatay bir kaydırma çubuğu oluşturur. Yatay kaydırma çubuğunun KIMLIĞI önceden tanımlanmıştır (bir pencere bundan sonra olayları nasıl yakalayacağından emin olmak için) ve boyut otomatik (üst pencerenin istemci genişliğini doldurmaları gerektiğinden). İstemci alanı kaydırma çubuklarında izin vermeye karar verirse, kimlik ve boyut parametreleriyle başka bir oluşturma işlevi eklememiz gerekir.

### <a name="parameters"></a>Parametreler

- **kaydırma çubuğu** ScrollBar pencere öğesi denetim bloğu
- **ad** Kaydırma çubuğunun adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **Görünüm** Görünüm yapısı, kaydırma çubuğunun görünümünü tanımlar. Bu değer GX_NULL ise, kaydırma çubuğu gx_system_scroll_appearance_get tarafından tanımlanan varsayılan kaydırma çubuğu görünümünü kullanır. GX_SCROLLBAR_APPEARANCE yapısının tanımı için **Ek I** ' ye başvurun.
- **Stil** ScrollBar pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yatay kaydırma çubuğu oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create horizontal scrollbar “my_scrollbar”. */
status = gx_horizontal_scrollbar_create(&my_scrollbar,
    “my_horizontal_scrollbar”, &my_parent, GX_NULL,
    GX_STYLE_SCROLLBAR_END_BUTTONS);

/* If status is GX_SUCCESS the horizontal scrollbar “my_scrollbar” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_scrollbar_draw
- gx_scrollbar_event_process
- gx_scrollbar_limit_check
- gx_scrollbar_reset
- gx_vertical_scrollbar_create

## <a name="gx_icon_button_create"></a>gx_icon_button_create


Simge Oluştur düğmesi

### <a name="prototype"></a>Prototype

```C
UINT gx_icon_button_create(
    GX_ICON_BUTTON *button,
    GX_CONST GX_CHAR *name, 
    GX_WIDGET *parent,
    GX_RESOURCE_ID icon_id,
    ULONG style,
    USHORT icon_button_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen simge düğmesi pencere öğesini oluşturur.

GX_ICON_BUTTON GX_BUTTON türetilir ve tüm gx_button API hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **düğme** Simge düğmesi denetim bloğuna işaretçi
- **ad** Simge düğmesi pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **icon_id** Simgenin kaynak KIMLIĞI
- **Stil** Simgenin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **icon_button_id** Uygulama tanımlı simge düğmesi KIMLIĞI
- **Boyut** Simge düğmesi boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarıyla oluşturuldu simge düğmesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_icon_button”. */
status = gx_icon_button_create(&my_icon_button, “my_icon_button”,
    &my_parent,
    MY_ICON_RESOURCE_ID, GX_STYLE_BORDER_RAISED, MY_ICON_BUTTON_ID,
    &size);

/* If status is GX_SUCCESS the icon button “my_icon_button” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_create
- gx_icon_draw
- gx_icon_pixelmap_set
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_radio_button_create
- gx_radio_button_draw gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_icon_button_draw"></a>gx_icon_button_draw


Bir simge düğmesi çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_icon_button_draw(GX_ICON_BUTTON *button);
```

### <a name="description"></a>Açıklama

Bu hizmet, simge düğmesini çizer. Bu işlev normalde bir tuval yenileme işleminin parçası olarak Gux tarafından dahili olarak çağrılır, ancak özel bir çizim işlevi sağlamak ve varsayılan simge düğme çizimini özel çizim temeli olarak çağırmak isteyebileceğiniz uygulamaya de sunulur.

### <a name="parameters"></a>Parametreler

- **düğme** Simge düğmesi denetim bloğuna işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom icon draw function. */
void MyIconButtonDraw(GX_ICON_BUTTON *button)
{
    /* Do the normal drawing first */
    gx_icon_button_draw(button);

    /* Add custom drawing here */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_create
- gx_icon_draw
- gx_icon_pixelmap_set
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_radio_button_create
- gx_radio_button_draw gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_icon_button_pixelmap_set"></a>gx_icon_button_pixelmap_set


Pixelmap 'i simge düğmesi pencere öğesine ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_icon_button_pixelmap_set(
    GX_ICON_BUTTON *button,
    GX_RESOURCE_ID icon_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, simge düğmesi pencere öğesine yeni bir pixelmap atar.

### <a name="parameters"></a>Parametreler

- **düğme** Simge düğmesi denetim bloğuna işaretçi
- **icon_id** Pixelmap kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) simge düğmesi pixelmap başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set pixelmap for “my_icon_button”. */
status = gx_icon_button_pixelmap_set(&my_icon_button,
    GX_PIXELMAP_ID_ICON);

/* If status is GX_SUCCESS, the pixelmap of the icon button “my_icon_button” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_create
- gx_icon_draw
- gx_icon_pixelmap_set
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_radio_button_create
- gx_radio_button_draw gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_icon_background_draw"></a>gx_icon_background_draw


Çizim simgesi arka planı

### <a name="prototype"></a>Prototype

```C
VOID gx_icon_background_draw(GX_ICON *icon);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen simge pencere öğesinin arka planını çizer. Bu hizmet, genellikle gx_icon_button_draw işlevi tarafından dahili olarak çağrılır, ancak özel çizim işlevleri yazma konusunda yardımcı olmak için uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **simge** Simge pencere öğesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom icon draw function. */
void MyIconButtonDraw(GX_ICON *icon)
{
    /* Call icon background draw. */
    gx_icon_background_draw(icon);

    /* Add custom drawing here */

    /* Draw child widgets. */
    gx_widget_children_draw(icon);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_icon_create
- gx_icon_draw
- gx_icon_event_process
- gx_icon_pixelmap_set

## <a name="gx_icon_create"></a>gx_icon_create


Oluştur simgesi

### <a name="prototype"></a>Prototype

```C
UINT gx_icon_create(
    GX_ICON *icon, 
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_RESOURCE_ID pixelmap_id, 
    ULONG style,
    USHORT icon_id, 
    GX_VALUE x, 
    GX_VALUE y);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen simge pencere öğesini oluşturur.

### <a name="parameters"></a>Parametreler

- **simge** Simge Denetim bloğu işaretçisi
- **ad** Simge pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **pixelmap_id** Pixelmap kaynak KIMLIĞI
- **Stil** Simgenin stili
- **icon_id** Uygulama tanımlı simgenin KIMLIĞI
- **x x koordinatı konumunu başlatma**
- y koordinatı konumunu **y** başlatılıyor

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı simge oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_icon”. */
status = gx_icon_create(&my_icon, “my_icon”, &my_parent,
    MY_PIXELMAP_RESOURCE_ID, GX_STYLE_BORDER_RAISED, MY_ICON_ID,
    5, 30);

/* If status is GX_SUCCESS the icon “my_icon” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_icon_button_create
- gx_icon_draw
- gx_icon_pixelmap_set

## <a name="gx_icon_draw"></a>gx_icon_draw


Çizim simgesi

### <a name="prototype"></a>Prototype

```C
VOID gx_icon_draw(GX_ICON *icon);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen simge pencere öğesini çizer. Bu hizmet, bir tuval yenileme işleminin parçası olarak normalde GUıDX tarafından dahili olarak çağrılır, ancak özel bir çizim işlevi sağlamak ve varsayılan simge çizimini özel çizim temeli olarak çağırmak isteyebileceğiniz uygulamaya de sunulur.

### <a name="parameters"></a>Parametreler

- **simge** Simge pencere öğesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom icon drawing function. */

VOID my_icon_draw(GX_MENU *menu)
{
    /* Call default icon draw. */
    gx_icon_draw(menu);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_icon_button_create
- gx_icon_create
- gx_icon_pixelmap_set

## <a name="gx_icon_event_process"></a>gx_icon_event_process

Simge pencere öğesi olay işleme

### <a name="prototype"></a>Prototype

```C
UINT gx_icon_event_process(
    GX_ICON *icon, 
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet GX_ICON bir pencere öğesine gönderilen olayları işler.

### <a name="parameters"></a>Parametreler

- **simge** Simge pencere öğesi denetim bloğu işaretçisi
- **event_ptr** GX_EVENT yapısına yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı işlenen simge olayı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
switch(event_ptr->gx_event_type)
{
case GX_EVENT_SHOW:
    /* Do default handling. */
    status = gx_icon_event_process(icon, event_ptr);

    /* add your own handling here */
    break;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_icon_button_create
- gx_icon_create
- gx_icon_pixelmap_set

## <a name="gx_icon_pixelmap_set"></a>gx_icon_pixelmap_set


Simgeye yönelik pixelmap ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_icon_pixelmap_set(
    GX_ICON *icon, 
    GX_RESOURCE_ID normal_id,
    GX_RESOURCE_ID selected_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen simge pencere öğesi için pixelmap 'i ayarlar.

### <a name="parameters"></a>Parametreler

- **simge** Simge pencere öğesi denetim bloğu işaretçisi
- **normal_id** Normal durum kaynak KIMLIĞI
- **selected_id** Seçili durum kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı simgesi pixelmap kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set pixelmap for “my_icon”. */
status = gx_icon_pixelmap_set(&my_icon,
    MY_NOT_SELECTED_RESOURCE_ID,
    MY_SELECTED_ID);

/* If status is GX_SUCCESS, the icon “my_icon” has a pixelmap set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_icon_button_create
- gx_icon_create
- gx_icon_draw

## <a name="gx_image_reader_create"></a>gx_image_reader_create


Görüntü okuyucu modülü örneği oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_image_reader_create(
    GX_IMAGE_READER *image_reader,
    GX_CONST GX_UBYTE *data, 
    INT data_size,
    GX_UBYTE color_format, 
    GX_UBYTE mode);
```

### <a name="description"></a>Açıklama

Bu işlev, bir çalışma zamanı Ham görüntü okuyucu/kod çözücü oluşturur. Şu anda yalnızca JPEG ve PNG RAW görüntü türleri desteklenir. Bu hizmet için GX_SOFTWARE_DECODER_SUPPORT tanımlanması gerekir.

### <a name="parameters"></a>Parametreler

- **image_reader** Görüntü okuyucu denetim bloğu
- **veri** Ham giriş verilerine yönelik işaretçi.
- **data_size** Ham giriş verilerinin boyutu.
- **color_format** İstenen çıkış rengi biçimi.
- **mod** Sıkıştır, titrek ve alfa modları bayrakları.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı görüntü okuyucu oluşturma
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE** (0x22) geçersiz veri boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve Iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_IMAGE_READER my_image_reader;

“color format” could be set to:
    GX_COLOR_FORMAT_32ARGB
    GX_COLOR_FORMAT_24RGB
    GX_COLOR_FORMAT_565RGB
    GX_COLOR_FORMAT_8BIT_PALETTE

/* Create image reader “my_image_reader”. */
status = gx_image_reader_create(&my_image_reader, decoder_data,
    decoder_data_size,
    GX_COLOR_FORMAT_32ARGB,
    GX_IMAGE_READER_MODE_COMPRESS)

/* If status is GX_SUCCESS, “my_image_reader” has been successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_image_reader_start
- gx_image_reader_palette_set

## <a name="gx_image_reader_palette_set"></a>gx_image_reader_palette_set


Görüntü okuyucu paleti tanımlama

### <a name="prototype"></a>Prototype

```C
UINT gx_image_reader_palette_set(
    GX_IMAGE_READER *image_reader,
    GX_COLOR *pal,
    UINT palsize);
```

### <a name="description"></a>Açıklama

Bu hizmet, görüntü okuyucu denetim bloğu için paleti ayarlar. Bu hizmet için GX_SOFTWARE_DECODER_SUPPORT tanımlanması gerekir.

### <a name="parameters"></a>Parametreler

- **image_reader** Görüntü okuyucu denetim bloğu
- **PAL** Palet işaretçisi
- **palsıze** Paletin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı görüntü okuyucu paleti kümesi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE** (0x22) geçersiz palet boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve Iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set “my_palette” as the palette of “my_image_reader”. */
status = gx_image_reader_palette_set(&my_image_reader, my_palette,
    my_palette_size);

/* If status is GX_SUCCESS the palette of “my_image_reader” has been set to “my_palette”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_image_reader_create
- gx_image_reader_start

## <a name="gx_image_reader_start"></a>gx_image_reader_start

Sıkıştırılmış ve dönüştürme işlemini Başlat

### <a name="prototype"></a>Prototype

```C
UINT gx_image_reader_start(
    GX_IMAGE_READER *image_reader, 
    GX_PIXELMAP *outmap);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir ham görüntünün belirtilen renk biçimiyle kodunu çözer. Şu anda yalnızca JPEG ve PNG RAW görüntü türleri desteklenir. Bunun tanımlanması GX_SOFTWARE_DECODER_SUPPORT gerekir.

### <a name="parameters"></a>Parametreler

- **image_reader** Görüntü okuyucu denetim bloğu
- **pixelmap** Çıktı pixelmap

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı görüntü kod çözme
- **GX_SYSTEM_MEMORY_ERROR** (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu
- **GX_NOT_SUPPORTED** (0x28) giriş resmi türü veya çıkış rengi biçimi desteklenmiyor
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve Iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_IMAGE_READER my_image_reader;
GX_PIXELMAP output_map;

/* Create my_image_reader here. */

/* Decoding a raw image according to the settings of “my_image_reader”. */
status = gx_image_reader_start(&my_image_reader, output_map)

/* If status is GX_SUCCESS “output_map” have been loaded with the requested pixelmap. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_image_reader_create
- gx_image_reader_palette_set

## <a name="gx_line_chart_axis_draw"></a>gx_line_chart_axis_draw


Çizgi grafiği x, y ekseni çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_line_chart_axis_draw(GX_LINE_CHART *chart);
```

### <a name="description"></a>Açıklama

Bu hizmet, çizgi grafiğinin x, y eksenini çizer. Eksen renkleri ve çizgi genişliği parametreleri çizgi grafik bilgi yapısından alınır.

Bu hizmet, genellikle gx_line_chart_draw işlevi tarafından dahili olarak çağrılır, ancak özel çizim işlevleri yazma konusunda yardımcı olmak için uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **grafik** Çizgi grafik denetim bloğu.

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom chart drawing function. */

VOID my_chart_draw(GX_LINE_CHART *chart)
{
    /* Call default window draw. */
    gx_window_draw((GX_WINDOW *)chart);

    /* Draw the line chart axis. */
    gx_line_chart_axis_draw(&chart->gx_line_chart_info);

    /* Draw the data line */
    gx_line_chart_data_draw(&chart->gx_line_chart_info);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_line_chart_create
- gx_line_chart_data_draw
- gx_line_chart_draw
- gx_line_chart_update
- gx_line_chart_y_scale_calculate

## <a name="gx_line_chart_create"></a>gx_line_chart_create


GX_LINE_CHART pencere öğesi oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_line_chart_create(
    GX_LINE_CHART *chart,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_LINE_CHART_INFO *info,
    ULONG style,
    USHORT chart_id, GX_RECTANGLE *size)
```

### <a name="description"></a>Açıklama

Bu hizmet bir çizgi grafik penceresi oluşturur. Grafik çizim parametreleri ve grafik verileri GX_LINE_CHART_INFO yapısı aracılığıyla geçirilir.

GX_LINE_CHART GX_WINDOW tabanlıdır ve tüm GX_WINDOW API 'Leri destekler.

### <a name="parameters"></a>Parametreler

- **grafik** GX_LINE_CHART denetim bloğuna yönelik işaretçi.
- **ad** İsteğe bağlı çizgi grafik adı
- **üst öğe** Üst pencere öğesi veya GX_NULL
- **bilgi** Çizgi grafik çizim parametrelerini tanımlayan yapı. **Ek ı** GX_LINE_CHART_INFO yapısına yönelik tanımı içerir.
- **Stil** Pencere öğesi stil bayrakları
- **chart_id** Grafik mantıksal KIMLIĞI değeri
- **Boyut** Grafik penceresi sınırlayıcı dikdörtgeni

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çizgi grafik oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create a line chart */
GX_LINE_CHART chart;
GX_RECTANGLE chart_size;
GX_LINE_CHART_INFO gx_chart_info;
GX_WINDOW_ROOT *root_window;

chart_size = root_window->gx_widget_size;

/* Initialize params for the GUIX base chart. */
gx_chart_info.gx_line_chart_min_val = DATA_MIN_VAL;
gx_chart_info.gx_line_chart_max_val = DATA_MAX_VAL;
gx_chart_info.gx_line_chart_max_data_count = MAX_DATA_COUNT;
gx_chart_info.gx_line_chart_active_data_count = 0;
gx_chart_info.gx_line_chart_axis_line_width = AXIS_LINE_WIDTH;
gx_chart_info.gx_line_chart_data_line_width = DATA_LINE_WIDTH;
gx_chart_info.gx_line_chart_data = chart_data;
gx_chart_info.gx_line_chart_line_color = GX_COLOR_ID_DATA_LINE;
gx_chart_info.gx_line_chart_axis_color = GX_COLOR_ID_AXIS_LINE;

/* Leave room for labels on bottom and right. */
gx_chart_info.gx_line_chart_left_margin = 0;
gx_chart_info.gx_line_chart_top_margin = 0;
gx_chart_info.gx_line_chart_right_margin = 80;
gx_chart_info.gx_line_chart_bottom_margin = 32;

status = gx_line_chart_create(&chart, “Line Chart”, root_window,
    &gx_chart_info, GX_STYLE_NONE, &chart_size);

/* If status is GX_SUCCESS, the “chart” has been successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_line_chart_create
- gx_line_chart_data_draw
- gx_line_chart_draw
- gx_line_chart_update
- gx_line_chart_y_scale_calculate

## <a name="gx_line_chart_data_draw"></a>gx_line_chart_data_draw


Çizgi grafik veri satırı çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_line_chart_data_draw(GX_LINE_CHART *chart);
```

### <a name="description"></a>Açıklama

Bu hizmet çizgi grafik veri çizgisini çizer. Çizgi renkleri ve çizgi genişliği parametreleri çizgi grafik bilgi yapısından alınır.

Bu hizmet, genellikle gx_line_chart_draw işlevi tarafından dahili olarak çağrılır, ancak özel çizim işlevleri yazma konusunda yardımcı olmak için uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **grafik** Çizgi grafik denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom chart drawing function. */

VOID my_chart_draw(GX_LINE_CHART *chart)
{
    /* Call default window draw. */
    gx_window_draw((GX_WINDOW *)chart);

    /* Draw the line chart axis. */
    gx_line_chart_axis_draw(chart);

    /* Draw the data line. */
    gx_line_chart_data_draw(chart);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_line_chart_create
- gx_line_chart_draw
- gx_line_chart_update
- gx_line_chart_y_scale_calculate

## <a name="gx_line_chart_draw"></a>gx_line_chart_draw


Çizgi grafiği çiz

### <a name="prototype"></a>Prototype

```C
UINT gx_line_chart_draw(GX_LINE_CHART *chart);
```

### <a name="description"></a>Açıklama

Bu, Grafik eksenini ve veri çizgisini çizen varsayılan çizgi grafik çizim işlevidir. Uygulamalar genellikle, temel çizgi grafik pencere öğesi tarafından çizilen grafik eksenine ve veri satırına tickiþaretleri, ölçek veya diğer bilgiler gibi şeyler eklemek için varsayılan çizimi değiştirmek üzere özel bir çizim işlevi sağlar.

### <a name="parameters"></a>Parametreler

- **grafik** Çizgi grafik denetim bloğuna yönelik işaretçi.

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom chart drawing function. */

VOID my_chart_draw(GX_LINE_CHART *chart)
{
    /* Call default line chart draw. */
    gx_line_chart_draw(chart);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_line_chart_create
- gx_line_chart_draw
- gx_line_chart_update
- gx_line_chart_y_scale_calculate

## <a name="gx_line_chart_update"></a>gx_line_chart_update


Satır grafik veri satırını güncelleştir

### <a name="prototype"></a>Prototype

```C
UINT gx_line_chart_update(
    GX_LINE_CHART *chart, 
    INT *data,
    INT data_count)
```

### <a name="description"></a>Açıklama

Bu hizmet, çizgi grafik penceresi tarafından çizilen veri dizisini güncelleştirir ve pencereyi yeniden boyutlandırmaya zorlar.

### <a name="parameters"></a>Parametreler

- **grafik** Çizgi grafik denetim bloğu
- **veri** Çizilemek üzere veri dizisi
- **data_count** Veri dizisinin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı metin düğmesi oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
INT chart_data[100];
GX_LINE_CHART chart;

/* Update the data array associated with “chart”. */
status = gx_line_chart_update(&chart, chart_data, 100);

/* If status is GX_SUCCESS, the line chart data has been updated. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_line_chart_create
- gx_line_chart_data_draw
- gx_line_chart_draw
- gx_line_chart_y_scale_calculate

## <a name="gx_line_chart_y_scale_calculate"></a>gx_line_chart_y_scale_calculate


Sabit noktalı y ekseni ölçekleme değerini hesapla

### <a name="prototype"></a>Prototype

```C
UINT gx_line_chart_y_scale_calculate(
    GX_LINE_CHART *chart,
    INT *return_val);
```

### <a name="description"></a>Açıklama

Bu hizmet, grafik Y ekseninde veri değerlerini çizmek için kullanılan sabit nokta ölçekleme değerini hesaplar. Bu ölçekleme değerini hesaplamak için chart_info parametreleri ve grafik sınırlayıcı dikdörtgeni kullanılır.

### <a name="parameters"></a>Parametreler

- **grafik** Çizgi grafik denetim bloğu
- **return_val** Sabit noktalı dönüş değerinin tutulacağı değerin adresi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı y ölçek değeri hesaplaması
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_LINE_CHART chart;
INT y_scale;

/* Caluclate y scale value of “chart”. */
status = gx_line_chart_y_scale_calculate(&chart, &y_scale);

/* If status is GX_SUCCESS, y scale value of “chart” has been calculated. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_line_chart_create
- gx_line_chart_data_draw
- gx_line_chart_draw
- gx_line_chart_update

## <a name="gx_menu_create"></a>gx_menu_create


Menü Oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_menu_create(
    GX_MENU *menu,GX_CONST GX_CHAR *name,
    GX_WIDGET *parent, 
    GX_RESOURCE_ID text_id,
    GX_RESOURCE_ID fill_id, 
    ULONG style, 
    USHORT menu_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen bir menü oluşturur ve menüyü sağlanan üst pencere öğesiyle ilişkilendirir. Alt menü öğesi olarak tüm pencere öğesi türlerini kabul eder. Bir pencere öğesini bir alt menü öğesi olarak eklemek için **gx_menu_insert** çağırın.

GX_MENU GX_PIXELMAP_PROMPT türetilir ve tüm gx_pixelmap_prompt API hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **menü** Menü denetim bloğu işaretçisi
- **ad** Menünün adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **text_id** Metnin kaynak KIMLIĞI
- **fill_id** Dolgunun kaynak KIMLIĞI
- **Stil** Pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **menu_id** Menünün uygulama tanımlı KIMLIĞI
- **Boyut** Menünün boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı menü oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_MENU my_menu;

/* Create “my_menu”. */
status = gx_menu_create(&my_menu, “my_menu”, parent, MY_TEXT_ID,
    MY_FILL_ID, GX_STYLE_ENABLED, MY_MENU_ID,
    &size);

/* If status is GX_SUCCESS, the menu was successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_meu_create
- gx_accordion_menu_draw
- gx_accordion_menu_event_process
- gx_accordion_menu_position
- gx_menu_draw
- gx_menu_event_process
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set

## <a name="gx_menu_draw"></a>gx_menu_draw


Çiz Menüsü

### <a name="prototype"></a>Prototype

```C
VOID gx_menu_draw(GX_MENU *menu);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen menüyü çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel menü pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **menü** Menü denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom menu drawing function. */

VOID my_menu_draw(GX_MENU *menu)
{
    /* Call default menu draw. */
    gx_menu_draw(menu);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_menu_create
- gx_accordion_menu_draw
- gx_accordion_menu_event_process
- gx_accordion_menu_position
- gx_menu_create
- gx_menu_event_process
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set

## <a name="gx_menu_event_process"></a>gx_menu_event_process

İşlem menüsü olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_menu_event_process(GX_MENU *menu, GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen menü için bir olayı işler. Bu hizmet özel bir menü olay işleme işlevleri tarafından varsayılan olay işleyicisi olarak çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **menü** Menü denetim bloğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı menü olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x23) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic menu event processing as part of custom event processing function. */

UINT custom_menu_event_process(GX_MENU *menu, GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */

        /* Call default event process if this is a system event such as GX_EVENT_SHOW. */
        status = gx_menu_event_process(menu, event);
        break;

    default:
        /* Pass all other events to the default menu
           event processing */
        status = gx_menu_event_process(menu, event);
        break;
    }
    return status;
}

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_create
- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set

## <a name="gx_menu_insert"></a>gx_menu_insert


Yeni öğe Ekle

### <a name="prototype"></a>Prototype

```C
UINT gx_menu_insert(
    GX_MENU *menu, 
    GX_WIDGET *insert);
```

### <a name="description"></a>Açıklama

Bu hizmet, menüye yeni bir öğe ekler.

### <a name="parameters"></a>Parametreler

- **menü** Menü denetim bloğu işaretçisi
- **pencere öğesi** Eklenecek pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) yeni öğe menüye başarıyla ekledi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Insert new item “my_widget” to the menu “my_menu”. */
status = gx_menu_insert(&my_menu, &my_widget);

/* If status is GX_SUCCESS the new item “my_widget” has been inserted to the menu “my_menu”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_menu_create
- gx_accordion_menu_draw
- gx_accordion_menu_event_process
- gx_accordion_menu_position
- gx_menu_create
- gx_menu_draw
- gx_menu_event_process
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set

## <a name="gx_menu_remove"></a>gx_menu_remove


Bir öğeyi kaldır

### <a name="prototype"></a>Prototype

```C
UINT gx_menu_remvoe(
    GX_MENU *menu, 
    GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet, menüden bir öğeyi kaldırır.

### <a name="parameters"></a>Parametreler

- **menü** Menü denetim bloğu işaretçisi
- **pencere öğesi** Kaldırılacak pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) menü öğesi başarıyla kaldırıldı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Remove item “my_widget” from menu “my_menu” */
status = gx_menu_remove(&my_menu, &my_widget);

/* If status is GX_SUCCESS the item “my_widget” has been removed from menu “my_menu”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_menu_create
- gx_accordion_menu_draw
- gx_accordion_menu_event_process
- gx_accordion_menu_position
- gx_menu_create
- gx_menu_draw
- gx_menu_event_process
- gx_menu_insert
- gx_menu_text_draw
- gx_menu_text_offset_set

## <a name="gx_menu_text_draw"></a>gx_menu_text_draw


Çiz menü metni

### <a name="prototype"></a>Prototype

```C
VOID gx_menu_text_draw(GX_MENU *menu);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir menünün metnini çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel menü pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **menü** Menü denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom menu drawing function. */

VOID my_menu_draw(GX_MENU *menu)
{
    /* Call default menu background draw. */
    gx_pixelmap_prompt_background_draw(
                            (GX_PIXELMAP_PROMPT *)menu);

    /* Draw menu text. */
    gx_menu_text_draw(menu);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_menu_create
- gx_accordion_menu_draw
- gx_accordion_menu_event_process
- gx_accordion_menu_position
- gx_menu_create
- gx_menu_draw
- gx_menu_event_process
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_offset_set

## <a name="gx_menu_text_offset_set"></a>gx_menu_text_offset_set


Menü metni çiz kaydırmayı ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_menu_text_offset_set(
    GX_MENU *menu, 
    GX_VALUE x_offset,
    GX_VALUE y_offset);
```

### <a name="description"></a>Açıklama

Bu hizmet menü metni için x, y görüntüleme sapmasını ayarlar.

### <a name="parameters"></a>Parametreler

- **menü** Menü denetim bloğu işaretçisi
- **x_offset** Uzaklığa X koordinatı
- **y_offset** Uzaklığa ait Y koordinatı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı Ayarla menü metni çiz boşluğu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set text draw offset of menu “my_menu” to (20, 10). */
status = gx_menu_text_offset_set(&my_menu, 20, 10);

/* If status is GX_SUCCESS the text draw offset of menu “my_menu” has been set to (20, 10). */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_accordion_menu_create
- gx_accordion_menu_draw
- gx_accordion_menu_event_process
- gx_accordion_menu_position
- gx_menu_create
- gx_menu_draw
- gx_menu_event_process
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw

## <a name="gx_multi_line_text_button_create"></a>gx_multi_line_text_button_create


Çok satırlı metin düğmesi oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_button_create(
    GX_MULTI_LINE_TEXT_BUTTON *text_button,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_RESOURCE_ID text_id,
    ULONG style,
    USHORT text_button_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı bir metin düğmesi pencere öğesi oluşturur. Çok satırlı bir metin düğmesi, düğme metnini 1-n satır üzerinde görüntüler. En fazla satır sayısı, varsayılan olarak 4 ' e kadar sabit GX_MULTI_LINE_TEXT_BUTTON_MAX_LINES tanımlanır. Satır sonları, çok satırlı metin düğmesine atanan metin dizesi içinde satır başı ve/veya satır başı + satır besleme çiftleri tarafından ayarlanır.

GX_MULTI_LINE_TEXT_BUTTON GX_TEXT_BUTTON türetilir ve tüm gx_text_button API hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **text_button** Metin düğmesi denetim bloğuna işaretçi
- **ad** Metin düğmesinin mantıksal adı
- **üst öğe** Düğmenin üst pencere öğesi işaretçisi
- **text_id** Metnin kaynak KIMLIĞI
- **Stil** Metin düğmesi stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **text_button_id** Metin düğmesinin uygulama tanımlı KIMLIĞI
- **Boyut** Düğmenin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin düğmesi oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create multi-line text button “my_text_button”. */
status = gx_multi_line_text_button_create(&my_text_button, "my text button",
    &my_parent_window, MY_TEXT_RESOURCE_ID,
    GX_STYLE_BUTTON_TOGGLE, MY_TEXT_BUTTON_ID,
    &size);

/* If status is GX_SUCCESS, the multi-line text button “my_text_button” was created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_button_create
- gx_button_create
- gx_multi_line_text_button_draw
- gx_multi_line_text_button_event_process
- gx_multi_line_text_button_text_set
- gx_multi_line_text_button_text_id_set

## <a name="gx_multi_line_text_button_draw"></a>gx_multi_line_text_button_draw


Çok satırlı metin düğmesi çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_multi_line_text_button_draw(GX_MULTI_LINE_TEXT_BUTTON *button);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin düğmesini çizer. Bu işlev normalde bir tuval yenileme işleminin parçası olarak Gux tarafından dahili olarak çağrılır, ancak özel bir çizim işlevi sağlamak ve özel çizim temeli olarak varsayılan çok satırlı metin düğmesi çizimini çağırmak isteyebileceğiniz uygulamaya de sunulur.

### <a name="parameters"></a>Parametreler

- **düğme** Metin düğmesi denetim bloğuna işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw the text button “my_text_button”. */
void MyButtonDraw(GX_MULTI_LINE_TEXT_BUTTON *button)
{
    /* Do the normal drawing first */
    gx_multi_line_text_button_draw(&my_text_button);

    /* Add custom drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_button_create
- gx_button_create
- gx_multi_line_text_button_draw
- gx_multi_line_text_button_event_process
- gx_multi_line_text_button_text_set
- gx_multi_line_text_button_text_id_set

## <a name="gx_multi_line_text_button_event_process"></a>gx_multi_line_text_button_event_process


Çok satırlı metin düğmesi için varsayılan olay işleme

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_button_event_process(
    GX_MULTI_LINE_TEXT_BUTTON *button,
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin düğmesi pencere öğesi için varsayılan olay işleme işlevidir. Bu işlev, metin düğmesi pencere öğesi için özel olay işleme sağlamak isteyen uygulamalar tarafından erişilebilir hale getirilir.

### <a name="parameters"></a>Parametreler

- **düğme** Metin düğmesi denetim bloğuna işaretçi
- **event_ptr** İşlenecek olay

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) olay başarıyla işlendi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT MyEventHandler(GX_MULTI_LINE_TEXT_BUTTON *button,
    GX_EVENT *event_ptr)
{
    switch(event->gx_event_type)
    {
    case GX_EVENT_SHOW:
        gx_multi_line_text_button_event_process(button, event_ptr);
        /* add custom actions here */
        break;
    default:
        gx_multi_line_text_button_event_process(button, event_ptr);
        break;
    }
    return GX_SUCCESS;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_button_create
- gx_button_create
- gx_multi_line_text_button_draw
- gx_multi_line_text_button_event_process
- gx_multi_line_text_button_text_set
- gx_multi_line_text_button_text_id_set

## <a name="gx_multi_line_text_button_text_draw"></a>gx_multi_line_text_button_text_draw


Çizim desteği işlevi

### <a name="prototype"></a>Prototype

```C
VOID gx_multi_line_text_button_text_draw(GX_MULTI_LINE_TEXT_BUTTON *text_button);
```

### <a name="description"></a>Açıklama

Bu destek işlevi, çok satırlı bir metin düğmesinin metin bölümünü çizer. Bu işlev, gx_multi_line_text_button_draw () tarafından dahili olarak çağrılır ve özel bir çok satırlı metin düğmesi çizim işlevi tanımlayan uygulamalar için kolaylık olarak ayrı bir API olarak sağlanır. Düğme arka plan çizimini özelleştirmek isteyen uygulamalar kendi özel çizim işlevlerini sağlayabilir ve multi_line_text_button_text_draw hizmetini özel çiziminin bir parçası olarak çağırarak arka plan üzerinde düğme metnini çizin.

### <a name="parameters"></a>Parametreler

- **text_button** Metin düğmesi denetim bloğuna işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define a custom drawing function */
VOID my_button_draw(GX_MULTI_LINE_TEXT_BUTTON *button)
{
    /* insert code here to draw button background */

    /* call support function to do text drawing */
    gx_multi_line_text_button_text_draw();

    /* draw child widgets */
    gx_widget_children_draw((GX_WIDGET *) button);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_button_create
- gx_button_create
- gx_multi_line_text_button_draw
- gx_multi_line_text_button_event_process
- gx_multi_line_text_button_text_set
- gx_multi_line_text_button_text_id_set


## <a name="gx_multi_line_text_button_text_id_set"></a>gx_multi_line_text_button_text_id_set


Metin düğmesi için metin kaynak KIMLIĞI ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_button_text_id_set(
    GX_MULTI_LINE_TEXT_BUTTON *text_button,
    RESOURCE_ID string_id)
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen dize kaynak KIMLIĞINI metin düğmesine ayarlar. Dize, metni düğme alanında birden çok satırda görüntülemeyi gören yeni satır karakterleri içerebilir.

### <a name="parameters"></a>Parametreler

- **text_button** Metin düğmesi denetim bloğuna işaretçi
- **string_id** Dizenin kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) DIZE kaynak kimliği 'ni metin düğmesine başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the string ID ”MY_STRING_ID” to the text button “my_text_button”. */
status = gx_multi_line_text_button_text_id_set(
    &my_text_button, MY_STRING_ID);

/* If status is GX_SUCCESS, the string ID MY_STRING_ID was set to “my_text_button”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_button_create
- gx_button_create
- gx_multi_line_text_button_draw
- gx_multi_line_text_button_event_process
- gx_multi_line_text_button_text_set
- gx_multi_line_text_button_text_id_set

## <a name="gx_multi_line_text_button_text_set"></a>gx_multi_line_text_button_text_set


Metin düğmesine metin ata (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_mult_line_text_button_text_set(
    GX_MULTI_LINE_TEXT_BUTTON *text_button,
    GX_CHAR *text);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_multi_line_text_button_text_set_ext () kullanımı için kullanım dışıdır.

Bu hizmet, belirtilen dizeyi metin düğmesine atar. Text_button pencere öğesi stil GX_STYLE_TEXT_COPY ile oluşturulduysa pencere öğesi, atanan metin dizesinin özel bir kopyasını oluşturur ve bu nedenle gx_system_memmory_allocate_set API 'SI bu hizmetin istenmediği bir kez çağrılmalıdır. GX_STYLE_TEXT_COPY etkin değilse, pencere öğesi gelen dizenin özel bir kopyasını oluşturmaz, bu nedenle dize statik veya genel olarak ayrılmış olmalıdır, yani bu bir otomatik veya geçici değişken olmayabilir.

### <a name="parameters"></a>Parametreler

- **text_button** Metin düğmesi denetim bloğuna işaretçi
- NULL ile sonlandırılmış dizeye **metin** işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin düğmeye başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_MEMORY_ERROR** (0x30) bellek ayırıcısı tanımlı değil
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
static GX_CHAR text[] = “myrstring”;

/* Set text to the text button “my_text_button”. */
status = gx_multi_line_text_button_text_set(&my_text_button, text);

/* If status is GX_SUCCESS, the text of “my_text_button” was set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_button_create
- gx_button_create
- gx_multi_line_text_button_draw
- gx_multi_line_text_button_event_process
- gx_multi_line_text_button_text_set
- gx_multi_line_text_button_text_id_set

## <a name="gx_multi_line_text_button_text_set_ext"></a>gx_multi_line_text_button_text_set_ext


Metin düğmesine metin atama

### <a name="prototype"></a>Prototype

```C
UINT gx_mult_line_text_button_text_set_ext(
    GX_MULTI_LINE_TEXT_BUTTON *text_button,
    GX_STRING *string)
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen dizeyi metin düğmesine atar. Text_button pencere öğesi stil GX_STYLE_TEXT_COPY ile oluşturulduysa pencere öğesi, atanan metin dizesinin özel bir kopyasını oluşturur ve bu nedenle gx_system_memmory_allocate_set API 'SI bu hizmetin istenmediği bir kez çağrılmalıdır. GX_STYLE_TEXT_COPY etkin değilse, pencere öğesi gelen dizenin özel bir kopyasını oluşturmaz, bu nedenle dize statik veya genel olarak ayrılmış olmalıdır, yani bu bir otomatik veya geçici değişken olmayabilir.

### <a name="parameters"></a>Parametreler

- **text_button** Metin düğmesi denetim bloğuna işaretçi
- GX_STRING değişkene yönelik **dize** işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin düğmeye başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_MEMORY_ERROR** (0x30) bellek ayırıcısı tanımlı değil
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
static GX_CHAR text[] = “myrstring”;
GX_STRING string;

string.gx_string_ptr = text;
string.gx_string_length = strlen(text);

/* Set text to the text button “my_text_button”. */
status = gx_multi_line_text_button_text_set_ext(&my_text_button, string);

/* If status is GX_SUCCESS, the text of “my_text_button” was set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_button_draw
- gx_multi_line_text_button_event_process
- gx_multi_line_text_button_text_set
- gx_multi_line_text_button_text_id_set

## <a name="gx_multi_line_text_input_backspace"></a>gx_multi_line_text_input_backspace


Çok satırlı metin girişi imleç konumundan önce bir karakter Sil

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_backspace(
    GX_MULTI_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin girişi imleç konumundan önce karakteri siler. Bu hizmet, bir geri anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin girişi geri al
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x23) pencere öğesi geçerli değil
- **GX_FAILURE** (0x10) geçersiz Yazı tipi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Delete a character before the cursor of “my_text_input”. */
status = gx_multi_line_text_input_backspace(&my_text_input);

/* If status is GX_SUCCESS the character before the cursor has been deleted. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_buffer_clear"></a>gx_multi_line_text_input_buffer_clear


Metin girişi arabelleğindeki tüm karakterleri siler

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_buffer_clear(GX_MULTI_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin girişi arabelleğindeki tüm karakterleri siler.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin girişi arabelleği temizle
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* clear input buffer of “my_text_input”. */
status = gx_multi_line_text_input_clear(&my_text_input);

/* If status is GX_SUCCESS the text input widget has emptied its input buffer. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_buffer_get"></a>gx_multi_line_text_input_buffer_get


Metin girişi pencere öğesinin arabellek bilgilerini alır

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_buffer_get(
    GX_MULTI_LINE_TEXT_INPUT *text_input, 
    GX_CHAR **buffer_address,
    UINT *content_size, 
    UINT *buffer_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı bir metin girişi pencere öğesinin arabellek bilgilerini alır.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **buffer_address** Giriş arabelleğinin adresi
- **content_size** Giriş verilerinin bayt sayısı
- **Buffer_size** Giriş arabelleğinin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin al
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR *buffer_address;
UINT context_size;
UINT buffer_size;

/* Retrieves buffer information of “my_text_input” widget. */
status = gx_multi_line_text_input_buffer_get(&my_text_input,
    &buffer_address, &string_size,
    &buffer_size);

/* If status is GX_SUCCESS the value of buffer_address, string_size and buffer_size has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_char_insert"></a>gx_multi_line_text_input_char_insert


Geçerli çok satırlı metin girişi imleç konumuna bir karakter dizesi Ekle (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_char_insert(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    GX_UBYTE *insert_str,
    UINT insert_size);
```

### <a name="description"></a>Açıklama

Bu API kullanım dışıdır ve gx_multi_line_text_input_char_insert_ext () ile değiştirilmiştir.

Bu hizmet, geçerli imleç konumundaki çok satırlı metin girişi dize arabelleğine bir karakter dizesi ekler. Bu hizmet, belirli bir anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **insert_str** Eklenecek UTF-8 biçimi karakter dizesi
- **insert_size** Eklenecek bayt sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) karakter dizesi başarıyla ekledi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) geçersiz dize boyutu
- **GX_FAILURE** (0x10) geçersiz Yazı tipi veya arabellek boyutu dışında

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Insert characters at current cursor position. */
GX_CHAR insert_text[10] = “insert”;
status = gx_multi_line_text_input_char_insert(&my_text_input,
    insert_text,
    GX_STRLEN(insert_text));

/* If status is GX_SUCCESS the multi line text input widget has successfully insert the string. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_char_insert_ext

## <a name="gx_multi_line_text_input_char_insert_ext"></a>gx_multi_line_text_input_char_insert_ext


Geçerli çok satırlı metin girişi imleç konumuna bir karakter dizesi Ekle (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_char_insert_ext(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    GX_CONST GX_STRING *string);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli imleç konumundaki çok satırlı metin girişi dize arabelleğine bir karakter dizesi ekler. Bu hizmet, belirli bir anahtar aşağı olayları alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **dize** Eklenecek UTF-8 kodlu karakter dizesi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) karakter dizesi başarıyla ekledi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) geçersiz dize boyutu
- **GX_FAILURE** (0x10) geçersiz Yazı tipi veya arabellek boyutu dışında
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Insert characters at current cursor position. */
GX_CHAR insert_text[10] = “insert”;
GX_STRING string;

string.gx_string_ptr = insert_text;
string.gx_string_length = strlen(insert_text);

status = gx_multi_line_text_input_char_insert_ext(&my_text_input, &string);

/* If status is GX_SUCCESS the multi line text input widget has successfully inserted the string. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_create"></a>gx_multi_line_text_input_create


Çok satırlı metin girişi oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_create(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    GX_CONST GX_CHAR *name, GX_WINDOW *parent,
    GX_CHAR *input_buffer, UINT buffer_size,
    ULONG style, USHORT text_input_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı bir metin girişi pencere öğesi oluşturur.

GX_MULTI_LINE_TEXT_INPUT GX_MULTI_LINE_TEXT_VIEW türetilir ve tüm gx_multi_line_text_view hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **ad** Metin girişi pencere öğesinin adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **input_buffer** Metin girişi arabelleği işaretçisi
- **Buffer_size** Metin girişi arabelleğinin bayt cinsinden boyutu
- **Stil** Metin girişi pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **text_input_id** Metin girişinin uygulama tanımlı KIMLIĞI
- **Boyut** Metin girişi pencere öğesi boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin girişi oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_WIDGET** (0x12) üst pencere öğesi geçerli değil
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_MULTI_LINE_TEXT_INPUT my_text_input;
GX_CHAR my_buffer[100];
GX_RECTANGLE size;

/* Define widget size. */
gx_utility_rectangle_define(&size, 10, 10, 100, 200);

/* Create multi-line text input widget “my_text_input”. */
status = gx_multi_line_text_input_create(&my_text_input,
    “my_text_input”, &my_parent,
    my_buffer, 100, GX_STYLE_BORDER_RAISED,
    MY_TEXT_INPUT_ID, &size);

/* If status is GX_SUCCESS, the text input “my_text_input” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_cursor_pos_get"></a>gx_multi_line_text_input_cursor_pos_get


Çok satırlı metin girişi imleç konumunu al

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_cursor_pos_get(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    GX_POINT cursor_pos);
```

### <a name="description"></a>Açıklama

Bu hizmet, mult satırı metin girişi imleç konumunu alır.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **cursor_pos** Alınan imleç konumu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) Imleç konumu başarıyla alındı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Retrieve the cursor position of “my_text_input”. */
GX_POINT cursor_pos;
status = gx_multi_line_text_input_cursor_pos_get(&my_text_input,
    &cursor_pos);

/* If status is GX_SUCCESS the cursor position has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_delete"></a>gx_multi_line_text_input_delete


Çok satırlı metin girişi imleç konumundaki karakteri sil

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_delete(GX_MULTI_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin girişi imleç konumundan sonra karakteri siler. Bu hizmet, bir DELETE anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) İmleçten sonra bir karakter başarıyla silindi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_FAILURE** (0x10) geçersiz Yazı tipi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Delete the character after the cursor of “my_text_input”. */
status = gx_multi_line_text_input_delete(&my_text_input);

/* If status is GX_SUCCESS the character after the cursor has been deleted. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_down_arrow"></a>gx_multi_line_text_input_down_arrow


Çok satırlı metin girişi imlecini sonraki satıra taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_down_arrow(GX_MULTI_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin girişi pencere öğesi imlecini sonraki satıra konumlandırır. Bu hizmet, aşağı ok tuşunu basılı bir olay alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin girişi imleci bir sonraki satıra başarıyla taşındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_FAILURE** (0x10) geçersiz Yazı tipi veya çizgi yüksekliği

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move input cursor to the next line. */
status = gx_multi_line_text_input_down_arrow(&my_text_input);

/* If status is GX_SUCCESS, text text input cursor has been moved to the next line. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_end"></a>gx_multi_line_text_input_end


Çok satırlı metin giriş imlecini geçerli satırın sonuna taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_end(GX_MULTI_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin girişi pencere öğesi imlecini geçerli dize satırının sonuna konumlandırır. Bu hizmet, bir son anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin giriş imlecini geçerli satırın sonuna başarıyla taşıdı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move input cursor to the end of current line. */
status = gx_multi_line_text_input_end(&my_text_input);

/* If status is GX_SUCCESS, the multi line text input cursor has been moved to the end of the current line. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_event_process"></a>gx_multi_line_text_input_event_process


Çok satırlı metin girişi için varsayılan olay işleme

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_event_process(
    GX_MULTI_LINE_TEXT_INPUT *input,
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin girişi pencere öğesi için varsayılan olay işleme işlevidir. Bu işlev, çok satırlı bir metin girişi pencere öğesi için özel olay işleme sağlamak isteyen uygulamalar tarafından erişilebilir hale getirilir.

### <a name="parameters"></a>Parametreler

- **düğme** Çok satırlı metin girişi denetim bloğu işaretçisi
- **event_ptr** İşlenecek olay

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) olay başarıyla işlendi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) üst pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT MyEventHandler(GX_MULTI_LINE_TEXT_INPUT *input,
    GX_EVENT *event_ptr)
{
    switch(event->gx_event_type)
    {
    case xyz:
        /* insert custom event handling here */
        break;
    default:
        /* pass all other events to the generic multi line text
            input event processing */
        gx_multi_line_text_input_event_process(input, event_ptr);
        break;
    }
    return GX_SUCCESS;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_fill_color_set"></a>gx_multi_line_text_input_fill_color_set


Çok satırlı metin girişi arka plan rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_fill_color_set(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    GX_RESOURCE_ID normal_fill_color_id,
    GX_RESOURCE_ID selected_fill_color_id,
    GX_RESOURCE_ID disabled_fill_color_id,
    GX_RESOURCE_ID readonly_fill_color_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin girişi pencere öğesi için Fill renkleri atar.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **normal_fill_color_id** Normal durumda kullanılan normal Fill renginin kaynak KIMLIĞI
- **selected_fill_color_id** Pencere öğesi odaklanıldığında kullanılan seçili Fill renginin kaynak KIMLIĞI
- **disabled_fill_color_id** GX_STYLE_ENABLED etkin olmadığında kullanılan devre dışı Fill renginin kaynak KIMLIĞI
- **readonly_fill_color_id** Hem GX_STYLE_ENABLED hem de GX_STYLE_INPUT_READONLY etkin olduğunda kullanılan salt okuma dolgusu renginin kaynak KIMLIĞI.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) çok satırlı metin girişi Için renkler başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set fill colors for the multi-line text input widget “my_text_input”. */

status = gx_multi_line_text_input_fill_color_set(&my_text_input,
    GX_COLOR_ID_NORMAL_FILL,
    GX_COLOR_ID_SELECTED_FILL,
    GX_COLOR_ID_DISABLED_FILL,
    GX_COLOR_ID_READONLY_FILL);

/* If status is GX_SUCCESS, the fill color of “my_text_input” has been successfully set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_home"></a>gx_multi_line_text_input_home


Metin girişi imlecini geçerli satırın başlangıcına taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_home(GX_MULTI_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin girişi imleç konumunu geçerli satırın başlangıcına taşımaktır. Bu hizmet, ana anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) imleci geçerli satırın başlangıcına başarıyla taşındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move cursor to the start of the current line. */
status = gx_multi_line_text_input_home(&my_text_input);

/* If status is GX_SUCCESS the cursor has been moved to the start of the current line. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_left_arrow"></a>gx_multi_line_text_input_left_arrow


Çok satırlı metin giriş imlecini sola bir karakter kaydır

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_left_arrow(GX_MULTI_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet çok satırlı metin giriş imlecini bir karakter sola kaydırır. Bu hizmet, sol tuşu basılı bir olay alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) Imleç sola başarıyla taşındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_FAILURE** (0x10) geçersiz Yazı tipi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move the cursor one character to the left. */
status = gx_multi_line_text_input_left_arrow(&my_text_input);

/* If status is GX_SUCCESS the multi line text input cursor has been moved one character to the left. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_right_arrow"></a>gx_multi_line_text_input_right_arrow


Mult satırı metin giriş imlecini bir karakter sağa taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_right_arrow(GX_MULTI_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet çok satırlı metin giriş imlecini bir karakter sağa kaydırır. Bu hizmet, doğru bir anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) Imleç sağa başarıyla taşındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move cursor one character to the right. */
status = gx_multi_line_text_input_right_arrow(&my_text_input);

/* If status is GX_SUCCESS the text input cursor has been moved one character to the right. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_style_add"></a>gx_multi_line_text_input_style_add


Çok satırlı metin girişi stilleri ekleme

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_style_add(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    ULONG style);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı bir metin girişi pencere öğesine stiller ekler.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **Stil** Eklenecek stiller. **Ek D** tüm pencere öğeleri için önceden tanımlanmış genel stilleri içerir

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin girişi stili ekleme
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Add style GX_STYTLE_CURSOR_ALWAYS to multi-line text input widget “my_text_input”. */
status = gx_multi_line_text_input_style_add(&my_text_input,
    GX_STYLE_CURSOR_ALWAYS);

/* If status is GX_SUCCESS the style GX_STYLE_CURSOR_ALWAYS has been successfully added. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_style_remove"></a>gx_multi_line_text_input_style_remove


Stilleri kaldır

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_remove(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    ULONG style);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen stilleri çok satırlı metin girişi pencere öğesinden kaldırır.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **Stil** Kaldırılacak stiller. **Ek D** tüm pencere öğeleri için önceden tanımlanmış genel stilleri içerir

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin girişi oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Remove style GX_STYLE_CURSOR_ALWAYS from text input widget “my_text_input”. */
status = gx_multi_line_text_input_style_remove(&my_text_input,
    GX_STYLE_CURSOR_ALWAYS);

/* If status is GX_SUCCESS, the style GX_STYLE_CURSOR_ALWAYS has been successfully removed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_style_set"></a>gx_multi_line_text_input_style_set

Çok satırlı metin giriş stillerini ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_style_set(
    GX_MULTI_LINE_TEXT_INPUT *text_input, 
    ULONG style);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı bir metin girişi pencere öğesinin stillerini ayarlar.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **Stil** Ayarlanacak stiller. **Ek D** tüm pencere öğeleri için önceden tanımlanmış genel stilleri içerir

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin girişi stili kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set style GX_STYLE_CURSOR_ALWAYS for text input widget “my_text_input”. */
status = gx_multi_line_text_input_style_set(&my_text_input,
    GX_STYLE_CURSOR_ALWAYS);

/* If status is GX_SUCCESS the text input style has been set */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_text_color_set"></a>gx_multi_line_text_input_text_color_set


Çok satırlı metin girişi metin rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_text_color_set(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    GX_RESOURCE_ID normal_text_color_id,
    GX_RESOURCE_ID selected_text_color_id,
    GX_RESOURCE_ID disabled_text_color_id,
    GX_RESOURCE_ID readonly_text_color_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin girişi pencere öğesi için metin renkleri atar.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi pencere öğesi denetim bloğu
- **normal_fill_color_id** Normal durumda kullanılan normal metin renginin kaynak KIMLIĞI
- **selected_text_color_id** Pencere öğesi odaklanıldığında kullanılan seçili metin renginin kaynak KIMLIĞI
- **disabled_text_color_id** GX_STYLE_ENABLED etkin olmadığında kullanılan devre dışı metin renginin kaynak KIMLIĞI
- **readonly_text_color_id** Hem GX_STYLE_ENABLED hem de GX_STYLE_TEXT_INPUT_READONLY etkin olduğunda kullanılan salt okuma metin renginin kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) çok satırlı metin girişi Için renkler başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set text colors for the multi-line text input widget “my_text_input”. */
status = gx_multi_line_text_input_text_color_set(&my_text_input,
    GX_COLOR_ID_NORMAL_TEXT,
    GX_COLOR_ID_SELECTED_TEXT,
    GX_COLOR_ID_DISABLED_TEXT,
    GX_COLOR_ID_READONLY_TEXT);

/* If status is GX_SUCCESS, the fill colors of “my_text_view” has been successfully set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_text_select"></a>gx_multi_line_text_input_text_select


Metin Seç

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_text_select(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    UINT start_index, UINT end_index);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen başlangıç işaretine ve bitiş işareti dizinine sahip çok satırlı metin girişi metnini seçer ve seçilen metni seçilen Fill ve Text renkleriyle vurgular.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi denetim bloğu işaretçisi
- **start_index** Seçilen ilk karakterin dizini
- **end_index** Son seçili karakterin dizini

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin girişi metin seçimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) dizin değeri geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Select text between index [0, 9]. */
status = gx_multi_line_text_input_text_select(&my_text_input,
    0,9);

/* If status is GX_SUCCESS, the text between 
    index [0, 9] “my_text_input” was selected. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_text_set"></a>gx_multi_line_text_input_text_set


Metin girişine metin atama (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_mult_line_text_input_text_set(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    GX_CHAR *text);
```

### <a name="description"></a>Açıklama

Bu API kullanım dışıdır ve gx_multi_line_text_input_text_set_ext () ile değiştirin.

Bu hizmet, belirtilen dizeyi çok satırlı metin girişine atar. Multi_line_text_input pencere öğesinin giriş arabelleği boyutu dize uzunluğundan küçükse, dize kesilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi denetim bloğu işaretçisi
- NULL ile sonlandırılmış dizeye **metin** işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin, çok satırlı metin girişine başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the string “my string” to the text button “my_text_input”. */
status = gx_multi_line_text_input_text_set(&my_text_input,
    “myrstring”);

/* If status is GX_SUCCESS, the content of “my_text_input” bas been reset. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_text_set_ext

## <a name="gx_multi_line_text_input_text_set_ext"></a>gx_multi_line_text_input_text_set_ext


Metin girişine metin atama

### <a name="prototype"></a>Prototype

```C
UINT gx_mult_line_text_input_text_set(
    GX_MULTI_LINE_TEXT_INPUT *text_input,
    GX_CONST GX_STRING *string);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen dizeyi çok satırlı metin girişine atar. Multi_line_text_input pencere öğesinin giriş arabelleği boyutu dize uzunluğundan küçükse, dize kesilir.

### <a name="parameters"></a>Parametreler

- **text_input** Çok satırlı metin girişi denetim bloğu işaretçisi
- atanacak GX_STRING **dize** işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin, çok satırlı metin girişine başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the string “my string” to the text button “my_text_input”. */
GX_STRING string;
string.gx_string_ptr = “myrstring”;
string.gx_string_length = strlen(string.gx_string_ptr);

status = gx_multi_line_text_input_text_set_ext(&my_text_input,
    &string);

/* If status is GX_SUCCESS, the content of “my_text_input” bas been reset. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_input_up_arrow"></a>gx_multi_line_text_input_up_arrow


Çok satırlı metin girişi imlecini önceki satıra taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_input_up_arrow(GX_MULTI_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin girişi imlecini önceki metin satırına taşIar. Bu hizmet, yukarı ok tuşu aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) imleci önceki satıra başarıyla taşındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move the cursor to the previous line. */
status = gx_multi_line_text_input_up_arrow(&my_text_input);

/* If status is GX_SUCCESS the multi line text input cursor has been moved to the previous line. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_create"></a>gx_multi_line_text_view_create


Çok satırlı metin görünümü oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_view_create(
    GX_MULTI_LINE_TEXT_VIEW *text_view,
    GX_CONST GX_CHAR *name, 
    GX_WINDOW *parent, 
    GX_RESOURCE_ID text_id,
    ULONG style, 
    USHORT text_view_id, 
    GX_CONST GX_RECTANGLE *size);

```

### <a name="description"></a>Açıklama

Bu hizmet bir GX_MULTI_LINE_TEXT_VIEW pencere öğesi oluşturur. Bu pencere öğesi türü GX_WINDOW türetilir ve bu nedenle tüm gx_window API hizmetleri bu pencere öğesi türü ile de kullanılabilir.

### <a name="parameters"></a>Parametreler

- **text_view** Çok satırlı metin görünümü pencere öğesi denetim bloğu
- **ad** Metin görünümü pencere öğesinin adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **text_id** Metin dizesinin kaynak KIMLIĞI
- **Stil** Metin görünümü pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **text_view_id** Uygulama tanımlı metin görünümü KIMLIĞI
- **Boyut** Metin görünümü pencere öğesinin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) çok satırlı metin görünümü pencere öğesi başarıyla oluşturuldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create multi-line text view widget “my_text_view”. */
status = gx_multi_line_text_view_create(&my_text_view,
    “my_text_view”, &my_parent,
    TEXT_STRING_ID, GX_STYLE_BORDER_RAISED,
    MY_TEXT_VIEW_ID, &size);

/* If status is GX_SUCCESS the text view “my_text_view” has been successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_draw"></a>gx_multi_line_text_view_draw


Çok satırlı metin görünümü pencere öğesi çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_multi_line_text_view_draw(GX_MULTI_LINE_TEXT_VIEW * text_view);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı bir metin görünümü pencere öğesi çizer. Bu hizmet, genellikle tuval yenilemesi sırasında dahili olarak çağrılır, ancak özel çok satırlı metin görünümü çizim işlevlerinden de çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_view** Çok satırlı metin görünümü pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom multi line text view drawing function. */

VOID my_multi_line_text_view_draw(GX_MULTI_LINE_TEXT_VIEW *view)
{
    /* Call default multi line text view draw. */
    gx_multi_line_text_view_draw(view);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_event_process"></a>gx_multi_line_text_view_event_process


Çok satırlı metin görünümü olayını işle

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_view_event_process(
    GX_MULTI_LINE_TEXT_VIEW *text_view, 
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı bir metin görünümü pencere öğesi için bir olayı işler.

### <a name="parameters"></a>Parametreler

- **text_view** Çok satırlı metin görünümü pencere öğesi denetim bloğu
- **olay** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı çok satırlı metin görünümü olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom event handler. */
UINT my_event_handler(GX_MULTI_LINE_TEXT_VIEW *view, GX_EVENT *event_ptr)
{
    switch(event->gx_event_type)
    {
    case GX_EVENT_SHOW:
        gx_multi_line_text_view_event_process(view, event_ptr);
        /* Add custom actions here. */
        break;
    default:
        gx_multi_line_text_view_event_process (view, event_ptr);
        break;
    }
    return GX_SUCCESS;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_font_set"></a>gx_multi_line_text_view_font_set


Çok satırlı metin görünümünde kullanılan yazı tipini ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_view_text_id_set(
    GX_MULTI_LINE_TEXT_VIEW *text_view, 
    GX_RESOURCE_ID font_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı bir metin görünümü pencere öğesinin yazı tipini ayarlar.

### <a name="parameters"></a>Parametreler

- **text_view** Çok satırlı metin görünümü pencere öğesi denetim bloğu
- **font_id** Yazı tipinin kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) çok satırlı metin görünümü için yazı tipi başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set font ID FONT_ID to the multi-line text view widget “my_text_view”. */
status = gx_multi_line_text_view_font_set(&my_text_view, FONT_ID);

/* If status is GX_SUCCESS, the text view “my_text_view” will use the specified font to display its text. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_line_space_set"></a>gx_multi_line_text_view_line_space_set


Çok satırlı metin görünümü satır alanını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_view_line_space_set(
    GX_MULTI_LINE_TEXT_VIEW *text_view, 
    GX_BYTE line_space);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin görünümü pencere öğesi için metin satırları arasındaki boşluğu ayarlar.

### <a name="parameters"></a>Parametreler

- **görüntüleme** Çok satırlı metin görünümü pencere öğesi denetim bloğu
- **line_space** Ayarlanacak değer

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) çok satırlı metin görünümü için satır alanı değeri başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

```C
/* Set line space of “my_text_view” to 2. */
status = gx_multi_line_text_view_line_space_set(&my_text_view, 2);

/* If status is GX_SUCCESS, the line space of “my_text_view” has been successfully set to 2. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_scroll_info_get"></a>gx_multi_line_text_view_scroll_info_get

Çok satırlı metin görünümü kaydırma bilgisi al


### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_view_scroll_info_get(
    GX_MULTI_LINE_TEXT_VIEW *text_view, ULONG style,
    GX_SCROLL_INFO *info);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin görünümü kaydırma bilgilerini alır.

### <a name="parameters"></a>Parametreler

- **text_view** Çok satırlı metin görünümü pencere öğesi denetim bloğu
- **Stil** GX_SCROLLBAR_HORIZONTAL veya GX_SCROLLBAR_VERTICAL
- **Bilgi** Kaydırma bilgisi için hedef işaretçisi. **Ek ı** GX_SCROLL_INFO yapısına yönelik tanımı içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin görünümü kaydırma bilgisini başarıyla aldı
- **GX_FAILURE** (0x10) pencere öğesi görünür değil veya metin görünümü yazı tipi kimliği geçerli değil
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_SCROLL_INFO scroll_info;

/* Get scroll information for multi-line text view “my_text_view”. */
status = gx_multi_line_text_view_scroll_info_get(&my_text_view,
    &scroll_info);

/* If status is GX_SUCCESS the “scroll_info” contains the scroll information for multi-line text view “my_text_view”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_text_color_set"></a>gx_multi_line_text_view_text_color_set


Çok satırlı metin görünümü için metin rengini ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_view_text_color_set(
    GX_MULTI_LINE_TEXT_VIEW *text_view,
    GX_RESOURCE_ID normal_text_color_id,
    GX_RESOURCE_ID selected_text_color_id,
    GX_RESOURCe_ID disabled_text_color_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin görünümü pencere öğesine metin rengi atar.

### <a name="parameters"></a>Parametreler

- **text_view** Çok satırlı metin görünümü pencere öğesi denetim bloğu
- **normal_text_color_id** Normal durumda kullanılan normal metin renginin kaynak KIMLIĞI
- **selected_text_color_id** Pencere öğesi odaklanıldığında kullanılan seçili metin renginin kaynak KIMLIĞI
- **disabled_text_color_id** GX_STYLE_ENABLED kullanılan devre dışı metin renginin kaynak KIMLIĞI etkin değil

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) çok satırlı metin görünümü Için renkler başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set text colors for the multi-line text view widget “my_text_view”. */
status = gx_multi_line_text_view_text_color_set(&my_text_view,
    GX_COLOR_ID_NORMAL_TEXT,
    GX_COLOR_ID_SELECTED_TEXT,
    GX_COLOR_ID_DISABLED_TEXT);

/* If status is GX_SUCCESS the text color of “my_text_view” has been successfully set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_text_id_set"></a>gx_multi_line_text_view_text_id_set


Birden çok satırlı metin görünümünde sistem metin dizesi ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_view_text_id_set(
    GX_MULTI_LINE_TEXT_VIEW *text_view, 
    GX_RESOURCE_ID text_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir dizenin kaynak KIMLIĞINI çok satırlı metin görünümü pencere öğesine ayarlar.

### <a name="parameters"></a>Parametreler

- **text_view** Çok satırlı metin görünümü pencere öğesi denetim bloğu
- **text_id** Metin dizesinin kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) çok satırlı metin görünümü için dize kimliği başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set string ID STRING_ID to the multi-line text view widget “my_text_view”. */
status = gx_multi_line_text_view_text_id_set(&my_text_view, STRING_ID);

/* If status is GX_SUCCESS the text id of “my_text_view” has been successfully set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_text_set"></a>gx_multi_line_text_view_text_set


Çok satırlı metin görünümünde Kullanıcı tanımlı dizeyi ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_view_text_set(
    GX_MULTI_LINE_TEXT_VIEW *text_view, 
    GX_CONST GX_CHAR *text);
```

### <a name="description"></a>Açıklama

Bu hizmet, çok satırlı metin görünümü pencere öğesine bir metin dizesi atar. Text_view pencere öğesi stil GX_STYLE_TEXT_COPY ile oluşturulduysa pencere öğesi, atanan metin dizesinin özel bir kopyasını oluşturur ve bu nedenle gx_system_memory_allocate_set API 'SI bu hizmetin istenmediği bir kez çağrılmalıdır. GX_STYLE_TEXT_COPY etkin değilse, pencere öğesi gelen dizenin özel bir kopyasını oluşturmaz ve bu nedenle atanan dize statik veya genel olarak ayrılmış olmalıdır, yani bu bir otomatik veya geçici değişken olmayabilir.

### <a name="parameters"></a>Parametreler

- **text_view** Çok satırlı metin görünümü pencere öğesi denetim bloğu
- **metin** NULL ile sonlandırılmış metin dizesi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) çok satırlı metin görünümü Için dize başarıyla ayarlandı
- **GX_SYSTEM_MEMORY_ERROR** (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set string “my string” to the multi-line text view widget “my_text_view”. */
status = gx_multi_line_text_view_text_set(&my_text_view, “my string”);

/* If status is GX_SUCCESS the text of “my_text_view” has been successfully set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_whitespace_set

## <a name="gx_multi_line_text_view_whitespace_set"></a>gx_multi_line_text_view_whitespace_set


Çok satırlı metin görünümü boşluğu ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_multi_line_text_view_whitespace_set(
    GX_MULTI_LINE_TEXT_VIEW *text_view, 
    GX_UBYTE whitespace);
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesi anahatları ve çok satırlı bir metin görünümü pencere öğesi için istemci alanı arasındaki aralığı ayarlar.

### <a name="parameters"></a>Parametreler

- **text_view** Çok satırlı metin görünümü pencere öğesi denetim bloğu
- **boşluk** Text_view pencere öğesi ile görüntülenmiş metin arasındaki kenar boşluğu genişliği (piksel cinsinden).

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) çok satırlı metin görünümü Için boşluk başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set whitespace of “my_text_view” to 2. */
status = gx_multi_line_text_view_whitespace_set(&my_text_view, 2);

/* If status is GX_SUCCESS the whitespace of “my_text_view” has been successfully set to 2. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_multi_line_text_input_backspace
- gx_multi_line_text_input_buffer_clear
- gx_multi_line_text_input_buffer_get
- gx_multi_line_text_input_char_insert
- gx_multi_line_text_input_create
- gx_multi_line_text_input_cursor_pos_get
- gx_multi_line_text_input_delete
- gx_multi_line_text_input_down_arrow
- gx_multi_line_text_input_end
- gx_multi_line_text_input_event_process
- gx_multi_line_text_input_fill_color_set
- gx_multi_line_text_input_home
- gx_multi_line_text_input_left_arrow
- gx_multi_line_text_input_right_arrow
- gx_mutli_line_text_input_style_add
- gx_multi_line_text_input_style_remove
- gx_multi_line_text_input_style_set
- gx_multi_line_text_input_text_color_set
- gx_multi_line_text_input_text_select
- gx_multi_line_text_input_text_set
- gx_multi_line_text_input_up_arrow
- gx_multi_line_text_view_create
- gx_multi_line_text_view_draw
- gx_multi_line_text_view_event_process
- gx_multi_line_text_view_font_set
- gx_multi_line_text_view_line_space_set
- gx_multi_line_text_view_scroll_info_get
- gx_multi_line_text_view_text_color_set
- gx_multi_line_text_view_text_id_set
- gx_multi_line_text_view_text_set

## <a name="gx_numeric_pixelmap_prompt_create"></a>gx_numeric_pixelmap_prompt_create


Sayısal pixelmap istemi oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_numeric_pixelmap_prompt_create(
    GX_NUMERIC_PIXELMAP_PROMPT *prompt,
    GX_CONST GX_CHAR name, GX_WIDGET *parent,
    GX_RESOURCE_ID text_id, GX_RESOURCE_ID fill_id,
    ULONG style, USHORT pixelmap_prompt_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet sayısal bir pixelmap istemi pencere öğesi oluşturur. Numeric_pixelmap_prompt, kendi arabelleğini tutan ve bir gx_numeric_pixelmap_prompt_value_set (INT) API sağlayan bir pixelmap_prompt, arabellek boyutu sabit GX_NUMERIC_PROMPT_BUFFER_SIZE tarafından tanımlanır, varsayılan olarak 16 ' dır.

GX_NUMERIC_PIXELMAP_PROMPT GX_PIXELMAP_PROMPT türetilir ve tüm gx_pixelmap_prompt API hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **komut istemi** Sayısal pixelmap istem denetim bloğu
- **ad** İstem adı
- **üst öğe** Üst pencere öğesi denetim bloğu
- **text_id** Kaynak dize kimliği
- **fill_id** Fill alanı için pixelmap kimliği
- **Stil** Sayısal pixelmap isteminin stili, **Ek D** tüm pencere öğeleri için önceden tanımlanmış genel stilleri ve pencere öğesine özgü stilleri içerir.
- **pixelmap_prompt_id** Uygulama tanımlı istem KIMLIĞI
- **Boyut** Sayısal pixelmap isteminin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) sayısal piksellimap Istemi başarıyla oluşturuldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_numeric_pix_prompt”. */
status = gx_numeric_pixelmap_prompt_create(&my_numeric_pix_prompt,
    “my_numeric_pix_prompt”, &my_parent,
    MY_TEXT_RESOURCE_ID, MY_FEEL_RESOURCE_ID,
    GX_STYLE_BORDER_RAISED, MY_NUMERIC_PIXELMAP_PROMPT_ID,
    &size);

/* If status is GX_SUCCESS the numeric pixelmap prompt “my_numeric_pix_prompt” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_pixelmap_format_function_set
- gx_numeric_pixelmap_prompt_value_set

## <a name="gx_numeric_pixelmap_prompt_format_function_set"></a>gx_numeric_pixelmap_prompt_format_function_set


Sayısal pixelmap isteminin biçim işlevini geçersiz kıl

### <a name="prototype"></a>Prototype

```C
UINT gx_numeric_pixelmap_format_function_set(
    GX_NUMERIC_PIXELMAP_PROMPT *prompt,
    OID (*format_func)(GX_NUMERIC_PIXELMAP_PROMPT *, INT));
```

### <a name="description"></a>Açıklama

Bu hizmet, sayısal piksellimap istem pencere öğesinin varsayılan biçim işlevini geçersiz kılar. Varsayılan biçim işlevi, sayısal pixelmap istem değerini bir dizeye dönüştürür ve pencere öğesinin özel arabelleğinde depolar. Bu hizmet, uygulamanın, sayısal pixelmap istem değerini pencere öğesinin özel arabelleğinde biçimlendirmek ve depolamak için kendi biçim işlevini tanımlamasına olanak sağlar.

### <a name="parameters"></a>Parametreler

- **komut istemi** Sayısal pixelmap istem denetim bloğu
- **format_func** Ayarlanacak biçimlendirme işlevi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) sayısal piksellimap istem biçimi işlevini başarıyla ayarladı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define my numeric pixelmap format function. */
VOID my_format_function(GX_NUMERIC_PIXELMAP_PROMPT *prompt,
    INT value)
{
    /* If the value is “1234”, the new format will be “12.34”. */

    INT length;
    gx_utility_ltoa(value / 100,
        prompt->gx_numeric_pixelmap_prompt_buffer,
        GX_NUMERIC_PROMPT_ BUFFER_SIZE);
    Length = GX_STRLEN(prompt->gx_numeric_pixelmap_prompt_buffer);
    prompt->gx_numeric_pixelmap_prompt_buffer[length++] = ‘.’;
    gx_utility_ltoa(value % 100,
        prompt->gx_numeric_pixelmap_prompt_buffer + length,
        GX_NUMERIC_PROMPT_BUFFER_SIZE - length);
}

/* Override default format function of “my_numeric_pix_prompt”. */
status = gx_numeric_pixelmap_prompt_format_function_set(
    &my_numeric_pix_prompt,
    my_format_function);

/* If status is GX_SUCCESS the format function of “my_numeric_pix_prompt” has been override. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_pixelmap_prompt_create
- gx_numeric_pixelmap_prompt_value_set

## <a name="gx_numeric_pixelmap_prompt_value_set"></a>gx_numeric_pixelmap_prompt_value_set


Sayısal piksellimap istem değerini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_numeric_pixelmap_prompt_value_set(
    GX_NUMERIC_PIXELMAP_PROMPT *prompt,
    INT value);
```

### <a name="description"></a>Açıklama

Bu hizmet, sayısal bir pixelmap istemine bir tamsayı değeri.

### <a name="parameters"></a>Parametreler

- **komut istemi** Sayısal pixelmap istem denetim bloğu
- **değer** Ayarlanacak tamsayı değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) sayısal pixelmap Istem değeri başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set a value to “my_numeric_pix_prompt”. */
status = gx_numeric_pixelmap_prompt_value_set(&my_numeric_pix_prompt, 1000);

/* If status is GX_SUCCESS the value of the numeric pixelmap prompt “my_numeric_pix_prompt” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_pixelmap_prompt_create
- gx_numeric_pixelmap_format_function_set

## <a name="gx_numeric_prompt_create"></a>gx_numeric_prompt_create


Sayısal istem oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_numeric_prompt_create( 
    GX_NUMERIC_PROMPT *prompt,
    GX_CONST GX_CHAR name, GX_WIDGET *parent,
    GX_RESOURCE_ID text_id,
    ULONG style, USHORT prompt_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir sayısal istem pencere öğesi oluşturur. Numeric_ istem yalnızca kendi arabelleğini tutan ve bir gx_numeric_ prompt_value_set (INT) API 'SI sağlayan bir istemdir. arabellek boyutu, varsayılan olarak 16 olan sabit GX_NUMERIC_PROMPT_BUFFER_SIZE tarafından tanımlanır.

GX_NUMERIC_PROMPT GX_PROMPT türetilir ve tüm gx_prompt API hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **komut istemi** Sayısal istem denetim bloğu
- **ad** İstem adı
- **üst öğe** Üst pencere öğesi denetim bloğu
- **text_id** Kaynak dize kimliği
- **Stil** Sayısal istem stili, **Ek D** tüm pencere öğeleri için önceden tanımlanmış genel stilleri ve pencere öğesine özgü stilleri içerir.
- **prompt_id** Uygulama tanımlı istem KIMLIĞI
- **Boyut** Sayısal istem boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) sayısal Istem başarıyla oluşturuldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_numeric _prompt”. */
status = gx_numeric_prompt_create(&my_numeric_prompt,
    “my_numeric_prompt”, &my_parent,
    MY_TEXT_RESOURCE_ID, GX_STYLE_BORDER_RAISED, MY_NUMERIC_PROMPT_ID,
    &size);

/* If status is GX_SUCCESS the numeric prompt “my_numeric_prompt” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_format_function_set
- gx_numeric_prompt_value_set

## <a name="gx_numeric_prompt_format_function_set"></a>gx_numeric_prompt_format_function_set


Sayısal istem için biçim işlevini geçersiz kıl

### <a name="prototype"></a>Prototype

```C
UINT gx_numeric_format_function_set(
    GX_NUMERIC_PROMPT *prompt,
    VOID (*format_func)(GX_NUMERIC_PROMPT *, INT));
```

### <a name="description"></a>Açıklama

Bu hizmet, sayısal istem pencere öğesinin varsayılan biçim işlevini geçersiz kılar. Varsayılan biçim işlevi, sayısal istem değerini bir dizeye dönüştürür ve pencere öğesinin özel arabelleğinde depolar. Bu hizmet, uygulamanın, sayısal istem değerini pencere öğesinin özel arabelleğinde biçimlendirmek ve depolamak için kendi biçim işlevini tanımlamasına olanak sağlar.

### <a name="parameters"></a>Parametreler

- **komut istemi** Sayısal istem denetim bloğu
- **format_func** Ayarlanacak biçimlendirme işlevi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) sayısal istem biçimi işlevini başarıyla ayarladı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define my numeric format function. */
VOID my_format_function(GX_NUMERIC_PROMPT *prompt, INT value)
{
    /* If the value is “1234”, the new format will be “12.34”. */

    INT length;
    gx_utility_ltoa(value / 100, prompt->gx_numeric_prompt_buffer,
        GX_NUMERIC_PROMPT_ BUFFER_SIZE);
    Length = GX_STRLEN(prompt->gx_numeric_prompt_buffer);
    prompt->gx_numeric_prompt_buffer[length++] = ‘.’;
    gx_utility_ltoa(value % 100,
        prompt->gx_numeric_prompt_buffer + length,
        GX_NUMERIC_PROMPT_BUFFER_SIZE - length);
}

/* Override the default format function of “my_numeric_prompt”. */
status = gx_numeric_prompt_format_function_set(&my_numeric_prompt,
    my_format_function);

/* If status is GX_SUCCESS, the format function of “my_numeric_prompt” has been override. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_prompt_create
- gx_numeric_prompt_value_set

## <a name="gx_numeric_prompt_value_set"></a>gx_numeric_prompt_value_set


Sayısal istem değeri ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_numeric_prompt_value_set(
    GX_NUMERIC_PROMPT *prompt, 
    INT value);
```

### <a name="description"></a>Açıklama

Bu hizmet bir sayısal istem için bir tamsayı değeri ayarlar.

### <a name="parameters"></a>Parametreler

- **komut istemi** Sayısal istem denetim bloğu
- **değer** Ayarlanacak tamsayı değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) sayısal Istem değeri başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set a value to “my_numeric_prompt”. */
status = gx_numeric_prompt_value_set(&my_numeric_prompt, 1000);

/* If status is GX_SUCCESS the value of the numeric prompt “my_numeric_prompt” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_prompt_create
- gx_numeric_format_function_set

## <a name="gx_numeric_scroll_wheel_create"></a>gx_numeric_scroll_wheel_create


Sayısal kaydırma tekerleği oluştur

### <a name="prototype"></a>Prototype


UINT gx_numeric_scroll_wheel_create (GX_NUMERIC_SCROLL_WHEEL * tekerlek, GX_CONST GX_CHAR * ad, GX_WIDGET * üst, INT start_val, INT end_val, ULONG stili, USHORT wheel_id, GX_CONST GX_RECTANGLE * size);

### <a name="description"></a>Açıklama

Bu hizmet sayısal bir kaydırma tekerleği pencere öğesi oluşturur.

Sayısal bir kaydırma tekerleği, bir dizi sayıyı görüntülemek için özel olarak kullanılan bir kaydırma tekerleği pencere öğesi türüdür. Diğer kaydırma tekerleği pencere öğesi türleri de mevcuttur. Kaydırma tekerleği pencere öğesi hiyerarşisi, pencere öğesi türleri ve pencere öğesi türetme hakkında daha fazla bilgi için gx_scroll_wheel_create () API 'sine bakın.

GX_NUMERIC_SCROLL_WHEEL GX_TEXT_SCROLL_WHEEL türetilir ve tüm gx_text_scroll_wheel ve gx_scroll_wheel hizmetlerini destekler.

Kaydırma tekerleği kaydırıldığında, tüm kaydırma tekerleği türleri üst öğesine GX_EVENT_LIST_SELECT olaylar oluşturur.

Sayısal bir kaydırma tekerleği varsayılan olarak ABS (end_val – start_val) + 1 satıra sahip olur. Diğer bir deyişle, kaydırma tekerleği start_val ve end_val arasındaki her değeri görüntüler, her satır ile 1 ' i artırmaz veya azaltılır. Uygulamanın aralığın görünmesini istediği yönteme bağlı olarak, start_val end_val daha fazla veya daha az olabileceğini unutmayın.

Uygulama satır artışını değiştirmek isterse, sayısal kaydırma tekerleğini oluşturduktan sonra gx_scroll_wheel_total_rows_set () çağırarak bunu yapabilir. Örneğin bir uygulama, 1980 ile 2020 arasındaki yılları görüntüleyen bir kaydırma tekerleği oluşturmak isteyen bir uygulamadır.

```C
gx_numeric_scroll_wheel_create(&wheel, GX_NULL, parent, 1980,
    2020, style, id, &size);

/* the years 1980 through 2020, inclusive, incrementing by 5 years,
yields 9 total rows */

gx_scroll_wheel_total_rows_set(&wheel, 9);
```

### <a name="parameters"></a>Parametreler

- **tekerlek** Sayısal kaydırma tekerleği denetim bloğu işaretçisi
- **ad** Pixelmap düğme pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **start_val** Başlangıç sayısal değeri
- **end_val** Bitiş sayısal değeri
- **Stil** Onay kutusunun stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **wheel_id** Uygulama tanımlı kaydırma tekerleği KIMLIĞI
- **Boyut** Kaydırma tekerleği pencere öğesinin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) sayısal kaydırma tekerleği başarıyla oluşturuldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “year_wheel”. */
status = gx_numeric_scroll_wheel_create(&year_wheel,
    “year_selector””, &parent,
    1980, 2040,
    GX_STYLE_ENABLED | GX_STYLE_TEXT_CENTER |
    GX_STYLE_TRANSPARENT | GX_STYLE_WRAP |
    GX_STYLE_TEXT_SCROLL_WHEEL_ROUND,
    YEAR_WHEEL_ID,
    &size);

/* If status is GX_SUCCESS the scroll wheel “year_wheel” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_text_get

## <a name="gx_numeric_scroll_wheel_range_set"></a>gx_numeric_scroll_wheel_range_set


Sayısal kaydırma tekerleğinin değer aralığını ata

### <a name="prototype"></a>Prototype

```C
UINT
gx_numeric_scroll_wheel_range_set(
    GX_NUMERIC_SCROLL_WHEEL *wheel,
    INT start_val, INT end_val);
```

### <a name="description"></a>Açıklama

Bu hizmet, izin verilen ve sayısal bir kaydırma tekerleği pencere öğesi tarafından görünen değer aralığını değiştirir.

Sayısal bir kaydırma tekerleği, bir dizi sayıyı görüntülemek için özel olarak kullanılan bir kaydırma tekerleği pencere öğesi türüdür. Diğer kaydırma tekerleği pencere öğesi türleri de mevcuttur. Kaydırma tekerleği pencere öğesi hiyerarşisi, pencere öğesi türleri ve pencere öğesi türetme hakkında daha fazla bilgi için gx_scroll_wheel_create () API 'sine bakın.

Bu API 'YI çağırmak, kaydırma tekerleği toplam satırlarını ABS (end_val – start_val) + 1 olarak sıfırlar, yani kaydırma tekerleği her satır için 1 ile artacaktır. Bunu değiştirmek için, uygulama toplam satır sayısını değiştirmek için gx_scroll_wheel_total_rows_set () çağırabilir ve satırlar arasındaki değer artışını etkin bir şekilde değiştirir.

### <a name="parameters"></a>Parametreler

- **tekerlek** Sayısal kaydırma tekerleği denetim bloğu işaretçisi
- **start_val** Başlangıç sayısal değeri 
- **end_val** Bitiş sayısal değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) sayısal kaydırma tekerleği aralığı başarıyla ayarlandı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları 

### <a name="example"></a>Örnek

```C
/* Change range of “rate” scroll wheel. */

status = gx_numeric_scroll_wheel_range_set(&year_wheel, 0, 200);

/* If status is GX_SUCCESS the scroll wheel range has been modified. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_pixelmap_button_create"></a>gx_pixelmap_button_create


Pixelmap oluştur düğmesi

### <a name="prototype"></a>Prototype

```C
UINT gx_pixelmap_button_create(
    GX_PIXELMAP_BUTTON *button,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_RESOURCE_ID normal_id,
    GX_RESOURCE_ID selected_id,
    GX_RESOURCE_ID disabled_id,
    ULONG style,
    USHORT pixelmap_button_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pixelmap düğme pencere öğesi oluşturur.

GX_PIXELMAP_BUTTON GX_BUTTON türetilir ve tüm gx_button hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **düğme** Pixelmap Button denetim bloğu işaretçisi
- **ad** Pixelmap düğme pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **normal_id** Normal durum kaynak KIMLIĞI
- **selected_id** Seçili durum kaynak KIMLIĞI
- **disabled_id** Devre dışı durum kaynak KIMLIĞI
- **Stil** Onay kutusunun stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **pixelmap_button_id** Uygulama tanımlı pixelmap düğmesinin KIMLIĞI
- **Boyut** Pixelmap düğmesinin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bir şekilde pixelmap düğmesi oluşturuldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_pixelmap_button”. */
status = gx_pixelmap_button_create(&my_pixelmap_button,
    “my_pixelmap_button”, &my_parent,
    MY_NORMAL_RESOURCE_ID, MY_SELECTED_RESOURCE_ID,
    MY_DESELECTED_RESOURCE_ID, GX_STYLE_BORDER_RAISED,
    MY_PIXELMAP_BUTTON_ID,
    &size);

/* If status is GX_SUCCESS the pixelmap button “my_pixelmap_button” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_pixelmap_button_draw
- gx_pixelmap_button_pxielmap_set
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_radio_button_create
- gx_radio_button_draw
- gx_icon_button_create
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_pixelmap_button_draw"></a>gx_pixelmap_button_draw


Pixelmap çiz düğmesi

### <a name="prototype"></a>Prototype

```C
VOID gx_pixelmap_button_draw(GX_PIXELMAP_BUTTON *button);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pixelmap düğme pencere öğesi çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel pixelmap düğme pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **düğme** Pixelmap Button denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom pixelmap button drawing function. */

VOID my_pixelmap_button_draw(GX_PIXELMAP_BUTTON *button)
{
    /* Call default pixelmap button draw. */
    gx_pixelmap_button_draw(button);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_pixelmap_button_create
- gx_pixelmap_button_pxielmap_set
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_radio_button_create
- gx_radio_button_draw
- gx_icon_button_create
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_pixelmap_button_event_process"></a>gx_pixelmap_button_event_process


Pixelmap düğmesi olay işleme

### <a name="prototype"></a>Prototype

```C
UINT gx_pixelmap_button_event_process(
    GX_PIXELMAP_BUTTON *button,
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, pixelmap düğmesi pencere öğesi türü için varsayılan olay işleme sağlar.

### <a name="parameters"></a>Parametreler

- **düğme** Pixelmap Button denetim bloğu işaretçisi
- **event_ptr** GX_EVENT yapısına yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pixelmap düğmesi çiz
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
switch(event_ptr->gx_event_type)
{
    case GX_EVENT_SHOW:
        /* Do default handling. */
        status = gx_pixelmap_button_event_process(icon, event_ptr);
    
        /* add my own handling here */
        break;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_pixelmap_button_create
- gx_pixelmap_button_pxielmap_set
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_radio_button_create
- gx_radio_button_draw
- gx_icon_button_create
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_pixelmap_button_pixelmap_set"></a>gx_pixelmap_button_pixelmap_set


Düğmeye pixelmaps ata

### <a name="prototype"></a>Prototype

```C
UINT gx_pixelmap_button_pixelmap_set(
    GX_PIXELMAP_BUTTON *button, 
    GX_RESOURCE_ID normal_id,
    GX_RESOURCE_ID selected_id, 
    GX_RESOURCE_ID disabled_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, pixelmaps 'i pixelmap düğmesine ayarlar.

### <a name="parameters"></a>Parametreler

- **düğme** Pixelmap Button denetim bloğu işaretçisi
- **normal_id** Normal durum olarak kullanılacak pixelmap 'in kaynak KIMLIĞI
- **selected_id** Düğme seçildiğinde kullanılacak pixelmap 'in kaynak KIMLIĞI
- **disabled_id** Düğme devre dışı bırakıldığında kullanılacak pixelmap 'in kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı, düğmeye pixelmap 'i ayarlar
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw “my_pixelmap_button”. */
status = gx_pixelmap_button_pixelmap_set (&my_pixelmap_button,
    NORMAL_ID, SELECTED_ID,
    DISABLED_ID);

/* If status is GX_SUCCESS the pixelmap button is properly configured with the specified pixelmaps. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_radio_button_create
- gx_radio_button_draw
- gx_icon_button_create
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_pixelmap_prompt_create"></a>gx_pixelmap_prompt_create


Pixelmap istemi oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_pixelmap_prompt_create(
    GX_PIXELMAP_PROMPT *prompt,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_RESOURCE_ID text_id,
    GX_RESOURCE_ID fill_pixelmap_id,
    ULONG style,
    USHORT pixelmap_prompt_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pixelmap istem pencere öğesi oluşturur. Bir pixelmap istemi, bir standart GX_PROMPT farklılık gösterir ve bu, pixelmaps kullanarak istemin arka planını boyar. Oluşturma işlevi bir pixelmap kimliği kabul eder, normal durum dolgusu pixelmap. En fazla altı pixelmaps, pixelmap istemine atanabilir.

### <a name="parameters"></a>Parametreler

- **komut istemi** Pixelmap istem denetim bloğu işaretçisi
- **ad** Pixelmap istem pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **text_id** Metnin kaynak KIMLIĞI
- **fill_id** Dolgunun kaynak KIMLIĞI
- **Stil** Onay kutusunun stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **pixelmap_prompt_id** Pixelmap isteminin uygulama tanımlı KIMLIĞI
- **Boyut** Pixelmap isteminin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bir pixelmap istemi oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_pixelmap_prompt”. */
status = gx_pixelmap_prompt_create(&my_pixelmap_prompt,
    “my_pixelmap_prompt”, &my_parent,
    MY_TEXT_RESOURCE_ID, MY_LEFT_RESOURCE_ID,
    MY_FILL_RESOURCE_ID, MY_RIGHT_RESOURCE_ID,
    GX_STYLE_BORDER_RAISED, MY_PIXELMAP_PROMPT_ID,
    &size);

/* If status is GX_SUCCESS the pixelmap prompt “my_pixelmap_prompt” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_pixelmap_button_pixelmap_set
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_get
- gx_prompt_text_set

## <a name="gx_pixelmap_prompt_draw"></a>gx_pixelmap_prompt_draw


Pixelmap istemi çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_pixelmap_prompt_draw(GX_PIXELMAP_PROMPT *prompt);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pixelmap istem pencere öğesi çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel pixelmap istem pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **komut istemi** Pixelmap istem denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom pixelmap prompt drawing function. */

VOID my_pixelmap_button_draw(GX_PIXELMAP_PROMPT *prompt)
{
    /* Call default pixelmap prompt draw. */
    gx_pixelmap_prompt_draw(prompt);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_pixelmap_button_pixelmap_set
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_get
- gx_prompt_text_set

## <a name="gx_pixelmap_prompt_pixelmap_set"></a>gx_pixelmap_prompt_pixelmap_set


İsteyecek pixelmaps ata

### <a name="prototype"></a>Prototype

```C
UINT gx_pixelmap_prompt_pixelmap_set(
    GX_PIXELMAP_PROMPT *prompt,
    GX_RESOURCE_ID normal_left_pixelmap,
    GX_RESOURCE_ID normal_fill_pixelmap,
    GX_RESOURCE_ID normal_right_pixelmap,
    GX_RESOURCE_ID selected_left_pixelmap,
    GX_RESOURCE_ID selected_fill_pixelmap,
    GX_RESOURCE_ID selected_right_pixelmap);
```

### <a name="description"></a>Açıklama

Bu hizmet, pixelmap kodlarını pixelmap istemine atar. Sol, Fill ve Right pixelmap kimlikleri, uygulamanın çeşitli genişlikler için bir dizi pixelmaps kullanmasına izin vermek için kullanılır, ancak depolama gereksinimlerine kaydetmek için ortak bir yükseklik. Sol ve sağ kimlikler kullanılmıyorsa, bunlar 0 olarak ayarlanmalıdır. İstem, giriş odağını kazandığında kendisini farklı çizirse, bu amaçla seçili pixelmap kimlikleri kullanılır. Seçilen kimlikler kullanılmıyorsa veya normal kimlikler ile aynıysa, bunları 0 olarak ayarlayın.

### <a name="parameters"></a>Parametreler

- **komut istemi** Pixelmap istem denetim bloğu işaretçisi
- **normal_left_id** Normal durumun sol tarafında kullanılacak olan pixelmap 'in kaynak KIMLIĞI
- **normal_fill_id** Normal durumda döşeli bir dolgusu olarak kullanılacak pixelmap 'in kaynak KIMLIĞI
- **normal_right_id** Sağ tarafta normal durumda kullanılacak olan pixelmap 'in kaynak KIMLIĞI
- **selected_left_id** Seçili durumda sol tarafta kullanılacak olan pixelmap 'in kaynak KIMLIĞI
- **selected_fill_id** Seçili durumda döşeli bir dolgusu olarak kullanılacak pixelmap 'in kaynak KIMLIĞI
- **selected_right_id** Seçili durumda sağ tarafta kullanılacak olan pixelmap 'in kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı, komut istemine pixelmap 'i ayarlar
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_RESOURCE_ID** (0x33) kaynak kimliği geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Assign pixelmap IDs to “my_prompt”. Only the normal state pixelmaps are used in this case */
status = gx_pixelmap_prompt_pixelmap_set (&my_prompt,
    normal_left_id, normal_fill_id,
    normal_right_id, 0, 0, 0);

/* If status is GX_SUCCESS the pixelmap prompt is properly configured with pixelmaps. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_pixelmap_button_pixelmap_set
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_radio_button_create
- gx_radio_button_draw
- gx_icon_button_create
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_pixelmap_slider_create"></a>gx_pixelmap_slider_create


Pixelmap kaydırıcı oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_pixelmap_slider_create(
    GX_PIXELMAP_SLIDER *slider,
    GX_CONST GX_CHAR *name, GX_WIDGET *parent,
    GX_SLIDER_INFO *info,
    GX_PIXELMAP_SLIDER_INFO *pixelmap_info, ULONG style,
    USHORT pixelmap_slider_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pixelmap kaydırıcı pencere öğesi oluşturur.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Pixelmap kaydırıcı denetim bloğu işaretçisi
- **ad** Pixelmap kaydırıcı pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **bilgi** Kaydırıcı minimum değeri, en büyük değer, geçerli değer ve iğne limitlerini tanımlayan değerleri içeren GX_SLIDER_INFO yapısına yönelik işaretçi. **Ek ı** GX_SLIDER_INFO yapısı için tanım içeriyor.
- **pixelmap_info** Kaydırıcı arka planını ve iğne çizmek için kullanılan pixelmaps 'i tanımlayan GX_PIXELMAP_SLIDER_INFO yapısına yönelik işaretçi. **Ek ı** GX_PIXELMAP_SLIDER_INFO yapısı için tanım içeriyor. Kaydırıcı arka planı bir veya iki pixelmaps kullanabilir. Bir tane varsa, iğne taşırken arka plan değişmez. İki arka plan tanımlanmışsa, iğne ilk arka plan pixelmap 'i kullanmadan önce arka plan ve iğne ikinci arka plan pixelmap 'i kullandıktan sonra arka plan kullanılır.
- **Stil** Kaydırıcı stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **pixelmap_slider_id** Pixelmap kaydırıcısının uygulama tanımlı KIMLIĞI
- **Boyut** Pixelmap isteminin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00), pixelmap kaydırıcısını başarıyla oluşturdu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_SLIDER_INFO info;
GX_PIXELMAP_SLIDER_INFO pixelmap_info;

/* Initiate slider information structure. */
info.gx_slider_info_min_val = 0;
info.gx_slider_info_max_val = 100;
info.gx_slider_info_current_val = 50;
info.gx_slider_info_min_travel = 10;
info.gx_slider_info_max_tralvel = 10;
info.gx_slider_info_needle_width = 5;
info.gx_slider_info_needle_height = 10;
info.gx_slider_info_needle_inset = 5;
info.gx_slider_info_needle_hotspot_offset;

/* Initiate pixelmap slider information structure. */
pixelmap_info.gx_pixelmap_slider_info_lower_background_pixelmap =
                                        GX_PIXELMAP_ID_ORANGE;
pixelmap_info.gx_pixelmap_slider_info_upper_background_pixelmap =
                                        GX_PIXELMAP_ID_EMPTY;
pixelmap_info.gx_pixelmap_slider_info_needle_pixelmap =
                                        GX_PIXELMAP_ID_NEEDLE;

/* Create “my_pixelmap_slider”. */
status = gx_pixelmap_slider_create(&my_pixelmap_slider,
                            “my_pixelmap_slider”, &my_parent,
                            &info, &pixelmap_info,
                            GX_STYLE_BORDER_RAISED,
                            MY_PIXELMAP_SLIDER_ID, &size);

/* If status is GX_SUCCESS the pixelmap slider “my_pixelmap_slider” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_pixelmap_button_pixelmap_set
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_slider_create
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_pixelmap_slider_draw"></a>gx_pixelmap_slider_draw


Pixelmap kaydırıcısını çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_pixelmap_slider_draw(GX_PIXELMAP_SLIDER *slider);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pixelmap kaydırıcı pencere öğesi çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel pixelmap kaydırıcı pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Pixelmap kaydırıcı denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom pixelmap slider drawing function. */

VOID my_pixelmap_slider_draw(GX_PIXELMAP_SLIDER *pixelmap_slider)
{
    /* Call default pixelmap slider draw. */
    gx_pixelmap_slider_draw(pixelmap_slider);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_pixelmap_button_pixelmap_set
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_create
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_pixelmap_slider_event_process"></a>gx_pixelmap_slider_event_process


İşlem pixelmap kaydırıcı olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_pixelmap_slider_event_process(
    GX_PIXELMAP_SLIDER *slider,
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pixelmap kaydırıcı pencere öğesi için bir olayı işler.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Pixelmap işaretçisi
- **kaydırıcı** denetimi olay işaretçisini işlenecek olaya engel

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pixelmap kaydırıcı olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom event processing function. */
UINT my_event_hanlder(GX_PIXELMAP_SLIDER *pixelmap_slider, GX_EVENT *event_ptr)
{
    switch(event_ptr->gx_event_type)
    {
    case GX_EVENT_SHOW:
        /* Do default handling. */
        status = gx_pixelmap_slider_event_process(pixelmap_slider,
                                                    event_ptr);

        /* add my own handling here */
        break;
    default:
        status = gx_pixelmap_slider_event_process(pixelmap_slider,
                                                  event_ptr);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_pixelmap_button_pixelmap_set
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_pixelmap_slider_pixelmap_set"></a>gx_pixelmap_slider_pixelmap_set


Kaydırıcıya pixelmaps ata

### <a name="prototype"></a>Prototype

```C
UINT gx_pixelmap_slider_pixelmap_set(
    GX_PIXELMAP_SLIDER *slider,
    GX_PIXELMAP_SLIDER_INFO *pixinfo);
```

### <a name="description"></a>Açıklama

Bu hizmet, pixelmaps 'i pixelmap kaydırıcıyla ayarlar.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Pixelmap kaydırıcı denetim bloğu işaretçisi
- **pikselınfo** Kaydırıcı arka planını ve iğne çizmek için kullanılan pixelmaps 'i tanımlayan GX_PIXELMAP_SLIDER_INFO yapısına yönelik işaretçi. **Ek ı** GX_PIXELMAP_SLIDER_INFO yapısı için tanım içeriyor. Kaydırıcı arka planı bir veya iki pixelmaps kullanabilir. Bir tane varsa, iğne taşırken arka plan değişmez. İki arka plan tanımlanmışsa, iğne ilk arka plan pixelmap 'i kullanmadan önce arka plan ve iğne ikinci arka plan pixelmap 'i kullandıktan sonra arka plan kullanılır.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı, kaydırıcı ile pixelmap 'i ayarlar
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_PIXELMAP_SLIDER_INFO pixelmap_info;

/* Initiate pixelmap slider information structure. */
pixelmap_info.gx_pixelmap_slider_info_lower_background_pixelmap =
                                        GX_PIXELMAP_ID_ORANGE;
pixelmap_info.gx_pixelmap_slider_info_upper_background_pixelmap =
                                        GX_PIXELMAP_ID_EMPTY;
pixelmap_info.gx_pixelmap_slider_info_needle_pixelmap =
                                        GX_PIXELMAP_ID_NEEDLE;

/* Draw “my_pixelmap_button”. */
status = gx_pixelmap_slider _pixelmap_set (&my_pixelmap_slider,
                                &pixelmap_info);

/* If status is GX_SUCCESS the pixelmap slider is properly configured with “pixelmap_info”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_radio_button_create
- gx_radio_button_draw
- gx_icon_button_create
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw

## <a name="gx_progress_bar_background_draw"></a>gx_progress_bar_background_draw


Çizim ilerleme çubuğu arka planı

### <a name="prototype"></a>Prototype

```C
VOID gx_progress_bar_background_draw(GX_PROGRESS_BAR *progress_bar)
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen ilerleme çubuğunun arka planını çizer. Bu işlev, gx_progress_bar_draw () bir parçası olarak dahili olarak çağrılır, ancak uygulamanın özel bir ilerleme çubuğu çizim işlevini tanımladığı bu durumları desteklemek için uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **ilerleme çubuğu** İlerleme çubuğu denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom progress bar drawing function. */

VOID my_progress_bar_draw(GX_PROGRESS_BAR *progress_bar)
{
    /* Call default progress bar background draw. */
    gx_progress_bar_background_draw(progress_bar);

    /* Call default progress bar text draw. */
    gx_progress_bar_text_draw(progress_bar);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_create
- gx_progress_bar_draw
- gx_progress_bar_event_process
- gx_progress_bar_font_set
- gx_progress_bar_info_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_range_set
- gx_progress_bar_text_color_set
- gx_progress_bar_value_set

## <a name="gx_progress_bar_create"></a>gx_progress_bar_create


İlerleme çubuğu oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_progress_bar_create(
    GX_PROGRESS_BAR *progress_bar,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_PROGRESS_BAR_INFO *progress_bar_info,
    ULONG style, 
    USHORT progress_bar_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir ilerleme çubuğu pencere öğesi oluşturur.

### <a name="parameters"></a>Parametreler

- **progress_bar** İlerleme çubuğu denetim bloğu
- **ad** Mantıksal ad
- **üst öğe** Üst pencere öğesi işaretçisi
- **progress_bar_info** GX_PROGRESS_BAR_INFO yapısına yönelik işaretçi. **Ek ı** GX_PROGRESS_BAR_INFO yapısı için tanım içeriyor.
- **Stil** İlerleme çubuğu stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **progress_bar_id** Uygulama tanımlı ilerleme çubuğu KIMLIĞI
- **Boyut** İlerleme çubuğunun boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ilerleme çubuğu oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET** (0x12) üst pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_PROGRESS_BAR_INFO info;
GX_RECTANGLE size;

info.gx_progress_bar_info_min_val = 0;
info.gx_progress_bar_info_max_val = 100;
info.gx_progress_bar_info_current_val = 0;
info.gx_progress_bar_font_id = GX_FONT_ID_SYSTEM_FONT;
info.gx_progress_bar_normal_text_color = GX_COLOR_ID_WHITE;
info.gx_progress_bar_selected_text_color = GX_COLOR_ID_BLUE;
info.gx_progress_bar_fill_pixelmap = 0;

size.gx_rectangle_left = 10;
size.gx_rectangle_top = 10;
size.gx_rectangle_right = 110;
size.gx_rectangle_bottom = 140;

/* Create a progress bar with the specified information. */
status = gx_progress_bar_create(&my_progress_bar, GX_NULL, GX_NULL,
                        &info, GX_STYLE_BORDER_THIN,
                        0, &size);

/* If status is GX_SUCSESS the progress bar “my_progress_bar” has been successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_draw
- gx_progress_bar_event_process
- gx_progress_bar_font_set
- gx_progress_bar_info_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_range_set
- gx_progress_bar_text_color_set
- gx_progress_bar_text_draw
- gx_progress_bar_value_set

## <a name="gx_progress_bar_draw"></a>gx_progress_bar_draw


İlerleme çubuğu çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_progress_bar_draw(GX_PROGRESS_BAR *progress_bar);
```

### <a name="description"></a>Açıklama

Bu hizmet bir ilerleme çubuğu pencere öğesi çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel ilerleme çubuğu pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **progress_bar** İlerleme çubuğu denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom progress bar drawing function. */

VOID my_progress_bar_draw(GX_PROGRESS_BAR *progress_bar)
{
    /* Call default progress bar draw. */
    gx_progress_bar_draw(progress_bar);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_create
- gx_progress_bar_event_process
- gx_progress_bar_font_set
- gx_progress_bar_info_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_range_set
- gx_progress_bar_text_color_set
- gx_progress_bar_text_draw
- gx_progress_bar_value_set

## <a name="gx_progress_bar_event_process"></a>gx_progress_bar_event_process


İlerleme durumu çubuğu olayını ilerleme

### <a name="prototype"></a>Prototype

```C
UINT gx_progress_bar_event_process(
    GX_PROGRESS_BAR *progress_bar,
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet bir ilerleme çubuğu olayını işler.

### <a name="parameters"></a>Parametreler

- **progress_bar** İlerleme çubuğu denetim bloğu
- **event_ptr** GX_EVENT yapısına yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı istem oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom event processing function. */

UINT my_event_process (GX_PROGRESS_BAR *progress_bar, GX_EVENT *event_ptr)
{
    switch(event_ptr->gx_event_type)
    {
    case GX_EVENT_SHOW:
        /* Do default handling. */
        status = gx_progress_bar_event_process(progress_bar,
                                                event_ptr);
        /* add my own handling here */
        break;
    default:
        status = gx_progress_bar_event_process(progress_bar,
                                                event_ptr);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_create
- gx_progress_bar_event_draw
- gx_progress_bar_font_set
- gx_progress_bar_info_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_range_set
- gx_progress_bar_text_color_set
- gx_progress_bar_text_draw
- gx_progress_bar_value_set

## <a name="gx_progress_bar_font_set"></a>gx_progress_bar_font_set


İlerleme çubuğu metninin yazı tipini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_progress_bar_font_set(
    GX_PROGRESS_BAR *progress_bar,
    GX_RESOURCE_ID font_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir ilerleme çubuğu pencere öğesinin yazı tipini ayarlar.

### <a name="parameters"></a>Parametreler

- **progress_bar** İlerleme çubuğu denetim bloğu
- **font_id** Yazı tipi kaynak kimliği

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ilerleme çubuğu yazı tipi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT status = gx_progress_bar_font_set(&progress_bar,
                                        GX_FONT_ID_MEDIUM);

/* if status is GX_SUCCESS, the font was successfully assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_create
- gx_progress_bar_draw
- gx_progress_bar_event_process
- gx_progress_bar_info_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_range_set
- gx_progress_bar_text_color_set
- gx_progress_bar_text_draw
- gx_progress_bar_value_set

## <a name="gx_progress_bar_info_set"></a>gx_progress_bar_info_set


İlerleme çubuğu bilgi yapısını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_progress_bar_info_set(
    GX_PROGRESS_BAR *progress_bar,
    GX_PROGRESS_BAR_INFO *info);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir ilerleme çubuğu pencere öğesinin bilgi yapısını sıfırlar.

### <a name="parameters"></a>Parametreler

- **progress_bar** İlerleme çubuğu denetim bloğu
- **bilgi** GX_PROGRESS_BAR_INFO yapısına yönelik işaretçi. **Ek ı** GX_PROGRESS_BAR_INFO yapısı için tanım içeriyor.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) ilerleme çubuğu bilgilerini başarıyla sıfırladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_PROGRESS_BAR_INFO info;

info.gx_progress_bar_info_min_val = 0;
info.gx_progress_bar_info_max_val = 100;
info.gx_progress_bar_info_current_val = 0;
info.gx_progress_bar_font_id = GX_FONT_ID_SYSTEM_FONT;
info.gx_progress_bar_normal_text_color = GX_COLOR_ID_WHITE;
info.gx_progress_bar_selected_text_color = GX_COLOR_ID_BLUE;
info.gx_progress_bar_fill_pixelmap = 0;

status = gx_progress_bar_info_set(&progress_bar, &info);

/* if status == GX_SUCCESS the progress bar info was re-assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_info_create
- gx_progress_bar_draw
- gx_progress_bar_event_process
- gx_progress_bar_font_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_range_set
- gx_progress_bar_text_color_set
- gx_progress_bar_text_draw
- gx_progress_bar_value_set

## <a name="gx_progress_bar_pixelmap_set"></a>gx_progress_bar_pixelmap_set


İlerleme çubuğu çizmek için kullanılan pixelmap 'i ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_progress_bar_pixelmap_set(
    GX_PROGRESS_BAR *progress_bar,
    GX_RESOURCE_ID pixelmap_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, ilerleme çubuğu arka planını dolduracak şekilde kullanılan pixelmap 'i ayarlar.

### <a name="parameters"></a>Parametreler

- **progress_bar** İlerleme çubuğu denetim bloğu
- **pixelmap_id** Pixelmap kaynak kimliği

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ilerleme çubuğu pixelmap kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT status = gx_progress_bar_pixelmap_set(&progress_bar,
                                GX_PIXELMAP_ID_PROGRESS_FILL);

/* if status is GX_SUCCESS, the pixelmap was successfully assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_pielmap_create
- gx_progress_bar_draw
- gx_progress_bar_event_process
- gx_progress_bar_font_set
- gx_progress_bar_info_set
- gx_progress_bar_range_set
- gx_progress_bar_text_color_set
- gx_progress_bar_text_draw
- gx_progress_bar_value_set

## <a name="gx_progress_bar_range_set"></a>gx_progress_bar_range_set


İlerleme çubuğunun değer aralığını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_progress_bar_range_set(
    GX_PROGRESS_BAR *progress_bar,
    INT min_value, 
    INT max_value);
```

### <a name="description"></a>Açıklama

Bu hizmet, ilerleme çubuğu değer aralığını ayarlar.

### <a name="parameters"></a>Parametreler

- **progress_bar** İlerleme çubuğu denetim bloğu
- **min_value** İlerleme çubuğu minimum değeri
- **MAX_VALUE** İlerleme çubuğu maksimum değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ilerleme çubuğu aralığı kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT status = gx_progress_bar_range_set(progress_bar, 0, 100);

/* if status is GX_SUCCESS, the progress bar range was successfully assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_range_create
- gx_progress_bar_draw
- gx_progress_bar_event_process
- gx_progress_bar_font_set
- gx_progress_bar_info_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_text_color_set
- gx_progress_bar_text_draw
- gx_progress_bar_value_set

## <a name="gx_progress_bar_text_color_set"></a>gx_progress_bar_text_color_set


İlerleme çubuğunun metin rengini ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_progress_bar_text_color_set(
    GX_PROGRESS_BAR *progress_bar,
    GX_RESOURCE_ID normal_text_color,
    GX_RESOURCE_ID selected_text_color,
    GX_RESOURCE_ID disabled_text_color);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir ilerleme çubuğu pencere öğesinin metin rengini ayarlar.

### <a name="parameters"></a>Parametreler

- **progress_bar** İlerleme çubuğu denetim bloğu
- **normal_text_color** Normal durumda kullanılan normal metin renginin kaynak KIMLIĞI
- **selected_text_color** Pencere öğesi odaklanıldığında kullanılan seçili metin renginin kaynak KIMLIĞI
- **disabled_text_color** GX_STYLE_ENABLED etkin olmadığında kullanılan devre dışı metin renginin kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ilerleme çubuğu metin rengi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set text colors for the progress bar “my_progress_bar”*/
UINT status = gx_progress_bar_text_color_set(&my_progress_bar,
                        GX_COLOR_ID_NORMAL_TEXT,
                        GX_COLOR_ID_SELECTED_TEXT,
                        GX_COLOR_ID_DISABLED_TEXT);

/* if status is GX_SUCCESS, the progress bar text colors were successfully assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_create
- gx_progress_bar_draw
- gx_progress_bar_event_process
- gx_progress_bar_font_set
- gx_progress_bar_info_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_range_set
- gx_progress_bar_text_draw
- gx_progress_bar_value_set

## <a name="gx_progress_bar_text_draw"></a>gx_progress_bar_text_draw


Çizim ilerleme çubuğu metni

### <a name="prototype"></a>Prototype

```C
VOID gx_progress_bar_text_draw(GX_PROGRESS_BAR *progress_bar)
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen ilerleme çubuğunun metnini çizer. Bu işlev, gx_progress_bar_draw () bir parçası olarak dahili olarak çağrılır, ancak uygulamanın özel bir ilerleme çubuğu çizim işlevini tanımladığı bu durumları desteklemek için uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **ilerleme çubuğu** İlerleme çubuğu denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom progress bar drawing function. */

VOID my_progress_bar_draw(GX_PROGRESS_BAR *progress_bar)
{
    /* Call default progress bar background draw. */
    gx_progress_bar_background_draw(progress_bar);

    /* Call default progress bar text draw. */
    gx_progress_bar_text_draw(progress_bar);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_create
- gx_progress_bar_draw
- gx_progress_bar_event_process
- gx_progress_bar_font_set
- gx_progress_bar_info_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_range_set
- gx_progress_bar_text_color_set
- gx_progress_bar_value_set

## <a name="gx_progress_bar_value_set"></a>gx_progress_bar_value_set


İlerleme çubuğunun geçerli değerini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_progress_bar_value_set(
    GX_PROGRESS_BAR *progress_bar,
    INT value);
```

### <a name="description"></a>Açıklama

Bu hizmet, ilerleme çubuğu geçerli değerini atar. İlerleme çubuğu değeri değiştirildiğinde ilerleme çubuğu pencere öğesi otomatik olarak geçersiz kılacak ve yeniden çizilecektir.

### <a name="parameters"></a>Parametreler

- **progress_bar** İlerleme çubuğu denetim bloğu
- **değer** İlerleme çubuğu geçerli değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarıyla ilerleme çubuğunun değerini ayarla
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT status = gx_progress_bar_value_set(progress_bar, 50);

/* if status == GX_SUCCESS the progress bar value was successfully assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_progress_bar_value_create
- gx_progress_bar_draw
- gx_progress_bar_event_process
- gx_progress_bar_font_set
- gx_progress_bar_info_set
- gx_progress_bar_pielmap_set
- gx_progress_bar_range_set
- gx_progress_bar_text_color_set
- gx_progress_bar_text_draw

## <a name="gx_prompt_create"></a>gx_prompt_create


İstem oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_prompt_create(
    GX_PROMPT *prompt, 
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent, 
    GX_RESOURCE_ID text_id,
    ULONG style, 
    USHORT prompt_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir istem pencere öğesi oluşturur.

GX_PROMPT GX_WIDGET türetilir ve tüm gx_widget hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- Üst pencere öğesi **işaretçisi**
- **text_id** İstem metninin kaynak KIMLIĞI
- **Stil** İstem stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **prompt_id** Uygulama tanımlı istem KIMLIĞI
- **Boyut** İstem boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı istem oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_prompt”. */
status = gx_prompt_create(&my_prompt, “my_promPt”, &my_parent,
                    MY_PROMPT_TEXT_RESOURCE_ID,
                    GX_STYLE_BORDER_RAISED, MY_PROPMT_ID, &size);

/* If status is GX_SUCCESS the prompt “my_prompt” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_draw
- gx_prompt_event_process
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_get
- gx_prompt_text_id_set
- gx_prompt_text_set

## <a name="gx_prompt_draw"></a>gx_prompt_draw


Çizim istemi

### <a name="prototype"></a>Prototype

```C
VOID gx_prompt_draw(GX_PROMPT *prompt);
```

### <a name="description"></a>Açıklama

Bu hizmet bir istem pencere öğesi çizer. Bu hizmet, tuval yenilemesi sırasında Gux tarafından dahili olarak çağrılır, ancak özel çizim işlevleri tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem öğesi denetim bloğunun işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom prompt drawing function. */

VOID my_prompt_draw(GX_PROMPT *prompt)
{
    /* Call default prompt draw. */
    gx_prompt_draw(prompt);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_event_process
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_get
- gx_prompt_text_id_set
- gx_prompt_text_set

## <a name="gx_prompt_event_process"></a>gx_prompt_event_process


İşlem istemi olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_prompt_event_process(GX_PROMPT *prompt, GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen istem için bir olayı işler. Bu hizmet, özel istem olayı işleme işlevleri tarafından varsayılan olay işleyicisi olarak çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem denetim bloğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı istem olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic prompt event processing as part of custom event processing function. */

UINT custom_prompt_event_process(GX_PROMPT *prompt, GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;

    default:
        /* Pass all other events to the default prompt event processing */
        status = gx_prompt_event_process(prompt, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_get
- gx_prompt_text_id_set
- gx_prompt_text_set

## <a name="gx_prompt_font_set"></a>gx_prompt_font_set


İstem yazı tipini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_prompt_font_set(
    GX_PROMPT *prompt, 
    GX_RESOURCE_ID font_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir istem pencere öğesinin yazı tipini ayarlar.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem öğesi denetim bloğunun işaretçisi
- **font_id** Yazı tipinin kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı istem yazı tipi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the font of “my_prompt”. */
status = gx_prompt_font_set(&my_prompt, MY_PROMPT_FONT_ID);

/* If status is GX_SUCCESS the font for prompt “my_prompt” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_event_process
- gx_prompt_text_color_set
- gx_prompt_text_get
- gx_prompt_text_id_set
- gx_prompt_text_set

## <a name="gx_prompt_text_color_set"></a>gx_prompt_text_color_set


İstem metni rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_prompt_text_color_set(
    GX_PROMPT *prompt,
    GX_RESOURCE_ID normal_color,
    GX_RESOURCE_ID selected_color,
    GX_RESOURCE_ID disabled_color);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir istem pencere öğesinin metin rengini ayarlar.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem öğesi denetim bloğunun işaretçisi
- **normal_color** Normal metnin renginin kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **selected_color** Seçili metin için rengin kaynak KIMLIĞI, pencere öğesi odaklanıldığında kullanılır. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **disabled_color** GX_STYLE_ENABLED etkin olmadığında kullanılan, devre dışı bırakılan metnin renk kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı istem metin rengi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET_SIZE** (0x14) geçersiz pencere öğesi boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the text color of “my_prompt”. */
status = gx_prompt_text_color_set(&my_prompt,
                    GX_COLOR_ID_BLACK,
                    GX_COLOR_ID_LIGHTGRAY,
                    GX_COLOR_ID_DISABLED_TEXT);

/* If status is GX_SUCCESS the text color for prompt “my_prompt” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_event_process
- gx_prompt_font_set
- gx_prompt_text_get
- gx_prompt_text_id_set
- gx_prompt_text_set

## <a name="gx_prompt_text_draw"></a>gx_prompt_text_draw


Çizim desteği işlevi

### <a name="prototype"></a>Prototype

```C
VOID gx_prompt_text_draw(GX_PROMPT *prompt);
```

### <a name="description"></a>Açıklama

Bu destek işlevi bir istemin metin bölümünü çizer. Bu işlev, gx_prompt_draw () tarafından dahili olarak çağrılır ve özel bir istem çizimi işlevini tanımlayan uygulamalar için kolaylık olarak ayrı bir API olarak sağlanır. İstem arka plan çizimini özelleştirmek isteyen uygulamalar özel çizim işlevlerini sağlayabilir ve istem metnini arka planda çizmek için özel çiziminin bir parçası olarak gx_prompt_text_draw hizmetini çağırabilir.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem denetim bloğunun işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Define a custom drawing function */
VOID my_prompt_draw(GX_PROMPT *prompt)
{
    /* insert code here to draw prompt background */

    /* call support function to do text drawing */
    gx_prompt_text_draw();

    /* draw child widgets */
    gx_widget_children_draw((GX_WIDGET *) prompt);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_event_process
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_id_set
- gx_prompt_text_set

## <a name="gx_prompt_text_get"></a>gx_prompt_text_get


İstem metnini al (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_prompt_text_get(
    GX_PROMPT *prompt, 
    GX_CHAR **return_text);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_prompt_text_get_ext () kullanımı için kullanım dışıdır.

Bu hizmet bir istem pencere öğesinin metnini alır.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem öğesi denetim bloğunun işaretçisi
- **return_text** Metin için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı istem metni al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_PROMPT my_prompt;
GX_CHAR *my_prompt_text;

/* Get the text of “my_prompt”. */
status = gx_prompt_text_get(&my_prompt, &my_prompt_text);

/* If status is GX_SUCCESS the pointer “my_prompt_text” points to the text displayed by “my_prompt”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_event_process
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_id_set
- gx_prompt_text_set

## <a name="gx_prompt_text_get_ext"></a>gx_prompt_text_get_ext


İstem metnini al

### <a name="prototype"></a>Prototype

```C
UINT gx_prompt_text_get(
    GX_PROMPT *prompt, 
    GX_STRING *return_string);
```

### <a name="description"></a>Açıklama

Bu hizmet bir istem pencere öğesinin dizesini alır.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem öğesi denetim bloğunun işaretçisi
- **return_string** Dize için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı istem metni al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_PROMPT my_prompt;
GX_STRING my_prompt_string;

/* Get the text of “my_prompt”. */
status = gx_prompt_text_get_ext(&my_prompt, &my_prompt_string);

/* If status is GX_SUCCESS then my_prompt_string has been initialize to hold a copy of the prompt string. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_event_process
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_id_set
- gx_prompt_text_set

## <a name="gx_prompt_text_id_set"></a>gx_prompt_text_id_set


İstem metin KIMLIĞINI ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_prompt_text_id_set(
    GX_PROMPT *prompt, 
    GX_RESOURCE_ID string_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin istemi pencere öğesi için dize KIMLIĞINI ayarlar.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem öğesi denetim bloğunun işaretçisi
- **string_id** Dizenin kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı Istem metni kimliği kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_SYSTEM_MEMORY_ERROR** (0x30) bellek boş işlevi tanımlı değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the string ID of “my_prompt”. */
status = gx_prompt_text_id_set(&my_prompt, MY_STRING_ID);

/* If status is GX_SUCCESS the text ID for prompt “my_prompt” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_event_process
- gx_prompt_font_set
- gx_prompt_text_get
- gx_prompt_text_set

## <a name="gx_prompt_text_set"></a>gx_prompt_text_set


İstem metnini ayarla (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_prompt_text_set(
    GX_PROMPT *prompt, 
    GX_CHAR *text);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_prompt_text_set_ext () kullanım dışı bırakılmıştır.

Bu hizmet bir istem pencere öğesinin metnini ayarlar. İstem pencere öğesi stil GX_STYLE_TEXT_COPY ile oluşturulduysa pencere öğesi, atanan metin dizesinin özel bir kopyasını oluşturur. GX_STYLE_TEXT_COPY etkin değilse, pencere öğesi gelen dizenin özel bir kopyasını oluşturmaz, bu nedenle dize statik veya genel olarak ayrılmış olmalıdır, yani bu bir otomatik veya geçici değişken olmayabilir.

GX_PROMPT GX_WIDGET türetilir ve bu nedenle tüm gx_widget API hizmetleri GX_PROMPT ile kullanılabilir.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem öğesi denetim bloğunun işaretçisi
- **metin** Metin işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı istem metin kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_SYSTEM_MEMORY_ERROR** (0x30) bellek ayırma işlevi tanımlı değil
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the text of “my_prompt” to “my_text”. */
status = gx_prompt_text_set(&my_prompt, “my_text”);

/* If status is GX_SUCCESS the text for “my_prompt” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_event_process
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_id_set
- gx_prompt_text_get

## <a name="gx_prompt_text_set_ext"></a>gx_prompt_text_set_ext

İstem metnini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_prompt_text_set_ext(
    GX_PROMPT *prompt,
    GX_STRING *string);
```

### <a name="description"></a>Açıklama

Bu hizmet bir istem pencere öğesinin metnini ayarlar. İstem pencere öğesi stil GX_STYLE_TEXT_COPY ile oluşturulduysa pencere öğesi, atanan metin dizesinin özel bir kopyasını oluşturur. GX_STYLE_TEXT_COPY etkin değilse, pencere öğesi gelen dizenin özel bir kopyasını oluşturmaz, bu nedenle dize statik veya genel olarak ayrılmış olmalıdır, yani bu bir otomatik veya geçici değişken olmayabilir.

GX_PROMPT GX_WIDGET türetilir ve bu nedenle tüm gx_widget API hizmetleri GX_PROMPT ile kullanılabilir.

### <a name="parameters"></a>Parametreler

- **komut istemi** İstem öğesi denetim bloğunun işaretçisi
- **metin** Metin işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı istem metin kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_SYSTEM_MEMORY_ERROR** (0x30) bellek ayırma işlevi tanımlı değil
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING new_string;
new_string.gx_string_ptr = “my_text”;
new_string.gx_string_length = strlen(new_string.gx_string_ptr);

/* Set the text of “my_prompt” to “new_string”. */
status = gx_prompt_text_set(&my_prompt, &new_string);

/* If status is GX_SUCCESS the text for “my_prompt” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_prompt_create
- gx_pixelmap_prompt_draw
- gx_pixelmap_prompt_pixelmap_set
- gx_prompt_create
- gx_prompt_draw
- gx_prompt_event_process
- gx_prompt_font_set
- gx_prompt_text_color_set
- gx_prompt_text_id_set
- gx_prompt_text_get

## <a name="gx_radial_progress_bar_anchor_set"></a>gx_radial_progress_bar_anchor_set


Başlangıç açısını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_progress_bar_anchor_set(
    GX_RADIAL_PROGRESS_BAR *progress_bar, 
    GX_VALUE angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal ilerleme çubuğu için başlangıç açısını ayarlar.

### <a name="parameters"></a>Parametreler

- radyal ilerleme çubuğu denetim bloğu için **ilerleme** çubuğu işaretçisi
- **açı** Dairesel ark başlangıç açısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal ilerleme çubuğu tutturucu kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_VALUE start_angle = 90;

/* Set the start angle of “my_progress_bar” to 90 degree. */
status = gx_radial_progress_bar_anchor_set(&my_progress_bar, start_angle);

/* If status is GX_SUCCESS the anchor value of “my_progress_bar” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_background_draw
- gx_radial_progress_bar_create
- gx_radial_progress_bar_draw
- gx_radial_progress_bar_event_process
- gx_radial_progress_bar_font_set
- gx_radial_progress_bar_info_set
- gx_radial_progress_bar_text_color_set
- gx_radial_progress_bar_text_draw
- gx_radial_progress_bar_value_set

## <a name="gx_radial_progress_bar_background_draw"></a>gx_radial_progress_bar_background_draw


Arka plan çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_radial_progress_bar_background_draw(GX_RADIAL_PROGRESS_BAR *progress_bar);
```

### <a name="description"></a>Açıklama

Bu hizmet bir radyal ilerleme çubuğu arka planı çizer. Bu hizmete gx_radial_progress_bar_draw işlevi tarafından dahili olarak başvuruluyor, ancak uygulamanın özel bir radyal ilerleme çubuğu çizim işlevini tanımladığı durumlarda uygulama tarafından kullanıma sunuldu

### <a name="parameters"></a>Parametreler

- **ilerleme çubuğu** Radyal ilerleme çubuğu denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom radial progress bar drawing function. */

VOID my_radial_progress_bar_draw(GX_RADIAL_PROGRESS_BAR *radial_progress)
{
    /* Call default radial progress bar background draw. */
    gx_radial_progress_bar_background_draw(radial_progress);

    /* Add your own drawing here. */

    /* Draw child widgets. */
    gx_widget_children_draw((GX_WIDGET *)radial_progress);
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_anchor_set
- gx_radial_progress_bar_create
- gx_radial_progress_bar_draw
- gx_radial_progress_bar_event_process
- gx_radial_progress_bar_font_set
- gx_radial_progress_bar_info_set
- gx_radial_progress_bar_text_color_set
- gx_radial_progress_bar_text_draw
- gx_radial_progress_bar_value_set

## <a name="gx_radial_progress_bar_create"></a>gx_radial_progress_bar_create


Radyal ilerleme çubuğu oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_progress_bar_create(
    GX_RADIAL_PROGRESS_BAR *progress_bar,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_RADIAL_PROGRESS_BAR_INFO *info,
    ULONG style
    USHORT id);
```

### <a name="description"></a>Açıklama

Bu hizmet bir radyal ilerleme çubuğu oluşturur.

Pencere öğesi stili GX_STYLE_ENABLED ilerleme çubuğuna uygulanmışsa, ilerleme çubuğu geçerli değeri değiştirmek için pen_down, pen_drag ve pen_up girişi kabul eder.

GX_STYLE_PROGRESS_TEXT_DRAW pencere öğesi stili, ilerleme çubuğu değerini ilerleme çubuğu alanı içinde metin olarak çizmeyi etkinleştirmek için kullanılabilir. Bu stil GX_STYLE_PROGRESS_PERCENT stille birlikte kullanılırsa, ilerleme çubuğu değeri yüzde olarak görüntülenir. Aksi takdirde, ilerleme çubuğu değeri geçerli angular değeri olarak görüntülenir.

### <a name="parameters"></a>Parametreler

- **ilerleme çubuğu** Radyal ilerleme çubuğu denetimine yönelik işaretçi
- radyal ilerleme çubuğu denetim bloğu için **ilerleme** çubuğu işaretçisi
- **ad** Radyal ilerleme çubuğunun adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **bilgi** GX_RADIAL_PROGRESS_BAR yapısına yönelik işaretçi. **Ek ı** GX_RADIAL_PROGRESS_BAR yapısı için tanım içeriyor.
- **Stil** Radyal ilerleme çubuğu stili
- uygulama tarafından tanımlanan **kimlik** ilerleme çubuğunun kimliği

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal ilerleme çubuğu oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_WIDGET** (0x12) geçersiz üst pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RAIDAL_PROGRESS_BAR_INFO info;

info.gx_radial_progress_bar_info_xcenter = 200;
info.gx_radial_progress_bar_info_ycenter = 200;
info.gx_radial_progress_bar_info_radius = 100;
info.gx_radial_progress_bar_info_current_angle = 180;
info.gx_radial_progress_bar_info_anchor_val = -180;
info.gx_radial_progress_bar_info_font_id = GX_FONT_ID_SYSTEM;
info.gx_raidal_progress_bar_info_normal_text_color =
                                        GX_COLOR_ID_TEXT;
info.gx_radial_progress_bar_info_selected_text_color =
                                        GX_COLOR_ID_TEXT;
info.gx_radial_progress_bar_info_disabled_text_color =
                                        GX_COLOR_ID_DISABLED_TEXT;
info.gx_radial_progress_bar_info_normal_brush_width = 20;
info.gx_raidal_progress_bar_info_selected_brush_width = 16;
info.gx_radial_progress_bar_info_normal_brush_color =
                                        GX_COLOR_ID_WIDGET_FILL;
info.gx_radial_progress_bar_info_selected_brush_color =
                                        GX_COLOR_ID_SELECTED_FILL;

/* Create a radial progress bar “my_progress_bar”. */
status = gx_radial_progress_bar_create(&my_progress_bar,
                    “my_progress_bar”, parent, &info,
                    GX_STYLE_ENABLED | GX_STYLE_TRANSPARENT |
                    GX_STYLE_PROGRESS_TEXT_DRAW,
                    ID_MY_RADIAL_PROGRESS);

/* If status is GX_SUCCESS the radial progress bar “my_progress_bar” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_anchor_set
- gx_radial_progress_bar_background_draw
- gx_radial_progress_bar_draw
- gx_radial_progress_bar_event_process
- gx_radial_progress_bar_font_set
- gx_radial_progress_bar_info_set
- gx_radial_progress_bar_text_color_set
- gx_radial_progress_bar_text_draw
- gx_radial_progress_bar_value_set

## <a name="gx_radial_progress_bar_draw"></a>gx_radial_progress_bar_draw


Radyal ilerleme çubuğu çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_radial_progress_bar_draw(GX_RADIAL_PROGRESS_BAR *progress_bar);
```

### <a name="description"></a>Açıklama

Bu hizmet bir radyal ilerleme çubuğu çizer. Bu hizmet gx_radial_progress_bar_create işlevi tarafından dahili olarak başvurulur, ancak uygulamanın özel bir radyal ilerleme çubuğu çizim işlevini tanımladığı durumlarda uygulama tarafından kullanıma sunulur.

### <a name="parameters"></a>Parametreler

- **ilerleme çubuğu** Radyal ilerleme çubuğu denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom radial progress bar drawing function. */

VOID my_radial_progress_bar_draw(GX_RADIAL_PROGRESS_BAR *radial_progress)
{
    /* Call default radial progress bar draw. */
    gx_radial_progress_bar_draw(radial_progress);

    /* Add your own drawing here. */

    /* Draw child widgets. */
    gx_widget_children_draw((GX_WIDGET *)radial_progress);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_anchor_set
- gx_radial_progress_bar_background_draw
- gx_radial_progress_bar_create
- gx_radial_progress_bar_event_process
- gx_radial_progress_bar_font_set
- gx_radial_progress_bar_info_set
- gx_radial_progress_bar_size_calculate
- gx_radial_progress_bar_text_color_set
- gx_radial_progress_bar_text_draw
- gx_radial_progress_bar_value_set

## <a name="gx_radial_progress_bar_event_process"></a>gx_radial_progress_bar_event_process


Radyal ilerleme çubuğu olayını işle

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_progress_bar_event_process(
    GX_RADIAL_PROGRESS_BAR *progress_bar,
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet bir radyal ilerleme çubuğu olayını işler. Bu işleve gx_radial_progress_bar_create işlevi tarafından dahili olarak başvurulur, ancak uygulamanın özel bir radyal ilerleme olayı işleme işlevini tanımladığı durumlarda uygulama tarafından kullanıma sunulur.

### <a name="parameters"></a>Parametreler

- radyal ilerleme çubuğu denetim bloğu için **ilerleme** çubuğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal ilerleme çubuğu olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom event processing function. */

UINT my_event_process (GX_RADIAL_PROGRESS_BAR *radial_progress, GX_EVENT *event_ptr)
{
    switch(event_ptr->gx_event_type)
    {
        case GX_EVENT_SHOW:
        /* Do default handling. */
        status = gx_radial_progress_bar_event_process(
                            radial_progress, event_ptr);
        /* add my own handling here */
        break;
    default:
        status = gx_radial_progress_bar_event_process(
                            radial_progress, event_ptr);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_anchor_set
- gx_radial_progress_bar_background_draw
- gx_radial_progress_bar_create
- gx_radial_progress_bar_draw
- gx_radial_progress_bar_font_set
- gx_radial_progress_bar_info_set
- gx_radial_progress_bar_text_color_set
- gx_radial_progress_bar_text_draw
- gx_radial_progress_bar_value_set

## <a name="gx_radial_progress_bar_font_set"></a>gx_radial_progress_bar_font_set


Radyal ilerleme çubuğu yazı tipini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_progress_bar_font_set(
    GX_RADIAL_PROGRESS_BAR *progress_bar,
    GX_RESOURCE_ID font_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal ilerleme çubuğu pencere öğesinin yazı tipini ayarlar. Pencere öğesi stili GX_STYLE_PROGRESS_TEXT_DRAW ayarlanmamışsa bu parametrenin etkisi yoktur.

### <a name="parameters"></a>Parametreler

- radyal ilerleme çubuğu denetim bloğu için **ilerleme** çubuğu işaretçisi
- **font_id** Yazı tipinin kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal ilerleme çubuğu yazı tipi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set font for radial progress bar “my_progress_bar”. */
status = gx_radial_progress_bar_font_set(&my_progress_bar, font);

/* If status is GX_SUCCESS the font of “my_progress_bar” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_anchor_set
- gx_radial_progress_bar_background_draw
- gx_radial_progress_bar_create
- gx_radial_progress_bar_draw
- gx_radial_progress_bar_event_process
- gx_radial_progress_bar_info_set
- gx_radial_progress_bar_text_color_set
- gx_radial_progress_bar_text_draw
- gx_radial_progress_bar_value_set

## <a name="gx_radial_progress_bar_info_set"></a>gx_radial_progress_bar_info_set


Radyal ilerleme çubuğu bilgilerini ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_progress_bar_info_set(
    GX_RADIAL_PROGRESS_BAR *progress_bar,
    GX_RADIAL_PROGRESS_BAR_INFO *info);
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal ilerleme çubuğuna atanan bilgi parametrelerini sıfırlar.

### <a name="parameters"></a>Parametreler

- radyal ilerleme çubuğu denetim bloğu için **ilerleme** çubuğu işaretçisi
- **bilgi** Radyal ilerleme çubuğu bilgi yapısına yönelik işaretçi. **Ek ı** GX_RADIAL_PROGRESS_BAR_INFO yapısı için tanım içeriyor.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal ilerleme çubuğu bilgi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RAIDAL_PROGRESS_BAR_INFO info;

info.gx_radial_progress_bar_info_xcenter = 200;
info.gx_radial_progress_bar_info_ycenter = 200;
info.gx_radial_progress_bar_info_radius = 100;
info.gx_radial_progress_bar_info_current_angle = 180;
info.gx_radial_progress_bar_info_anchor_val = -180;
info.gx_radial_progress_bar_info_font_id = GX_FONT_ID_SYSTEM;
info.gx_raidal_progress_bar_info_normal_text_color =
                                GX_COLOR_ID_TEXT;
info.gx_radial_progress_bar_info_selected_text_color =
                                GX_COLOR_ID_TEXT;
info.gx_radial_progress_bar_info_disabled_text_color =
                                GX_COLOR_ID_DISABLED_TEXT;
info.gx_radial_progress_bar_info_normal_brush_width = 20;
info.gx_raidal_progress_bar_info_selected_brush_width = 16;
info.gx_radial_progress_bar_info_normal_brush_color =
                                GX_COLOR_ID_WIDGET_FILL;
info.gx_radial_progress_bar_info_selected_brush_color =
                                GX_COLOR_ID_SELECTED_FILL;

/* Set appearance information for radial progress bar “my_progress_bar”. */
status = gx_radial_progress_bar_info_set(&my_progress_bar, &info);

/* If status is GX_SUCCESS the appearance information of “my_progress_bar” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_anchor_set
- gx_radial_progress_bar_background_draw
- gx_radial_progress_bar_create
- gx_radial_progress_bar_draw
- gx_radial_progress_bar_event_process
- gx_radial_progress_bar_font_set
- gx_radial_progress_bar_text_color_set
- gx_radial_progress_bar_text_draw
- gx_radial_progress_bar_value_set

## <a name="gx_radial_progress_bar_text_color_set"></a>gx_radial_progress_bar_text_color_set


Radyal ilerleme çubuğu metin rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_progress_bar_text_color_set(
    GX_RADIAL_PROGRESS_BAR *progress_bar,
    GX_RESOURCE_ID normal_text_color,
    GX_RESOURCE_ID selected_text_color,
    GX_RESOURCE_ID disabled_text_color);
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal ilerleme çubuğunun metin rengini ayarlar. Bu değer yalnızca Style GX_STYLE_PROGRESS_TEXT_DRAW ayarlandıysa kullanılır.

### <a name="parameters"></a>Parametreler

- radyal ilerleme çubuğu denetim bloğu için **ilerleme** çubuğu işaretçisi
- **normal_color** Normal durumdaki metin renginin kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **selected_color** Pencere öğesi odaklanıldığında metin renginin kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **disabled_color** Stil GX_STYLE_ENABLED ayarlanmamışsa metin renginin kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal ilerleme çubuğu metin rengi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi denetimi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set text color for radial progress bar “my_progress_bar”. */
status = gx_radial_progress_bar_text_color_set(&my_progress_bar,
                            GX_COLOR_ID_NORMAL_TEXT,
                            GX_COLOR_ID_SELECTED_TEXT,
                            GX_COLOR_ID_DISABLED_TEXT);

/* If status is GX_SUCCESS the text color of “my_progress_bar” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_anchor_set
- gx_radial_progress_bar_background_draw
- gx_radial_progress_bar_create
- gx_radial_progress_bar_draw
- gx_radial_progress_bar_event_process
- gx_radial_progress_bar_font_set
- gx_radial_progress_bar_info_set
- gx_radial_progress_bar_text_draw
- gx_radial_progress_bar_value_set

## <a name="gx_radial_progress_bar_text_draw"></a>gx_radial_progress_bar_text_draw


Radyal ilerleme çubuğu metni çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_radial_progress_bar_text_draw(GX_RADIAL_PROGRESS_BAR *progress_bar);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen radyal ilerleme çubuğunun metnini çizer. Bu işlev, gx_radial_progress_bar_draw () bir parçası olarak dahili olarak çağrılır, ancak uygulamanın özel bir ilerleme çubuğu çizim işlevini tanımladığı bu durumları desteklemek için uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **ilerleme çubuğu** Radyal ilerleme çubuğu denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

Başlatma ve Iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Draw text for radial progress bar “my_progress_bar”. */
status = gx_radial_progress_bar_text_draw (&my_progress_bar);

/* If status is GX_SUCCESS the text of “my_progress_bar” has been drawn. */

/* Write a custom radial progress bar drawing function. */
VOID my_radial_progress_bar_draw(GX_RADIAL_PROGRESS_BAR *radial_progress)
{
    /* Add your own background draw here. */

    /* Call default radial progress bar text draw. */
    gx_radial_progress_bar_text_draw(radial_progress);

    /* Draw child widgets. */
    gx_widget_children_draw((GX_WIDGET *)radial_progress);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_anchor_set
- gx_radial_progress_bar_background_draw
- gx_radial_progress_bar_create
- gx_radial_progress_bar_draw
- gx_radial_progress_bar_event_process
- gx_radial_progress_bar_font_set
- gx_radial_progress_bar_info_set
- gx_radial_progress_bar_text_color_set
- gx_radial_progress_bar_value_set

## <a name="gx_radial_progress_bar_value_set"></a>gx_radial_progress_bar_value_set


Radyal ilerleme çubuğu değerini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_progress_bar_value_set(
    GX_RADIAL_PROGRESS_BAR *progress_bar, 
    GX_VALUE value);
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal ilerleme çubuğu değerini ayarlar. Atanan değer [-360, 360] aralığı ile sınırlıdır ve ilerleme çubuğu geçerli konumu için olası Ansal değer aralığını tanımlar. Uygulama, ilerleme çubuğu pencere öğesine angular değeri atamak için belirtilen gerçek uluslararası değeri ölçeklendirmelidir.

İlerleme çubuğu, geçerli değerin, üst yayı yer işareti konumu ve bitiş noktası arasındaki açısal değişikliği gösterdiği şekilde çizilir. Negatif değerler, Arc konumundan başlayarak saat yönünde bir yönde çizilmesine neden olur. Pozitif geçerli değer, bağlayıcının bağlantı konumundan başlayan saat yönünde bir yönde çizilmesini sağlar.

Örneğin, yayı en üstünde (12 saat konum) başlayan ve sağ tarafta (üç saat içinde) biten bir yay çizmek için 90 derece bir bağlantı değeri ve geçerli-90 derece değeri atayın.

### <a name="parameters"></a>Parametreler

- radyal ilerleme çubuğu denetim bloğu için **ilerleme** çubuğu işaretçisi
- **değer** Yeni ilerleme çubuğu değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal ilerleme çubuğu değer kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçiler
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_VALUE new_value = 180;

/* Set value for radial progress bar “my_progress_bar”. */
status = gx_radial_progress_bar_value_set(&my_progress_bar,
                                        new_value);

/* If status is GX_SUCCESS the value of “my_progress_bar” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_progress_bar_anchor_set
- gx_radial_progress_bar_background_draw
- gx_radial_progress_bar_create
- gx_radial_progress_bar_draw
- gx_radial_progress_bar_event_process
- gx_radial_progress_bar_font_set
- gx_radial_progress_bar_info_set
- gx_radial_progress_bar_text_color_set
- gx_radial_progress_bar_text_draw

## <a name="gx_radio_button_create"></a>gx_radio_button_create


Radyo düğmesi oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_radio_button_create(
    GX_RADIO_BUTTON *button,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_RESOURCE_ID text_id, ULONG style,
    USHORT radio_button_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir radyo düğmesi pencere öğesi oluşturur. GX_RADIO_BUTTON GX_TEXT_BUTTON türetilir ve bu nedenle tüm gx_text_button hizmetleri de bu pencere öğesi türü tarafından desteklenir.

### <a name="parameters"></a>Parametreler

- **düğme** Radyo düğmesi denetim bloğu işaretçisi
- **ad** Radyo düğmesi pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **text_id** Radyo düğmesinin kaynak KIMLIĞI
- **Stil** Radyo düğmesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **radio_button_id** Uygulama tanımlı radyo düğmesi KIMLIĞI
- **Boyut** Radyo düğmesinin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyo düğmesi oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_** Boyut (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_radio_button”. */
status = gx_radio_button_create(&my_radio_button, “my_radio_button”, &my_parent,
                    MY_RADIO_BUTTON_TEXT_RESOURCE_ID,
                    GX_STYLE_BORDER_RAISED, MY_RADIO_BUTTON_ID, &size);

/* If status is GX_SUCCESS the radio button “my_radio_button” has been created. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw
- gx_radio_button_draw

## <a name="gx_radio_button_draw"></a>gx_radio_button_draw


Çizim radyo düğmesi

### <a name="prototype"></a>Prototype

```C
VOID gx_radio_button_draw(GX_RADIO_BUTTON *button);
```

### <a name="description"></a>Açıklama

Bu hizmet bir radyo düğmesi pencere öğesi çizer. Bu hizmet, Gux tuvali yenilemesi tarafından dahili olarak çağrılır, ancak geçersiz kılınan çizim işlevleri tarafından çağrılabilir.

### <a name="parameters"></a>Parametreler

- **düğme** Radyo düğmesi pencere öğesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom radio button drawing function. */

VOID my_radio_button_draw(GX_RADIO_BUTTON *radio_button)
{
    /* Call default radio button draw. */
    gx_radio_button_draw(radio_button);

    /* Add your own drawing here. */

    /* Draw child widgets. */
    gx_widget_children_draw((GX_WIDGET *)radio_button);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw
- gx_radio_button_create

## <a name="gx_radio_button_pixelmap_set"></a>gx_radio_button_pixelmap_set


Radyo düğmesi için pixelmaps ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_radio_button_pixelmap_set(
    GX_RADIO_BUTTON *button,
    GX_RESOURCE_ID off_id,
    GX_RESOURCE_ID on_id,
    GX_RESOURCE_ID off_disabled_id,
    GX_RESOURCE_ID on_disabled_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, her düğme durumu için belirtilen radyo düğmesi tarafından görüntülenecek pixelmaps 'ı atar. Kaynak kimlikleri yinelenebilir.

### <a name="parameters"></a>Parametreler

- **off_id** Radyo düğmesi kapalı durumu için kullanılan pixelmap
- **on_id** Durum üzerinde radyo düğmesi için pixelmap kullanıldı
- **off_disabled_id** Radyo düğmesi devre dışı ve kapalı durumu için kullanılan pixelmap
- **on_disabled_id** Radyomap radyo düğmesi devre dışı ve durum durumunda kullanıldı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyo düğmesi pixelmaps kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set pixelmap for “my_radio_button”. */
status = gx_radio_button_pixelmap_set(&my_radio_button,
                                MY_OFF_PIXELMAP,
                                MY_ON_PIXELMAP,
                                MY_OFF_DISABLED_PIXELMAP,
                                MY_ON_DISABLED_PIXELMAP);

/* If status is GX_SUCCESS the pixelmaps for radio button “my_radio_button” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_color_set
- gx_text_button_draw
- gx_radio_button_create

## <a name="gx_radial_slider_anchor_angles_set"></a>gx_radial_slider_anchor_angles_set


Radyal kaydırıcı bağlayıcı listesini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_slider_anchor_angles_set(
    GX_RADIAL_SLIDER *slider,
    GX_VALUE *anchor_angles, 
    USHORT anchor_count);
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal kaydırıcı için bağlantı açılarını ayarlar. Çapa açısı listesi ayarlandıysa, radyal kaydırıcı açısı tanımlı çapa açılarının biri olacaktır.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu
- **anchor_angles** Ayarlanacak açı listesi
- **anchor_count** Çapa açılarının sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı bağlayıcı açısı kümesi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi
- **GX_INVALID_VALUE** (0x22) geçersiz bağlantı listesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_VALUE anchor_angles[]={0, 30, 60, 90, 120, 150, 180};
USHORT anchor_count = 7;

/* Set anchor angles for radial slider. */
status = gx_radial_slider_anchor_angles_set(&my_radial_slider,
                                anchor_angles, anchor_count);

/* If status is GX_SUCCESS the anchor angles have been set for “my_radial_slider”. */

/* Set anchor angles for radial slider. */
status = gx_radial_slider_anchor_angles_set(&my_radial_slider,
                                GX_NULL, 0);

/* If status is GX_SUCCESS the anchor angles have been removed from “my_radial_slider”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_angle_set
- gx_radial_slider_animation_set
- gx_radial_slider_animation_start
- gx_radial_slider_create
- gx_radial_slider_draw
- gx_radial_slider_event_process
- gx_radial_slider_info_get
- gx_radial_slider_info_set
- gx_radial_slider_pixelmap_set

## <a name="gx_radial_slider_angle_set"></a>gx_radial_slider_angle_set

Radyal kaydırıcı açısını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_slider_angle_set(
    GX_RADIAL_SLIDER *slider,
    GX_VALUE new_angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal kaydırıcı için yeni açılı değeri ayarlar.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu işaretçisi
- **new_angle** Ayarlanacak yeni açı değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal kaydırıcı açısı kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set “my_radial_slider” angle to 0 degree(3 o’clock position). */
status = gx_radial_slider_angle_set(&my_radial_slider, 0);

/* If status is GX_SUCCESS the value of “my_radial_slider” has been set to 0 degree. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_anchor_angles_set
- gx_radial_slider_animation_set
- gx_radial_slider_animation_start
- gx_radial_slider_create
- gx_radial_slider_draw
- gx_radial_slider_event_process
- gx_radial_slider_info_get
- gx_radial_slider_info_set
- gx_radial_slider_pixelmap_set

## <a name="gx_radial_slider_animation_set"></a>gx_radial_slider_animation_set


Radyal kaydırıcı animasyon bilgisi oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_slider_animation_set(
    GX_RADIAL_SLIDER *slider,
    USHORT steps, USHORT delay, 
    USHORT animation_style,
    VOID (*animation_update_callback)(GX_RADIAL_SLIDER *slider));
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal kaydırıcı iğne animasyonu için animasyon adımlarını, gecikme süresini ve animasyon stillerini ayarlar.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu işaretçisi
- **adımlar** Tek animasyon için toplam adım
- **gecikme** Her animasyon adımı için gecikme süresi
- **animation_style** Kolaylaştırıcı işlev türü şunları içerir:
  - GX_ANIMATION_BACK_EASE_IN
  - GX_ANIMATION_BACK_EASE_OUT
  - GX_ANIMATION_BACK_EASE_IN_OUT
  - GX_ANIMATION_BOUNCE_EASE_IN
  - GX_ANIMATION_BOUNCE_EASE_OUT
  - GX_ANIMATION_BOUNCE_EASE_IN_OUT
  - GX_ANIMATION_CIRC_EASE_IN
  - GX_ANIMATION_CIRC_EASE_OUT
  - GX_ANIMATION_CIRC_EASE_IN_OUT
  - GX_ANIMATION_CUBIC_EASE_IN
  - GX_ANIMATION_CUBIC_EASE_OUT
  - GX_ANIMATION_CUBIC_EASE_IN_OUT
  - GX_ANIMATION_ELASTIC_EASE_IN
  - GX_ANIMATION_ELASTIC_EASE_OUT
  - GX_ANIMATION_ELASTIC_EASE_IN_OUT
  - GX_ANIMATION_EXPO_EASE_IN
  - GX_ANIMATION_EXPO_EASE_OUT
  - GX_ANIMATION_EXPO_EASE_IN_OUT
  - GX_ANIMATION_QUAD_EASE_IN
  - GX_ANIMATION_QUAD_EASE_OUT
  - GX_ANIMATION_QUAD_EASE_IN_OUT
  - GX_ANIMATION_QUART_EASE_IN
  - GX_ANIMATION_QUART_EASE_OUT
  - GX_ANIMATION_QUART_EASE_IN_OUT
  - GX_ANIMATION_QUINT_EASE_IN
  - GX_ANIMATION_QUINT_EASE_OUT
  - GX_ANIMATION_QUINT_EASE_IN_OUT
  - GX_ANIMATION_SINE_EASE_IN
  - GX_ANIMATION_SINE_EASE_OUT
  - GX_ANIMATION_SINE_EASE_IN_OUT
- **animation_update_callback** Her animasyon adımından sonra çağrılacak Kullanıcı tanımlı geri çağırma işlevi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal kaydırıcı animasyon kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
VOID animation_callback(GX_RADIAL_SLIDER *slider)
{
    /* This function will be called after each animation step,
    add custom code here. */
}

/* Set animation info for “my_radial_slider”. */
status = gx_radial_slider_animation_set(&my_radial_slider, 15, 2,
                                GX_ANIMATION_CIRC_EASE_IN_OUT,
                                animation_callback);

/* If status is GX_SUCCESS the radial slider needle will move with specified animation. */

/* Disable animation for “my_radial_slider”. */
status = gx_radial_slider_animation_set(&my_radial_slider, 0, 0,
                                        0, 0);

/* If status is GX_SUCCESS the radial slider needle will move without animation. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_anchor_angles_set
- gx_radial_slider_angle_set
- gx_radial_slider_animation_start
- gx_radial_slider_create
- gx_radial_slider_draw
- gx_radial_slider_event_process
- gx_radial_slider_info_get
- gx_radial_slider_info_set
- gx_radial_slider_pixelmap_set

## <a name="gx_radial_slider_animation_start"></a>gx_radial_slider_animation_start


Animasyonla yeni radyal kaydırıcı değeri ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_slider_animation_start(
    GX_RADIAL_SLIDER *slider,
    GX_VALUE target_angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırıcı iğne 'yi geçerli konumdan belirtilen konuma taşımak için bir animasyon başlatır.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu işaretçisi
- **target_angle** Hedef açı değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal kaydırıcı animasyon başlangıcı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Start an animation to move radial slider needle from
current position to 90 degree position. */
status = gx_radial_slider_animation_start(&my_radial_slider, 90);

/* If status is GX_SUCCESS the radial slider needle animation has been started. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_anchor_angles_set
- gx_radial_slider_angle_set
- gx_radial_slider_animation_set
- gx_radial_slider_create
- gx_radial_slider_draw
- gx_radial_slider_event_process
- gx_radial_slider_info_get
- gx_radial_slider_info_set
- gx_radial_slider_pixelmap_set

## <a name="gx_radial_slider_create"></a>gx_radial_slider_create


Radyal kaydırıcı oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_slider_create(
    GX_RADIAL_SLIDER *slider,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_RADIAL_SLIDER_INFO *info,
    ULONG style,
    USHORT slider_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir radyal kaydırıcı pencere öğesi oluşturur.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu işaretçisi
- **ad** Radyal kaydırıcı pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **bilgi** Radyal kaydırıcı görünüm tanımı, **ek i** GX_RADIAL_SLIDER_INFO tanım içeriyor.
- **Stil** Radyo düğmesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **radio_button_id** Radyal kaydırıcının uygulama tanımlı KIMLIĞI
- **Boyut** Radyal kaydırıcı boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal kaydırıcı oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_** Boyut (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET** (0x12) geçersiz üst pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RADIAL_SLIDER_INFO info;
GX_RECTANGLE size;

/* Distance from left side of widget to rotating center. */
info.gx_radial_slider_info_xcenter = 100;

/* Distance from top size of widget to rotating center. */
info.gx_radial_slider_info_ycenter = 100;

/* Radius of rotating circle. */
info.gx_radial_slider_info_radius = 100;

/* Widget of rotating track. */
info.gx_radial_slider_info_track_width = 40;

/* Current angle value. */
info.gx_radial_slider_info_current_angle = 0;

/* Minimum angle value. */
info.gx_radial_slider_min_anlge = -60;

/* Maximum angle value. */
info.gx_radial_slider_max_angle = 240;

/* Anchor value list. */
info.gx_radial_slider_angle_list = GX_NULL;

/* Anchor value count. */
info.gx_radial_slider_list_count = 0;

/* Resource ID of background pixelmap. */
info.gx_radial_slider_background_pixelmap = GX_PIXELMAP_ID_BKGRD;

/* Resource ID of needle pixelmap. */
info.gx_radial_slider_needle_pixelmap = GX_PIXELMAP_ID_NEEDLE;

/* Define widget size. */
gx_utility_rectangle_define(&size, 0, 0, 200, 200);

/* Create “my_radial_slider”. */
status = gx_radial_slider_create(&my_radial_slider,
                                “my_radial_slider”, &my_parent,
                                &info, GX_STYLE_ENABLED,
                                MY_RADIAL_SLIDER_ID, &size);

/* If status is GX_SUCCESS the radial slider “my_radial_slider” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_anchor_angles_set
- gx_radial_slider_angle_set
- gx_radial_slider_animation_set
- gx_radial_slider_animation_start
- gx_radial_slider_draw
- gx_radial_slider_event_process
- gx_radial_slider_info_get
- gx_radial_slider_info_set
- gx_radial_slider_pixelmap_set

## <a name="gx_radial_slider_draw"></a>gx_radial_slider_draw


Radyal kaydırıcı çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_radial_slider_draw(GX_RADIAL_SLIDER *slider);
```

### <a name="description"></a>Açıklama

Bu hizmet bir radyal kaydırıcı çizer. Bu hizmet, Gux tuvali yenilemesi tarafından dahili olarak çağrılır, ancak geçersiz kılınan çizim işlevleri tarafından çağrılabilir.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom radio button drawing function. */

VOID my_radial_slider_draw(GX_RADIAL_SLIDER *radial_slider)
{
    /* Call default radial slider draw. */
    gx_radio_slider_draw(radial_slider);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_anchor_angles_set
- gx_radial_slider_angle_set
- gx_radial_slider_animation_set
- gx_radial_slider_animation_start
- gx_radial_slider_create
- gx_radial_slider_draw
- gx_radial_slider_event_process
- gx_radial_slider_info_get
- gx_radial_slider_info_set
- gx_radial_slider_pixelmap_set

## <a name="gx_radial_slider_event_process"></a>gx_radial_slider_event_process


Radyal kaydırıcı olayını işle

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_slider_event_process(
    GX_RADIAL_SLIDER *slider,
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet bir radyal kaydırıcı olayını işler. Bu hizmet özel bir radyal kaydırıcı olay işleme işlevleri tarafından varsayılan olay işleyicisi olarak çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal kaydırıcı olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom event processing function. */

UINT my_event_process(GX_RADIAL_SLIDER *slider,
                    GX_EVENT *event_ptr)
{
    switch(event_ptr->gx_event_type)
    {
    case GX_EVENT_SHOW:
        /* Do default handling. */
        status = gx_radial_slider_event_process(slider, event_ptr);

        /* add my own handling here */
        break;
    default:
        status = gx_radial_slider_event_process(slider, event_ptr);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_anchor_angles_set
- gx_radial_slider_angle_set
- gx_radial_slider_animation_set
- gx_radial_slider_animation_start
- gx_radial_slider_create
- gx_radial_slider_draw
- gx_radial_slider_info_get
- gx_radial_slider_info_set
- gx_radial_slider_pixelmap_set

## <a name="gx_radial_slider_info_get"></a>gx_radial_slider_info_get


Radyal kaydırıcı bilgilerini al

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_slider_info_get(
    GX_RADIAL_SLIDER *slider,
    GX_RADIAL_SLIDER_INFO **info);
```

### <a name="description"></a>Açıklama

Bu hizmet radyal kaydırıcı bilgisi işaretçisini alır.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu işaretçisi
- **bilgi** Radyal kaydırıcı bilgi işaretçisi alındı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal kaydırıcı bilgisi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RADIAL_SLIDER_INFO *info;

/* Retrive radial slider information structure. */
status = gx_radial_slider_info_get(&my_radial_slider,
                                    “my_radial_slider”, &info);

/* If status is GX_SUCCESS the radial slider information pointer of “my_radial_slider” has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_anchor_angles_set
- gx_radial_slider_angle_set
- gx_radial_slider_animation_set
- gx_radial_slider_animation_start
- gx_radial_slider_create
- gx_radial_slider_draw
- gx_radial_slider_event_process
- gx_radial_slider_info_set
- gx_radial_slider_pixelmap_set

## <a name="gx_radial_slider_info_set"></a>gx_radial_slider_info_set


Radyal kaydırıcı bilgilerini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_slider_info_set(
    GX_RADIAL_SLIDER *slider,
    GX_RADIAL_SLIDER_INFO *info);
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal kaydırıcı bilgilerini ayarlar.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu işaretçisi
- **bilgi** Ayarlanacak radyal kaydırıcı bilgileri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal kaydırıcı bilgi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RADIAL_SLIDER_INFO info;

/* Distance from left side of widget to rotating center. */
info.gx_radial_slider_info_xcenter = 100;

/* Distance from top size of widget to rotating center. */
info.gx_radial_slider_info_ycenter = 100;

/* Radius of rotating circle. */
info.gx_radial_slider_info_radius = 100;

/* Widget of rotating track. */
info.gx_radial_slider_info_track_width = 40;

/* Current angle value. */
info.gx_radial_slider_info_current_angle = 0;

/* Minimum angle value. */
info.gx_radial_slider_min_anlge = -60;

/* Maximum angle value. */
info.gx_radial_slider_max_angle = 240;

/* Anchor value list. */
info.gx_radial_slider_angle_list = GX_NULL;

/* Anchor value count. */
info.gx_radial_slider_list_count = 0;

/* Resource ID of background pixelmap. */
info.gx_radial_slider_background_pixelmap = GX_PIXELMAP_ID_BKGRD;

/* Resource ID of needle pixelmap. */
info.gx_radial_slider_needle_pixelmap = GX_PIXELMAP_ID_NEEDLE;

/* Reset radial slider info for “my_radial_slider”. */
status = gx_radial_slider_info_set(&my_radial_slider, &info);

/* If status is GX_SUCCESS the radial slider info of “my_radial_slider” has been reset. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_anchor_angles_set
- gx_radial_slider_angle_set
- gx_radial_slider_animation_set
- gx_radial_slider_animation_start
- gx_radial_slider_create
- gx_radial_slider_draw
- gx_radial_slider_event_process
- gx_radial_slider_info_get
- gx_radial_slider_pixelmap_set

## <a name="gx_radial_slider_pixelmap_set"></a>gx_radial_slider_pixelmap_set


Radyal kaydırıcı pixelmaps ayarlayın

### <a name="prototype"></a>Prototype

```C
UINT gx_radial_slider_pixelmap_set(
    GX_RADIAL_SLIDER *slider,
    GX_RESOURCE_ID background_pixemap,
    GX_REOUSRCE_ID needle_pixelmap);
```

### <a name="description"></a>Açıklama

Bu hizmet, radyal kaydırıcı arka planını ve iğne pixelmaps 'ı ayarlar.

### <a name="parameters"></a>Parametreler

- **kaydırıcı** Radyal kaydırıcı denetim bloğu işaretçisi
- **background_pixelmap** Arka plan pixelmap kaynak KIMLIĞI
- **needle_pixelmap** İğne pixelmap kaynak KIMLIĞI

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı radyal kaydırıcı pixelmap kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create “my_radio_button”. */
status = gx_radial_slider_pixelmap_set(&my_radial_slider, GX_PIXELMAP_ID_BG, GX_PIXELMAP_ID_NEEDLE);

/* If status is GX_SUCCESS the background and needle pixelmap of “my_radial_slider” has been reset. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_radial_slider_anchor_angles_set
- gx_radial_slider_angle_set
- gx_radial_slider_animation_set
- gx_radial_slider_animation_start
- gx_radial_slider_create
- gx_radial_slider_draw
- gx_radial_slider_event_process
- gx_radial_slider_info_get
- gx_radial_slider_info_set

## <a name="gx_rich_text_view_create"></a>gx_rich_text_view_create

Zengin metin görünümü oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_rich_text_view_create(
    GX_RICH_TEXT_VIEW *text_view,
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_RESOURCE_ID text_id,
    GX_RICH_TEXT_FONTS *fonts,
    USHORT id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen şekilde zengin metin görünümü oluşturur.


**Biçimlendirme etiketleri metin için özel türleri göstermek için kullanılır:**

- **\<b>\</b>** Metin yazı tipini Kullanıcı tarafından belirtilen kalın yazı tipi kimliğiyle ayarla
- **\<i>\</i>** Metin yazı tipini Kullanıcı tarafından belirtilen italik yazı tipi kimliğiyle ayarla
- **\<u>\</u>** Metnin altını çizmeyi etkinleştir
- **\<f GX_FONT_ID>\</f>** Metin yazı tipini belirtilen yazı tipi kimliğiyle ayarla
- **\<c GX_COLOR_ID>\</c>** Metin yazı tipini belirtilen renk kimliğiyle ayarla
- **\<hc GX_COLOR_ID>\</hc>** Metin vurgulama rengini belirtilen renk kimliğini ayarla
- **\<align left/right/center>\</align>** Metin hizalamasını ayarla

**Biçimlendirme etiketi kullanımı örnekleri:**

- \<b>Bu,< \b metin>
- \<i>Bu,< \i> italik metindir
- \<u>Bu metin< \u> altı çizili
- \<f 0>Bu metin yazı tipi kimliği 0< \f olarak ayarlanmıştır>
- \<c 1>Bu metin rengi kimliği 1< \C olarak ayarlanmıştır>
- \<hc 2>Bu metin vurgu rengi kimliği 2< \hc olarak ayarlanmıştır>
- \<align left> Bu metin, \ align< sola hizalı>

### <a name="parameters"></a>Parametreler

- **text_view** Zengin metin görünümü denetim bloğu işaretçisi
- **ad** Zengin metin görünümünün adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **text_id** Metin dizesinin kaynak KIMLIĞI
- **yazı tipleri** Zengin metin görünümü yazı tipi bilgilerine yönelik işaretçi. **Apbitix** , GX_RICH_TEXT_FONTS yapısına yönelik tanımı içerir.
- **Stil** Pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- zengin metin görünümünün **kimlik** uygulama tanımlı kimliği
- **Boyut** Zengin metin görünümü boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı zengin metin görünümü oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RICH_TEXT_VIEW rich_view;
GX_RCIH_TEXT_FONTS fonts;
GX_RECTANGLE size;

/* Defined widget size. */
gx_utility_rectangle_define(&size, 100, 100, 300, 150);

/* Define font information. */
fonts.gx_rich_text_fonts_normal_id = GX_FONT_ID_SYSTEM;
fonts.gx_rich_text_fonts_bold_id = GX_FONT_ID_SYSTEM;
fonts.gx_rich_text_fonts_italic_id = GX_FONT_ID_SYSTEM;
fonts.gx_rich_text_fonts_bold_italic_id = GX_FONT_ID_SYSTEM;

/* Create rich text view widget. */
status = gx_rich_text_view_create(&rich_view, “my_rich_view”,
                                  parent, GX_STRING_ID_TEST_STRING,
                                  &fonts,
                                  GX_STYLE_ENABLED,
                                  MY_RICH_VIEW_ID, &size);

/* If status is GX_SUCCESS the rich text view was successfully created. */

```

GUX Studio yüklemesinin bir parçası olarak sağlanan demo uygulaması demo_guix_widget_types, zengin metin görünümü pencere öğesini kullanma hakkında ayrıntılı bir örnek sağlar.

### <a name="see-also"></a>Ayrıca Bkz.

- gx_rich_text_view_draw
- gx_rich_text_view_fonts_set
- gx_rich_text_view_text_draw

## <a name="gx_rich_text_view_draw"></a>gx_rich_text_view_draw


Zengin metin görünümü çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_rich_text_view_draw(GX_RICH_TEXT_VIEW *text_view);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen zengin metin görünümü pencere öğesini çizer. Bu hizmet, genellikle bir tuval yenileme işleminin parçası olarak Gux tarafından dahili olarak çağrılır, ancak özel bir çizim işlevi sağlamak ve varsayılan zengin metin görünümü çizimini özel çizim temeli olarak çağırmak isteyebileceğiniz uygulamaya de sunulur.

### <a name="parameters"></a>Parametreler

- **text_view** Zengin metin görünümü pencere öğesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom rich text view drawing function. */

VOID my_rich_text_view_draw(GX_RICH_TEXT_VIEW *text_view)
{
    /* Call default rich text view draw. */
    gx_rich_text_view_draw(text_view);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_rich_text_view_create
- gx_rich_text_view_fonts_set
- gx_rich_text_view_text_draw

## <a name="gx_rich_text_view_fonts_set"></a>gx_rich_text_view_fonts_set

Zengin metin görünümü yazı tiplerini ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_rich_text_view_fonts_set(GX_RICH_TEXT_VIEW *text_view, GX_RICH_TEXT_FONTS *fonts);
```

### <a name="description"></a>Açıklama

Bu hizmet bir zengin metin görünümü pencere öğesinin yazı tiplerini ayarlar.

### <a name="parameters"></a>Parametreler

- **text_view** Zengin metin görünümü pencere öğesi denetim bloğu işaretçisi
- **yazı tipleri** Zengin metin görünümü yazı tipi bilgilerine yönelik işaretçi. **Apbitix I** GX_RICH_TEXT_FONTS yapısına yönelik tanımlar içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı zengin metin görünümü yazı tipi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RICH_TEXT_FONTS fonts;

/* Replace the font ids as needed. */
fonts.gx_rich_text_fonts_normal_id = GX_FONT_ID_SYSTEM;
fonts.gx_rich_text_fonts_bold_id = GX_FONT_ID_SYSTEM;
fonts.gx_rich_text_fonts_italic_id = GX_FONT_ID_SYSTEM;
fonts.gx_rich_text_fonts_bold_italic_id = GX_FONT_ID_SYSTEM;

/* Set the font of “my_rich_view”. */
status = gx_rich_text_view_fonts_set(&my_rich_view, &fonts);

/* If status is GX_SUCCESS the font for rich text view “my_rich_view” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_rich_text_view_create
- gx_rich_text_view_draw
- gx_rich_text_view_text_draw

## <a name="gx_rich_text_view_text_draw"></a>gx_rich_text_view_text_draw


Zengin metin görünümü metni çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_rich_text_view_text_draw(GX_RICH_TEXT_VIEW *text_view);
```

### <a name="description"></a>Açıklama

Bu destek işlevi bir zengin metin görünümünün metin bölümünü çizer. Bu işlev, gx_rich_text_view_draw () tarafından dahili olarak çağrılır ve özel bir zengin metin görünümü çizim işlevi tanımlayan uygulamalar için kolaylık olarak ayrı bir API olarak sağlanır. Zengin metin görünümü arka plan çizimini özelleştirmek isteyen uygulamalar özel çizim işlevlerini sağlayabilir ve zengin metin görünümü metnini arka plan üzerine çizmek için gx_rich_text_view_text_draw hizmetini özel çiziminin bir parçası olarak çağırabilir.

### <a name="parameters"></a>Parametreler

- **text_view** Zengin metin görünümü pencere öğesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom rich text view drawing function. */

VOID my_rich_text_view_draw(GX_RICH_TEXT_VIEW *text_view)
{
    /* Insert code here to draw rich text view background. */

    /* Call support function to do text drawing. */
    gx_rich_text_view_text_draw();

    /* Draw child widgets. */
    gx_widget_children_draw((GX_WIDGET *) rich_text_view);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_rich_text_view_create
- gx_rich_text_view_draw
- gx_rich_text_view_fonts_set

## <a name="gx_screen_stack_create"></a>gx_screen_stack_create


Ekran yığını başlatma

### <a name="prototype"></a>Prototype

```C
UINT gx_screen_stack_create(
    GX_SCREEN_STACK_CONTROL *control,
    GX_WIDGET **memory_buffer, 
    INT buffer_size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir ekran yığınını başlatır. Uygulamanın, ekran yığını özelliğini uygulamak için kullanılan bellek bloğunu ve arabellek boyutunu tanımlamanız gerekir.

> [!NOTE]
> *Bu API kullanım dışı bırakılmış ve gx_system_screen_stack_create () ile değiştirilmiştir. Bu sürüm yalnızca önceki kitaplık sürümleriyle geriye dönük uyumluluk için sağlanır.*

### <a name="parameters"></a>Parametreler

- **Denetim** Ekran yığını denetim bloğu
- **memory_buffer** Ekran yığını olarak kullanılan bir bellek arabelleği işaretçisi
- **Buffer_size** Bayt cinsinden bellek boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ekran yığını oluşturma
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE** (0x22) geçersiz arabellek boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
#define SCREEN_STACK_SIZE 10

GX_SCREEN_STACK_CONTROL my_stack_control;
GX_WIDGET *screen_stack[SCREEN_STACK_SIZE];

/* Initialize “my_stack_control”. */
status = gx_screen_stack_create(&my_stack_control, screen_stack,
                        SCREEN_STACK_SIZE * sizeof(GX_WIDGET *));

/* If status is GX_SUCCESS the screen control block “my_stack control” has been initialized. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_screen_stack_push
- gx_screen_stack_pop
- gx_screen_stack_reset

## <a name="gx_screen_stack_pop"></a>gx_screen_stack_pop


Ekran yığınından en üstteki girişi kaldırma

### <a name="prototype"></a>Prototype

```C
UINT gx_screen_stack_pop(GX_SCREEN_STACK_CONTROL *control);
```

### <a name="description"></a>Açıklama

Bu hizmet, ekran yığınından en üstteki girişi kaldırır ve önceki üst öğesine açılan ekranı ekler. Bu API aynı zamanda var olan alt öğeleri üst öğeden ayırır.

> [!NOTE]
> *Bu API kullanım dışı bırakılmış ve gx_system_screen_stack_pop () ile değiştirilmiştir. Bu sürüm yalnızca önceki kitaplık sürümleriyle geriye dönük uyumluluk için sağlanır.*

### <a name="parameters"></a>Parametreler

- **Denetim** Ekran yığını denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ekran yığını açılan kutusu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Remove the topmost entry from the screen stack. */
status = gx_screen_stack_pop(&my_stack_control);

/* If status is GX_SUCCESS the topmost entry has been removed from the screen stack, 
    and the popped screen has been attached to its parent. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_screen_stack_create
- gx_screen_stack_push
- gx_screen_stack_reset

## <a name="gx_screen_stack_push"></a>gx_screen_stack_push


Gönder ekranı ve üst öğeleri yığına

### <a name="prototype"></a>Prototype

```C
UINT gx_screen_stack_push(
    GX_SCREEN_STACK_CONTROL *control,
    GX_WIDGET *screen,
    GX_WIDGET *new_screen);
```

### <a name="description"></a>Açıklama

Bu hizmet ekranı üst öğesinden ayırır ve ekran işaretçisini ve üst işaretçiyi ekran yığınına iter. Yeni ekran işaretçisi daha sonra üst öğeye eklenir.


> [!NOTE]
> *Bu API kullanım dışı bırakılmış ve gx_system_screen_stack_pop () ile değiştirilmiştir. Bu sürüm yalnızca önceki kitaplık sürümleriyle geriye dönük uyumluluk için sağlanır.*

### <a name="parameters"></a>Parametreler

- **Denetim** Ekran yığını denetim bloğu
- **ekran** Gönderim için ekran işaretçisi
- **new_screen** Yeni ekranın işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ekran yığını gönderimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Push “screen” and its parent to screen stack, Dettach “screen” from its parent, and attach “new screen” to the parent. */
status = gx_screen_stack_push(&my_stack_control,
                                screen, new_screen);

/* If status is GX_SUCCESS the widget “screen” and its parent have been pushed to screen stack, “screen” has been detached from its parent, “new_screen” has been attached to the parent. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_screen_stack_create
- gx_screen_stack_push
- gx_screen_stack_reset

## <a name="gx_screen_stack_reset"></a>gx_screen_stack_reset


Tüm girişleri ekran yığınından kaldırır

### <a name="prototype"></a>Prototype

```C
UINT gx_screen_stack_reset(GX_SCREEN_STACK_CONTROL *control);
```

### <a name="description"></a>Açıklama

Bu hizmet, tüm girişleri ekran yığınından kaldırır.

> [!NOTE]
> *Bu API kullanım dışı bırakılmış ve gx_system_screen_stack_pop () ile değiştirilmiştir. Bu sürüm yalnızca önceki kitaplık sürümleriyle geriye dönük uyumluluk için sağlanır.*

### <a name="parameters"></a>Parametreler

- **Denetim** Ekran yığını denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı kaydırma parmak izi oluştur
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Remove all enteries from the screen stack. */
status = gx_screen_stack_reset(&my_stack_control);

/* If status is GX_SUCCESS all entries of screen stack has been removed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_screen_stack_create
- gx_screen_stack_push
- gx_screen_stack_pop

## <a name="gx_scroll_thumb_create"></a>gx_scroll_thumb_create


Kaydırma parmak izi oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_thumb_create(
    GX_SCROLL_THUMB *scroll_thumb,
    GX_SCROLLBAR *parent, ULONG style);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir kaydırma Parmak tekerleği oluşturur. Bu hizmet, genellikle GX_SCROLLBAR oluşturulduğunda dahili olarak çağrılır, ancak özel kaydırma çubuğu uygulamalarına izin vermek için genel hale getirilir.

### <a name="parameters"></a>Parametreler

- **scroll_thumb** Kaydırma kutusu pencere öğesi denetim bloğu
- **üst öğe** Üst kaydırma çubuğu işaretçisi
- **Stil** ScrollBar pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı kaydırma parmak izi oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET** (0x12) üst pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_SCROLL_THUMB my_scroll_thumb;

/* Create scroll thumb “my_scroll_thumb”. */
status = gx_scroll_thumb_create(&my_scroll_thumb, &my_scrollbar,
                                GX_STYLE_NONE);

/* If status is GX_SUCCESS the scroll thumb “my_scroll_thumb” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_scroll_thumb_draw
- gx_scroll_thumb_event_process

## <a name="gx_scroll_thumb_draw"></a>gx_scroll_thumb_draw


Kaydırma parmak izi çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_scroll_thumb_draw(GX_SCROLL_THUMB *scroll_thumb);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir kaydırma Parmak tekerleği çizer. Bu hizmet, Gux tuvali yenilemesi tarafından dahili olarak çağrılır, ancak geçersiz kılınan çizim işlevleri tarafından çağrılabilir.

### <a name="parameters"></a>Parametreler

- **scroll_thumb** Kaydırma kutusu pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom scroll thumb drawing function. */

VOID my_scroll_thumb_draw(GX_SCROLL_THUMB *thumb)
{
    /* Call default scroll thumb draw. */
    gx_scroll_thumb_draw(thumb);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_scroll_thumb_create
- gx_scroll_thumb_event_process

## <a name="gx_scroll_thumb_event_process"></a>gx_scroll_thumb_event_process


İşlem kaydırma parmak izi olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_thumb_event_process(
    GX_SCROLL_THUMB *scroll_thumb,
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir ScrollBar parmak tekerinin gönderdiği olayları işler. Bu hizmet normalde Gux tarafından dahili olarak kullanılır, ancak özel kaydırma çubuğu davranışları uygulamaya yardımcı olmak için genel kullanıma açıktır.

### <a name="parameters"></a>Parametreler

- **scroll_thumb** Kaydırma kutusu pencere öğesi denetim bloğu
- **olay** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı kaydırma parmak izi olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom event processing function. */

UINT my_event_process (GX_SCROLL_THUMB *thumb, GX_EVENT *event_ptr)
{
    switch(event_ptr->gx_event_type)
    {
    case GX_EVENT_SHOW:
        /* Do default handling. */
        status = gx_scroll_thumb_event_process(thumb, event_ptr);

        /* add my own handling here */
        break;
    default:
        status = gx_scroll_thumb_event_process(thumb, event_ptr);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_scroll_thumb_create
- gx_scroll_thumb_draw

## <a name="gx_scroll_wheel_create"></a>gx_scroll_wheel_create


Temel kaydırma tekerleği oluşturma pencere öğesi

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_wheel_create( 
    GX_SCROLL_WHEEL *wheel, 
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    INT total_rows, 
    ULONG style,
    USHORT id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet, genel bir kaydırma tekerleği pencere öğesi oluşturur.

Genel bir kaydırma tekerleği, *gx_numeric_scroll_wheel** * ve *gx_string_ scroll_wheel** * pencere öğeleri için temel olan *gx_text_scroll_wheel** * dahil olmak üzere tüm kaydırma tekerleği pencere öğesi türlerinin temel pencere öğesi. Taban kaydırma tekerleği pencere öğesi, tüm kaydırma tekerleği pencere öğesi türleri için olay işleme, kayan animasyon ve seçilen satır hesaplamasını sağlar.

Bu pencere öğesi türü çizim işlevi sunmadığından, uygulamalar Normalde genel bir kaydırma tekerleği pencere öğesinin bir örneğini oluşturmamalıdır. Ancak, özel bir kaydırma tekerleği pencere öğesi türü oluşturması gereken uygulamalara yardımcı olmak için bu API 'ye erişim sağlanır.

GX_SCROLL_WHEEL GX_WINDOW tabanlıdır ve bu nedenle tüm GX_WINDOW API 'Leri GX_SCROLL_WHEEL türetilen GX_SCROLL_WHEEL ve pencere öğeleri ile kullanılabilir.

### <a name="parameters"></a>Parametreler

- **tekerlek** Genel kaydırma tekerleği denetim bloğu işaretçisi
- **ad** Uygulama tarafından atanan pencere öğesi adı
- **üst öğe** Üst pencere öğesi veya GX_NULL
- **total_rows** Toplam kullanılabilir satır
- **Stil** Pencere öğesi stil bayrakları
- **kimlik** uygulama tarafından atanan pencere öğesi kimliği
- **Boyut** İlk pencere öğesi boyutunu tanımlayan dikdörtgen.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) kaydırma tekerleği başarıyla oluşturuldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_SIZE** (0x19) geçersiz denetim bloğu boyutu
- **GX_ALREADY_CREATED** (0x13) pencere öğesi oluşturuldu
- **GX_INVALID_WIDGET** (0x12) üst pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic create function during custom widget createl. */

UINT custom_scroll_wheel_create(CUSTOM_SCROLL_WHEEL *wheel,
                    GX_CONST GX_CHAR *name,
                    GX_WIDGET *parent,
                    INT total_rows, ULONG style,
                    USHORT id,
                    GX_CONST GX_RECTANGLE *size)
{
    /* create base widget as part of custom create */
    status = gx_scroll_wheel_create(wheel, name, parent,
                            total_rows, style, id, size);

    /* If status is GX_SUCCESS the base scroll wheel has been created. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_speed_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_scroll_wheel_event_process"></a>gx_scroll_wheel_event_process


Genel kaydırma tekerleği pencere öğesi için olay işleme işlevi

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_wheel_event_process(
    GX_SCROLL_WHEEL *wheel,
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet, tüm kaydırma tekerleği pencere öğesi türleri için temel giriş olay işlemesini sağlar.

Bu işlev, özel bir kaydırma tekerleği pencere öğesi türü oluşturması gereken uygulamalarla yardım etmek için uygulama yazılımına sunulur. Uygulamalar genellikle kendi olay işleme işlevini sağlar, ancak özelleştirme gerektirmeyen olaylar için, tekerlek pencere öğeleri için genel olay işlemeyi çağırır.

### <a name="parameters"></a>Parametreler

- **tekerlek** Genel kaydırma tekerleği denetim bloğu işaretçisi
- **olay** GX_EVENT işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) tekerlek olay işlemini başarıyla kaydır
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic scroll wheel event processing 
    as part of custom event processing function. */

UINT custom_scroll_wheel_event_process(CUSTOM_SCROLL_WHEEL *wheel,
                    GX_EVENT *event)
{
    switch(event->gx_event_type)
    {
    case xyz:
        /* insert custom event handling here */
        break;

    default:
        /* pass all other events to the generic scroll wheel
            event processing */
        gx_scroll_wheel_event_process(wheel, event);
        break;
    }
}
```


### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_speed_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_scroll_wheel_gradient_alpha_set"></a>gx_scroll_wheel_gradient_alpha_set


İsteğe bağlı kaplama gradyanı için gradyan alfa değerleri atama

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_wheel_gradient_alpha_set(
    GX_SCROLL_WHEEL *wheel,
    GX_UBYTE start_alpha,
    GX_UBYTE end_alpha);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırma tekerleği pencere öğesinin isteğe bağlı gradyan kaplaması için başlangıç ve bitiş Alfa değerlerini tanımlar.

Tüm kaydırma tekerleği pencere öğeleri, kaydırma tekerleği pencere öğesinin üst ve alt kenarının yakınında bulunan satırlar olarak kaydırma tekerleği satırlarının "belirme" efektini destekler. Bu geçişli efekt, kaydırma tekerleği satırları üzerinde bir gradyan pixelmap çizerek, satırlar, kaydırma tekerleği pencere öğesinin üst ve alt kısmına yakın bir şekilde çizilerek satırları soluklaştırmak üzere çizerek gerçekleştirilir.

Bu API hizmeti, uygulamanın Soldurma efektinin yoğunluğunu değiştirmesine izin verir veya başlangıç ve bitiş Alfa değerlerini 0 olarak ayarlayarak bu etkiyi tamamen devre dışı bırakır.

Gradyan pixelmap, kaydırma tekerleği başlangıçta görünür hale geldiğinde çalışma zamanında oluşturulur. Bunun için _gx_system_memory_allocator_set () kullanılarak bir çalışma zamanı bellek ayırma hizmeti tanımlanmış olması gerekir. Hiç bellek ayırıcı işlevi tanımlanmamışsa, gradyan görüntü oluşturulmaz ve bir azalma efekti kullanılabilir olmaz.

### <a name="parameters"></a>Parametreler

- **tekerlek** Genel kaydırma tekerleği denetim bloğu işaretçisi
- **start_alpha** Kaplama gradyanı başlayan alfa değeri.
- **end_alpha** Kaplama gradyanı bitiş alfa değeri.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) kaydırma tekerleği gradyan Alpha 'ı başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
status = gx_scroll_wheel_gradient_alpha_set(&wheel, 240, 0);
/* if status == GX_SUCCESS the wheel gradient alpha values were
Successfully assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_speed_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_scroll_wheel_row_height_set"></a>gx_scroll_wheel_row_height_set


Her bir tekerlek satırı için satır yüksekliğini ata

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_wheel_row_height_set(
    GX_SCROLL_WHEEL *wheel,
    GX_VALUE row_height);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırma tekerleğinin her bir satırı için satır yüksekliğini atar. Kaydırma tekerleğinin stil GX_STYLE_TEXT_SCROLL_WHEEL_ROUND varsa, satır yüksekliği, ekranın üst veya alt kenarına yaklaştığında satır yüksekliğini etkin bir şekilde azaltacak bir dönüşümden geçer.

### <a name="parameters"></a>Parametreler

- **tekerlek** Genel kaydırma tekerleği denetim bloğu işaretçisi
- **row_height** Piksel cinsinden satır yüksekliği değeri.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) kaydırma tekerleği yüksekliğini başarıyla ayarla
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
status = gx_scroll_wheel_row_height_set(&wheel, 40);

/* if status == GX_SUCCESS the wheel row height has been set to 40
pixels. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_gradient_alpha_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_speed_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_scroll_wheel_selected_background_set"></a>gx_scroll_wheel_selected_background_set


Tekerlek seçili satırı için arka plan görüntüsü ata

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_wheel_selected_background_set(
    GX_SCROLL_WHEEL*wheel, 
    GX_RESOURCE_ID image_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırma tekerleğinin seçili satırının arkasında çizilen isteğe bağlı bir pixelmap KIMLIĞI atar. Bu, kullanıcının kaydırma tekerleğinin hangi satırının seçili olduğunu kolayca ayırabilmesi için seçili satırı vurgulamak üzere kullanılabilir.

### <a name="parameters"></a>Parametreler

- **tekerlek** Genel kaydırma tekerleği denetim bloğu işaretçisi
- **image_id** Seçilen satır arka plan görüntüsü olarak kullanılacak pixelmap KIMLIĞI.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) kaydırma tekerleği arka planını başarıyla ayarlama
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
status = gx_scroll_wheel_selected_background_set(&wheel,
GX_PIXELMAP_ID_SELECTED_ROW);

/* if status == GX_SUCCESS the background image has been
assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_speed_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_scroll_wheel_selected_get"></a>gx_scroll_wheel_selected_get


Şu anda seçili olan tekerlek satırını al

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_wheel_selected_get(
    GX_SCROLL_WHEEL *wheel,
    INT *row);
```

### <a name="description"></a>Açıklama

Bu hizmet, şu anda seçili olan satırı almak için kaydırma tekerleğini sorgular. Çağıran, seçilen satır dizinini bu işleve ikinci parametre olarak döndürmek için konumu geçmelidir.

### <a name="parameters"></a>Parametreler

- **tekerlek** Genel kaydırma tekerleği denetim bloğu işaretçisi
- **satır** Seçili satır değerinin döndürüleceği konum.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) seçili tekerlek satırı başarıyla alındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x19) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
INT row;
status = gx_scroll_wheel_selected_get(&wheel, &row);

/* if status == GX_SUCCESS the selected row has been returned in
the row variable. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_speed_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_scroll_wheel_selected_set"></a>gx_scroll_wheel_selected_set


Seçili kaydırma tekerleği satırını ata

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_wheel_selected_set(
    GX_SCROLL_WHEEL *wheel,
    INT row);
```

### <a name="description"></a>Açıklama

Bu hizmet şu anda seçili olan kaydırma tekerleği satırını atar.

### <a name="parameters"></a>Parametreler

- **tekerlek** Genel kaydırma tekerleği denetim bloğu işaretçisi
- **satır** Seçilecek kaydırma tekerleğinin satırı.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) seçili tekerlek satırını başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
status = gx_scroll_wheel_selected_set(&wheel, 20);

/* if status == GX_SUCCESS the scroll wheel has been set to select
row 20 */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_speed_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_scroll_wheel_speed_set"></a>gx_scroll_wheel_speed_set


Kaydırma hızı ata

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_wheel_speed_set(
    GX_SCROLL_WHEEL *wheel,
    GX_FIXED_VAL start_speed_rate,
    GX_FIXED_VAL end_speed_rate,
    GX_VALUE max_steps,
    GX_VALUE delay);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırma tekerleği pencere öğesi için kaydırma hızını atar.

### <a name="parameters"></a>Parametreler

- **tekerlek** Genel kaydırma tekerleği denetim bloğu işaretçisi
- **start_speed_rate** Hızlı hareket hızını kaydırma hızı.
- **end_speed_rate** Hareket hızına yönelik kaydırma bitiş hızı oranı
- **max_steps** Kaydırma için en fazla adım.
- **gecikme** Her adımın gecikme süresi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) tekerlek hızını başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) geçersiz değer

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
status = gx_scroll_wheel_speed_set(&wheel, GX_FIXED_VAL_MAKE(2),
                                GX_FIXED_VAL_MAKE(1) / 2, 10, 2);

/* if status == GX_SUCCESS the scroll wheel speed has been
successfully set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_scroll_wheel_total_rows_set"></a>gx_scroll_wheel_total_rows_set


Kullanılabilir toplam kaydırma tekerleği satırını ata

### <a name="prototype"></a>Prototype

```C
UINT gx_scroll_wheel_total_rows_set(
    GX_SCROLL_WHEEL *wheel,
    INT total_rows);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen kaydırma tekerleğindeki kullanılabilir satır sayısını atar. Kaydırma tekerleği pencere öğesi genellikle, bir dize dizisi veya Kullanıcı tarafından sağlanan dize verileri biçiminde uygulamadan alınan satır içeriğini alır. Bu API, kullanıcıya sunulması gereken toplam satır sayısının kaydırma tekerleğini bilgilendirir.

### <a name="parameters"></a>Parametreler

- **tekerlek** Genel kaydırma tekerleği denetim bloğu işaretçisi
- **total_rows** Kullanıcıya sunmak için toplam tekerlek satırı sayısı.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) kaydırma tekerleği toplam satırını başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) geçersiz değer

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
status = gx_scroll_wheel_total_rows_set(&wheel, 100);

/* if status == GX_SUCCESS the scroll wheel has been changed to
display 100 total rows */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_speed_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_text_get

## <a name="gx_scrollbar_draw"></a>gx_scrollbar_draw


Kaydırma çubuğu çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_scrollbar_draw(GX_SCROLLBAR *scrollbar);
```

### <a name="description"></a>Açıklama

Bu hizmet bir kaydırma çubuğu çizer. Genellikle dikey ve yatay kaydırma çubuğu pencere öğeleri için ortak bir çizim işlevi kullanılır. Bu hizmet, Gux tuvali yenilemesi tarafından dahili olarak çağrılır, ancak geçersiz kılınan çizim işlevleri tarafından çağrılabilir.

### <a name="parameters"></a>Parametreler

- **kaydırma çubuğu** Çizilecek ScrollBar pencere öğesi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom scrollbar drawing function. */

VOID my_scrollbar_draw(GX_SCROLLBAR *scrollbar)
{
    /* Call default scrollbar draw. */
    gx_scrollbar_draw(thumb);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_ horizontal_scrollbar_create
- gx_scrollbar_event_process
- gx_scrollbar_limit_check
- gx_scrollbar_reset
- gx_vertical_scrollbar_create

## <a name="gx_scrollbar_event_process"></a>gx_scrollbar_event_process


İşlem kaydırma çubuğu olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_scrollbar_event_process(
    GX_SCROLLBAR *scrollbar,
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet bir ScrollBar olayını işler. Hem dikey hem de yatay kaydırma çubuğu öğeleri için kullanılan ortak bir olay işleme işlevi.

### <a name="parameters"></a>Parametreler

- **kaydırma çubuğu** ScrollBar pencere öğesi denetim bloğu
- **olay** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı kaydırma çubuğu olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
Call generic scrollbar event processing as part of custom event processing function. */

UINT custom_scrollbar_event_process(GX_SCROLLBAR *scrollbar,
                                    GX_EVENT *event)
{
    switch(event->gx_event_type)
    {
    case xyz:
        /* insert custom event handling here */
        break;
    default:
        /* pass all other events to the generic scrollbar
            event processing */
        gx_scrollbar_event_process(scrollbar, event);
        break;
    }
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_ horizontal_scrollbar_create
- gx_scrollbar_draw
- gx_scrollbar_limit_check
- gx_scrollbar_reset
- gx_vertical_scrollbar_create

## <a name="gx_scrollbar_limit_check"></a>gx_scrollbar_limit_check


Kaydırma çubuğu sınırını denetle

### <a name="prototype"></a>Prototype

```C
UINT gx_scrollbar_limit_check(GX_SCROLLBAR *scrollbar);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırma çubuğunun sınırını denetler ve ScrollBar parmak tekerinin önceden tanımlanmış sınırların ötesinde hareket etmesini engeller.

### <a name="parameters"></a>Parametreler

- **kaydırma çubuğu** ScrollBar pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı kaydırma çubuğu sınırı denetimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Check scrollbar limit of “my_scrollbar”. */
status = gx_scrollbar_limit_check(&my_scrollbar);

/* If status is GX_SUCCESS the limit of scrollbar “my_scrollbar” has been checked. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_scrollbar_create
- gx_scrollbar_draw
- gx_scrollbar_event_process
- gx_scrollbar_reset
- gx_vertical_scrollbar_create

## <a name="gx_scrollbar_reset"></a>gx_scrollbar_reset


Kaydırma çubuğunu Sıfırla

### <a name="prototype"></a>Prototype

```C
UINT gx_scrollbar_reset(
    GX_SCROLLBAR *scrollbar,
    GX_SCROLL_INFO *info);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırma çubuğunu sıfırlar.

### <a name="parameters"></a>Parametreler

- **kaydırma çubuğu** ScrollBar pencere öğesi denetim bloğu
- **bilgi** Kaydırma çubuğu sınırlarını, geçerli değeri ve adım veya artışı tanımlayan GX_SCROLL_INFO yapısına yönelik işaretçi. **Ek ı** GX_SCROLL_INFO yapısına yönelik tanımı içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı ScrollBar sıfırlaması
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) kaydırma bilgileri geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Reset scrollbar “my_scrollbar”. */

GX_SCROLL_INFO my_info;

my_info.gx_scroll_value = 0;
my_info.gx_scroll_minimum = 0;
my_info.gx_scroll_maximum = 100;
my_info.gx_scroll_visible = 10;
my_info.gx_scroll_increment = 1;

status = gx_scrollbar_reset(&my_scrollbar, &my_info);

/* If status is GX_SUCCESS the scrollbar “my_scrollbar” has been reset. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_scrollbar_create
- gx_scrollbar_draw
- gx_scrollbar_event_process
- gx_scrollbar_limit_check
- gx_vertical_scrollbar_create

## <a name="gx_scrollbar_value_set"></a>gx_scrollbar_value_set


Kaydırma çubuğu değeri ata

### <a name="prototype"></a>Prototype

```C
UINT gx_scrollbar_value_set(
    GX_SCROLLBAR *scrollbar,
    INT value);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli ScrollBar değerini atar. Ana pencereye bir GX_EVENT_VERTICAL_SCROLL veya GX_EVENT_HORIZONTAL_SCROLL olayı oluşturulacaktır.

### <a name="parameters"></a>Parametreler

- **kaydırma çubuğu** ScrollBar pencere öğesi denetim bloğu
- **değer** Yeni kaydırma çubuğu değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı kaydırma çubuğu olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) kaydırma değeri geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Assign new value for scrollbar “my_scrollbar”. */

status = gx_scrollbar_value_set(&my_scrollbar, 0);

/* If status is GX_SUCCESS the current position of scrollbar “my_scrollbar” has been set. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_scrollbar_create
- gx_scrollbar_draw
- gx_scrollbar_limit_check
- gx_scrollbar_reset
- gx_vertical_scrollbar_create

## <a name="gx_single_line_text_input_backspace"></a>gx_single_line_text_input_backspace


Metin girişi pencere öğesinde bir geri al karakteri işle

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_backspace(GX_SINGLE_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin girişi imleç konumundan önce karakteri siler. Bu hizmet, bir geri anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tek satırlık metin girişi oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x23) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Delete a character before the cursor of “my_text_input”. */
status = gx_single_line_text_input_backspace(&my_text_input);

/* If status is GX_SUCCESS the character before the cursor has been deleted. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_input_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_buffer_clear"></a>gx_single_line_text_input_buffer_clear


Metin girişi arabelleğindeki tüm karakterleri siler

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_buffer_clear(
    GX_SINGLE_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin girişi arabelleğindeki tüm karakterleri siler.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) tek satırlık metin girişi arabelleğini başarıyla temizledi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* clear input buffer of “my_text_input”. */
status = gx_single_line_text_input_clear(&my_text_input);

/* If status is GX_SUCCESS the text input widget has emptied its input buffer. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_buffer_backspace
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_input_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_buffer_get"></a>gx_single_line_text_input_buffer_get


Metin girişi pencere öğesinin arabellek bilgilerini alır

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_buffer_get(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    GX_CHAR **buffer_address, 
    UINT *content_size, 
    UINT *buffer_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin girişi pencere öğesinin arabellek bilgilerini alır.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu
- **buffer_address** Giriş arabelleğinin adresi
- **content_size** Giriş verilerinin bayt sayısı
- **Buffer_size** Giriş arabelleğinin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) arabellek bilgileri başarıyla alındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR *buffer_address;
UINT buffer_size;
UINT content_size;

/* Retrieve buffer information of “my_text_input” widget. */
status = gx_single_line_text_input_buffer_get(&my_text_input,
                    &buffer_address, &string_size, &buffer_size);

/* If status is GX_SUCCESS the value of buffer_address, string_size and buffer_size has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_character_delete"></a>gx_single_line_text_input_character_delete


Geçerli imleç konumundaki karakteri sil

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_character_delete(
    GX_SINGLE_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin girişi imleç konumundan sonra karakteri siler. Bu hizmet, bir DELETE anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) İmleçten sonra bir karakter başarıyla silindi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Delete the character after the cursor of “my_text_input”. */
status = gx_single_line_text_input_character_delete(&my_text_input);

/* If status is GX_SUCCESS the character after the cursor has been deleted. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_input_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_multi_line_text_input_create
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_character_insert"></a>gx_single_line_text_input_character_insert


Geçerli imleç konumuna bir karakter dizesi Ekle

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_character_insert(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    GX_UBYTE *insert_str,
    UINT insert_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli imleç konumundaki metin girişi dize arabelleğine bir karakter dizesi ekler.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu
- **insert_str** Eklenecek karakter dizesi
- **insert_size** Eklenecek bayt sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) karakteri başarıyla ekledi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Insert characters at current cursor position. */

GX_CHAR insert_text[10] = “insert”;
status = gx_single_line_text_input_character_insert(&my_text_input,
                                            insert_text,
                                            GX_STRLEN(insert_text));

/* If status is GX_SUCCESS the text input widget has successfully insert the string. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_input_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_create"></a>gx_single_line_text_input_create


Metin girişi pencere öğesi oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_create(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    GX_CONST GX_CHAR *name, GX_WIDGET *parent,
    GX_CHAR *input_buffer, UINT buffer_size,
    UINT style, USHORT text_input_id, GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir metin girişi pencere öğesi oluşturur. Çağıran, giriş dizesi için depolama alanı sağlamalıdır ve en fazla dize uzunluğunu belirtmelidir.

GX_SINGLE_LINE_TEXT_INPUT GX_PROMPT türetilir ve bu nedenle tüm gx_prompt Hizmetleri GX_SINGLE_LINE_TEXT_INPUT pencere öğeleri ile kullanılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu
- **ad** İsteğe bağlı pencere öğesi mantıksal adı
- **üst öğe** İsteğe bağlı üst pencere öğesi
- **input_buffer** Giriş dizesi için depolama
- **Buffer_size** Giriş dizesi depolama alanının bayt cinsinden boyutu.
- **Stil** Metin girişi stil bayrakları
- **text_input_id** Giriş pencere öğesinin isteğe bağlı KIMLIĞI
- **Boyut** İlk pencere öğesi boyutunu tanımlayan dikdörtgen

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tek satırlık metin girişi oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_SINGLE_LINE_TEXT_INPUT my_text_input;
static GX_CHAR           text_input_buffer[100];
GX_RECTANGLE             size;

/* Define widget size. */
gx_utility_rectangle_define(&size, 10, 10, 110, 40);

/* Create single-line text input widget “my_text_input”. */
status = gx_single_line_text_input_create(&my_text_input,
                        “text_input”, GX_NULL, text_input_buffer, 100,
                        GX_STYLE_ENABLED, 0, &size);

/* If status is GX_SUCCESS, the text input widget has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_draw"></a>gx_single_line_text_input_draw


Metin girişi pencere öğesi çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_single_line_text_input_draw(GX_SINGLE_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet bir metin girişi pencere öğesi çizer. Bu hizmet, genellikle tuval yenilemesi sırasında dahili olarak çağrılır, ancak özel metin girişi çizim işlevlerinden de çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom single line text input draw function. */

VOID my_sl_text_input_draw(GX_SINGLE_LINE_TEXT_INPUT *input)
{
    /* Call default single line text input draw. */
    gx_single_line_text_input_draw(input);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_draw_position_get"></a>gx_single_line_text_input_draw_position_get


Metin çizme başlangıç konumunu al

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_draw_position_get(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    GX_VALUE *xpos, GX_VALUE *ypos);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin giriş metninin çizim başlangıç konumunu alır.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu
- **XPos** X koordinatı içinde çizim başlangıç konumu alındı
- **yılkonumu** Y koordinatı içinde çizim başlangıç konumu alındı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin girişi imlecini başarıyla sona taşı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom single line text input draw function. */

VOID my_sl_text_input_draw(GX_SINGLE_LINE_TEXT_INPUT *input)
{
GX_VALUE xpos;
GX_VALUE ypos;

    /* Draw background. */
    gx_widget_border_draw(input, border_color, upper_fill_color,
                          lower_fill_color, GX_TRUE);

    /* Retrieve text draw start position. */
    gx_single_line_text_input_draw_position_get(input, xpos,
                                                ypos);

    /* Add your text drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_end"></a>gx_single_line_text_input_end


Metin girişi imlecini dize sonuna taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_end(GX_SINGLE_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, giriş dizesinin sonundaki metin girişi pencere öğesi imlecini konumlandırır. Bu hizmet, bir son anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin girişi imlecini başarıyla sona taşı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move input cursor to end. */
status = gx_single_line_text_input_end(&my_text_input);

/* If status is GX_SUCCESS, text text input cursor has been moved to end. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_event_process"></a>gx_single_line_text_input_event_process


Metin girişi pencere öğesi olay işleme işlevi

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_event_process(
    GX_SINGLE_LINE_TEXT_INPUT *text_input, 
    GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet tek satırlık bir metin girişi olayını işler. Bu işleve gx_single_line_text_input_create işlevi tarafından dahili olarak başvurulur, ancak uygulamanın özel bir tek satırlık metin girişi olay işleme işlevi tanımladığı durumlarda uygulama tarafından kullanıma sunulur.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu
- **event_ptr** GX_EVENT yapısına yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin girişi olayını başarıyla işledi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic single line text input event processing as part of custom event processing function. */

UINT custom_sl_text_input_event_process(
                                GX_SINGLE_LINE_TEXT_INPUT *input,
                                GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;
    default:
        /* Pass all other events to the default single line
            text input event processing */
        status =
        gx_single_line_text_input_event_process(input, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_fill_color_set"></a>gx_single_line_text_input_fill_color_set


Tek satırlık metin girişi arka plan rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_fill_color_set(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    GX_RESOURCE_ID normal_fill_color_id,
    GX_RESOURCE_ID selected_fill_color_id,
    GX_RESOURCE_ID disabled_fill_color_id,
    GX_RESOURCE_ID readonly_fill_color_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, tek satırlık metin girişinin Fill rengini ayarlar.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi denetim bloğu işaretçisi
- **normal_fill_color_id** Pencere öğesi dolgusunun normal durumundaki kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **selected_fill_color_id** Pencere öğesi odaklanıldığında pencere öğesi dolgusu dolgusunun kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **disabled_fill_color_id** Stil GX_STYLE_ENABLED ayarlanmamışsa pencere öğesi dolgusunun kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **readonly_fill_color_id** Stil GX_STYLE_ENABLED ve GX_STYLE_TEXT_INPUT_READYONLY her ikisi de ayarlandığında pencere öğesi dolgusu rengi kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tek satırlık metin girişi dolgusu renk kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set fill colors for single line text input “my_text_input”. */
status = gx_single_line_text_input_fill_color_set(&my_text_input,
                    GX_COLOR_ID_NORMAL_FILL,
                    GX_COLOR_ID_SELECTED_FILL,
                    GX_COLOR_ID_DISABLED_FILL,
                    GX_COLOR_ID_READONLY_FILL);

/* If status is GX_SUCCESS, the fill color of “my_text_input” was
set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_home"></a>gx_single_line_text_input_home


Metin girişi imlecini ana konuma taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_home(GX_SINGLE_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet metin girişi imleç konumunu giriş dizesinin başlangıcına taşımaktır. Bu hizmet, ana anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) imleci ana konuma başarıyla taşındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move cursor to the start of the input text. */
status = gx_single_line_text_input_home(&my_text_input);

/* If status is GX_SUCCESS the cursor has been moved to the home position */
```

### <a name="see-also"></a>Ayrıca Bkz.
- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_left_arrow"></a>gx_single_line_text_input_left_arrow


Giriş imleci bir karakter sola taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_left_arrow(GX_SINGLE_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin giriş imlecini bir karakter sola kaydırır. Bu hizmet, sol tuşu basılı bir olay alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) Imleç sola başarıyla taşındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move the cursor one character to the left. */
status = gx_single_line_text_input_left_arrow(&my_text_input);

/* If status is GX_SUCCESS the text input cursor has been moved one character to the left. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_position_get"></a>gx_single_line_text_input_position_get

İmleci piksel konumuna taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_position_get(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    INT pixel_position);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin giriş imlecini istenen piksel konumuna göre konumlandırır. Metin girişi imleç dizini, piksel konumunun x değeri temel alınarak hesaplanır. Bu hizmet, bir kalem aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu
- **pixel_position** Piksel konumunun X değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) imleci Istenen konuma başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set cursor to requested position. */
status = gx_single_line_text_input_position_get(&my_text_input,
                                                100);

/* If status is GX_SUCCESS the text input widget cursor has been positioned */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_right_arrow"></a>gx_single_line_text_input_right_arrow


Giriş imlecini bir karakter sağa taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_right_arrow(
    GX_SINGLE_LINE_TEXT_INPUT *text_input);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin giriş imlecini bir karakter sağa kaydırır. Bu hizmet, doğru bir anahtar aşağı olayı alındığında dahili olarak çağrılır, ancak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) Imleç sağa başarıyla taşındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move cursor one character to the right. */
status = gx_single_line_text_input_right_arrow(&my_text_input);

/* If status is GX_SUCCESS the text input cursor has been moved one character to the right. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_position_get
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_style_add"></a>gx_single_line_text_input_style_add


Stil Ekle

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_style_add(
    GX_SINGLE_LINE_TEXT_INPUT *text_input, 
    ULONG style);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen stili (öğeleri) tek satırlık metin girişi pencere öğesine ekler.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu
- **Stil** Eklenecek yeni stil. **Ek D** tüm pencere öğeleri için önceden tanımlanmış genel stilleri içerir

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) stil pencere öğesine başarıyla eklendi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Add a new style to “my_text_input”. */
status = gx_single_line_text_input_style_add(&my_text_input,
GX_STYLE_CURSOR_AWAYS);

/* If status is GX_SUCCESS the GX_STYLE_CUSROSR_SHOR have been successfully added. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gax_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_style_remove"></a>gx_single_line_text_input_style_remove

Stilleri kaldır

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_style_remove(
    GX_SINGLE_LINE_TEXT_INPUT *text_input, 
    ULONG style);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen stili (öğeleri) tek satırlık metin girişi pencere öğesinden kaldırır.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu
- **Stil** Kaldırılacak stil (ler). **Ek D** tüm pencere öğeleri için önceden tanımlanmış genel stilleri içerir

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) pencere öğesi içindeki stil (ler) başarıyla kaldırıldı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Remove cursor blink style from “my_text_input”. */
status = gx_single_line_text_input_style_remove(&my_text_input,
GX_STYLE_CURSOR_BLINK);

/* If status is GX_SUCCESS the GX_STYLE_CURSOR_BLINK style has been successfully removed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_home
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_style_set"></a>gx_single_line_text_input_style_set


Metin girişi stillerini ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_style_set(
    GX_SINGLE_LINE_TEXT_INPUT *text_input, 
    ULONG style);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen stili (öğeleri) tek satırlık metin girişi pencere öğesine ayarlar.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi pencere öğesi denetim bloğu
- atanacak **Stil** stili bayrakları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) metin girişi stilini başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set style for “my_text_input”. */
status = gx_single_line_text_input_style_set(&my_text_input,
                    GX_STYLE_ENABLED | GX_STYLE_CURSOR_BLINK);

/* If status is GX_SUCCESS the text input style has been successfully set to the specified styles. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_signle_line_text_input_event_process
- gx_single_line_text_input_home
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_text_color_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_text_color_set"></a>gx_single_line_text_input_text_color_set


Tek satırlık metin girişi metin rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_text_color_set(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    GX_RESOURCE_ID normal_text_color_id,
    GX_RESOURCE_ID selected_text_color_id,
    GX_RESOURCE_ID disabled_text_color_id,
    GX_RESOURCE_ID readonly_text_color_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, tek satırlık metin girişinin metin rengini ayarlar.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi denetim bloğu işaretçisi
- **normal_text_color_id** Normal durumdaki metin renginin kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **selected_text_color_id** Pencere öğesi odaklanıldığında metin renginin kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **disabled_text_color_id** Stil GX_STYLE_ENABLED ayarlanmamışsa metin renginin kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **readonly_text_color_id** Stil GX_STYLE_ENABLED ve GX_STYLE_TEXT_INPUT_READONLY her ikisi de ayarlandığında metin renginin kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tek satırlık metin girişi metin rengi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set text colors for single line text input “my_text_input”. */
status = gx_single_line_text_input_text_color_set(&my_text_input,
                                        GX_COLOR_ID_NORMAL_TEXT,
                                        GX_COLOR_ID_SELECTED_TEXT,
                                        GX_COLOR_ID_DISABLED_TEXT,
                                        GX_COLOR_ID_READONLY_TEXT);

/* If status is GX_SUCCESS, the text color “my_text_input” was set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_select
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_text_select"></a>gx_single_line_text_input_text_select

Metin Seç

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_text_color_set(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    UINT start_index, UINT end_index);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen başlangıç işaretine ve bitiş işareti dizinine sahip metinleri seçer ve seçilen metni seçilen Fill ve Text renkleriyle vurgular.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi denetim bloğu işaretçisi
- **start_index** Seçilen ilk karakterin dizini
- **end_index** Son seçili karakterin dizini

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tek satırlık metin girişi metin seçimi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) dizin değeri geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Select text between index [0, 9]. */
status = gx_single_line_text_input_text_select(&my_text_input,
                                                0,9);

/* If status is GX_SUCCESS, the text between index [0, 9] “my_text_input” was selected. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_set

## <a name="gx_single_line_text_input_text_set"></a>gx_single_line_text_input_text_set


Tek satırlı metin giriş metnini ayarla (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_text_set(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    GX_CONST GX_CHAR *text);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_single_line_text_input_text_set_ext () kullanım dışı bırakıldı

Bu hizmet, tek satırlık metin girişinin metnini ayarlar.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi denetim bloğu işaretçisi
- **metin** NULL ile sonlandırılmış metin dizesi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tek satırlık metin girişi metin rengi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CONST GX_CHAR new_text = “Set Single Line Text Input Text”;

/* Set text for single line text input “my_text_input”. */
status = gx_single_line_text_input_text_set(&my_text_input,
                                        new_text);

/* If status is GX_SUCCESS, the text of “my_text_input” was set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_text_set_ext

## <a name="gx_single_line_text_input_text_set_ext"></a>gx_single_line_text_input_text_set_ext


Tek satırlık metin giriş metnini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_single_line_text_input_text_set(
    GX_SINGLE_LINE_TEXT_INPUT *text_input,
    GX_CONST GX_STRING *string);
```

### <a name="description"></a>Açıklama

Bu hizmet, tek satırlık metin girişinin metnini ayarlar.

### <a name="parameters"></a>Parametreler

- **text_input** Tek satırlı metin girişi denetim bloğu işaretçisi
- **dize** GX_STRING değişkeni

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı tek satırlık metin girişi metin rengi kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING new_string;
new_string.gx_string_ptr = “Set Single Line Text Input Text”;
new_string.gx_string_length = strlen(new_string.gx_string_ptr);

/* Set text for single line text input “my_text_input”. */
status = gx_single_line_text_input_text_set_ext(&my_text_input,
                                        &new_string);

/* If status is GX_SUCCESS, the string has been assigned to my_text_input. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_single_line_text_input_backspace
- gx_single_line_text_input_buffer_clear
- gx_single_line_text_input_buffer_get
- gx_single_line_text_input_character_delete
- gx_single_line_text_input_character_insert
- gx_single_line_text_input_create
- gx_single_line_text_input_draw
- gx_single_line_text_draw_position_get
- gx_single_line_text_input_end
- gx_single_line_text_input_event_process
- gx_single_line_text_input_fill_color_set
- gx_single_line_text_input_home
- gx_single_line_text_input_left_arrow
- gx_single_line_text_input_position_get
- gx_single_line_text_input_right_arrow
- gx_single_line_text_input_style_add
- gx_single_line_text_input_style_remove
- gx_single_line_text_input_style_set
- gx_single_line_text_input_text_set_ext


## <a name="gx_slider_create"></a>gx_slider_create

Kaydırıcı oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_slider_create(
    GX_SLIDER *slider, 
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent, INT tick_count,
    GX_SLIDER_INFO *slider_info,
    ULONG style, USHORT slider_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir kaydırıcı pencere öğesi oluşturur.

GX_SLIDER GX_WIDGET türetilir ve bu nedenle tüm gx_widget API hizmetleri GX_SLIDER türü pencere öğeleri ile kullanılabilir.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu
- **ad**: kaydırıcının adı
- **Parent**: üst pencere öğesi işaretçisi
- **tick_count**: kaydırıcı işaretleri sayısı
- **slider_info**: kaydırıcı değeri sınırlarını, kaydırıcı iğne boyutunu ve konumunu ve diğer kaydırıcı parametrelerini geçirmek için kullanılan bir yapı olan kaydırıcı bilgisine yönelik işaretçi. **Ek ı** GX_SLIDER_INFO yapısına yönelik tanımı içerir.
- **Stil**: kaydırıcı stili. **Ek D** , tüm pencere öğeleri için önceden tanımlanmış genel stilleri ve pencere öğesine özgü stilleri içerir.
- **slider_id**: uygulama TANıMLı kaydırıcının kimliği
- **Boyut**: kaydırıcının boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı kaydırıcı oluşturma
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED**: (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE**: (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET**: (0x12) üst pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create slider “my_slider”. */

GX_SLIDER my_slider;
GX_SLIDER_INFO info;

info.gx_slider_info_min_val = 0;
info.gx_slider_info_max_val = 100;
info.gx_slider_info_current_val = 50;
info.gx_slider_info_increment = 1;
info.gx_slider_info_min_travel = 20;
info.gx_slider_info_max_travel = 20;
info.gx_slider_info_needle_width = 10;
info.gx_slider_info_needle_height = 10;
info.gx_slider_info_needle_inset = 5;
info.gx_slider_info_needle_hotspot_offset = 5;

status = gx_slider_create(&my_slider, “my_slider”,
    &my_parent, 10, info, GX_STYLE_ENABLED, ID_MY_SLIDER, &size);

/* If status is GX_SUCCESS the slider “my_slider” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_slider_draw"></a>gx_slider_draw

Çizim kaydırıcısı

### <a name="prototype"></a>Prototype

```C
VOID gx_slider_draw(GX_SLIDER *slider);
```

### <a name="description"></a>Açıklama

Bu hizmet bir kaydırıcı çizer. Bu hizmet gx_slider_create işlevi tarafından dahili olarak kullanılır, ancak özel bir kaydırıcı çizim işlevi tanımlandığında Bu örneklerde uygulama tarafından kullanılmak üzere de sunulur.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom slider draw function. */
VOID my_slider_draw(GX_SLIDER *slider)
{
    /* Call default slider draw. */
    gx_slider_draw(slider);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_slider_event_process"></a>gx_slider_event_process

İşlem kaydırıcı olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_slider_event_process(
    GX_SLIDER *slider, 
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet bir kaydırıcı olayını işler. Bu işleve gx_slider_create işlevi tarafından dahili olarak başvurulur, ancak uygulamanın özel bir kaydırıcı olay işleme işlevini tanımladığı durumlarda uygulama tarafından kullanıma sunulur.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu
- **olay**: işlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı kaydırıcı olay işlemi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic slider event processing as part of custom event processing function. */

UINT custom_slider_event_process(GX_SLIDER *slider,
    GX_EVENT *event)
{
    UINT status = GX_SUCCESS;
    switch(event->gx_event_type)
    {
        case xyz:
            /* Insert custom event handling here */
            break;
        default:
            /* Pass all other events to the default slider event processing */
            status = gx_slider_event_process(slider, event);
            break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_slider_info_set"></a>gx_slider_info_set

Kaydırıcı bilgi bloğunu ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_slider_info_set(
    GX_SLIDER *slider, 
    GX_SLIDER_INFO *info);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırıcı minimum, Slider maksimum ve kaydırıcı geçerli değeri gibi belirtilen kaydırıcı bilgilerini belirtilen kaydırıcıya atar. Kaydırıcı, yeni kaydırıcı bilgilerine göre iğne konumunu güncelleştirir ve yeniden çizer.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu
- **bilgi**: kaydırıcı bilgi yapısına yönelik işaretçi. **Ek ı** GX_SLIDER_INFO yapısına yönelik tanımı içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) kaydırıcı bilgilerini başarıyla ayarla
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_SLIDER_INFO my_slider_info;
my_slider_info.gx_slider_info_min_val = 0;
my_slider_info.gx_slider_info_max_val = 100;
my_slider_info.gx_slider_info_current_val = 50;
my_slider_info.gx_slider_info_increment = 1;
my_slider_info.gx_slider_info_min_travel = 20;
my_slider_info.gx_slider_info_max_travel = 20;
my_slider_info.gx_slider_info_needle_width = 10;
my_slider_info.gx_slider_info_needle_height = 10;
my_slider_info.gx_slider_info_needle_inset = 5;

my_slider_info.gx_slider_info_needle_hotspot_offset = 5;

/* Set slider information for slider “my_slider”. */
status = gx_slider_info_set (&my_slider, &my_slider_info);

/* If status is GX_SUCCESS the “my_slider” is configured with my_slider_info. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_slider_needle_draw"></a>gx_slider_needle_draw

Çiz kaydırıcı iğne

### <a name="prototype"></a>Prototype

```C
VOID gx_slider_needle_draw(GX_SLIDER *slider);
```

### <a name="description"></a>Açıklama

Bu hizmet bir kaydırıcı iğne çizer. Bu hizmet gx_slider_draw işlevi tarafından otomatik olarak çağrılır, ancak özelleştirilmiş kaydırıcı çizim işlevinin bir parçası olarak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom slider draw function. */
VOID my_slider_draw(GX_SLIDER *slider)
{
    /* Add your own background draw here. */

    /* Call default tickmarks draw. */
    gx_slider_tickmarks_draw(slider);

    /* Call default slider needle draw. */
    gx_slider_needle_draw(slider);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_slider_needle_position_get"></a>gx_slider_needle_position_get

Kaydırıcı iğne konumunu al

### <a name="prototype"></a>Prototype

```C
UINT gx_slider_needle_position_get(
    GX_SLIDER *slider,
    GX_SLIDER_INFO *slider_info,
    GX_RECTANGLE *return_position);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırıcı iğne konumunu geçerli kaydırıcı değerine göre hesaplar.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu
- **slider_info**: kaydırıcı sınırlarını, iğne boyutunu ve kaydırmayı ve diğer kaydırıcı parametrelerini tanımlayan kaydırıcı bilgi yapısına yönelik işaretçi. **Ek ı** GX_SLIDER_INFO yapısına yönelik tanımı içerir.
- **return_position**: iğne konumu için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı kaydırıcı iğne konumu al
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE**: (0x22) kaydırıcı bilgisi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RECTANGLE needle_position;

/* Get the needle position for slider “my_slider”. */
status = gx_slider_needle_posistion_get(&my_slider, &slider_info,
    &needle_position);

/* If status is GX_SUCCESS the needle position for slider “my_slider” has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_slider_tickmarks_draw"></a>gx_slider_tickmarks_draw

Çiz kaydırıcı tickiþaretleri

### <a name="prototype"></a>Prototype

```C
VOID gx_slider_tickmarks_draw(GX_SLIDER *slider);
```

### <a name="description"></a>Açıklama

Bu hizmet kaydırıcı tickişaretlerini çizer. Bu işlev gx_slider_draw işlevi tarafından dahili olarak çağrılır, ancak özel bir kaydırıcı çizim işlevi uygulayabilen uygulamalar tarafından kullanıma sunulur.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom slider draw function. */
VOID my_slider_draw(GX_SLIDER *slider)
{
    /* Add your own background draw here. */

    /* Call default tickmarks draw. */
    gx_slider_tickmarks_draw(slider);

    /* Call default slider needle draw. */
    gx_slider_needle_draw(slider);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_travel_get
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_slider_travel_get"></a>gx_slider_travel_get

Kaydırıcı gezmasını al

### <a name="prototype"></a>Prototype

```C
UINT gx_slider_travel_get(
    GX_SLIDER *widget,
    GX_SLIDER_INFO *info,
    INT *return_min_travel, 
    INT *return_max_travel);
```

### <a name="description"></a>Açıklama

Bu hizmet kaydırıcı gezmasını alır.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu
- **bilgi**: kaydırıcı bilgi yapısına yönelik işaretçi. **Ek ı** GX_SLIDER_INFO yapısına yönelik tanımı içerir.
- **return_min_travel**: en düşük seyahat değeri için hedef işaretçisi</td>
- **return_max_travell**: en yüksek seyahat değeri için hedef işaretçisi</td>

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı kaydırıcı seyahat al
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE**: (0x22) kaydırıcı bilgisi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Get travel information for for slider “my_slider”. */
status = gx_slider_travel_get(&my_slider, &info,
    &my_min_travel, &my_max_travel);

/* If status is GX_SUCCESS the travel max/min values for slider “my_slider” have been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_value_calculate
- gx_slider_value_set

## <a name="gx_slider_value_calculate"></a>gx_slider_value_calculate

Kaydırıcı değerini hesapla

### <a name="prototype"></a>Prototype

```C
UINT gx_slider_value_calculate(
    GX_SLIDER *slider, 
    GX_SLIDER_INFO *info,
    INT new_position);
```

### <a name="description"></a>Açıklama

Bu hizmet kaydırıcı değerini kaydırıcı iğne konumuna göre hesaplar. Bu işlev, Kullanıcı kaydırıcı iğne 'yi taşırken Gux tarafından dahili olarak çağrılır, ancak özel bir kaydırıcı pencere öğesi uygularken uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu
- **bilgi**: kaydırıcı bilgisine yönelik işaretçi. **Ek ı** GX_LISDER_INFO yapısına yönelik tanımı içerir.
- **new_position**: yeni kaydırıcı konumu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı kaydırıcı değeri hesaplaması
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE**: (0x22) kaydırıcı bilgisi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Calculate new value for slider “my_slider”. */
status = gx_slider_value_calculate(&my_slider,
    &my_slider.gx_slider_info, new_slider_position);

/* If status is GX_SUCCESS the slider value of “my_slider” has been calculated. */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_set

## <a name="gx_slider_value_set"></a>gx_slider_value_set

Kaydırıcı değerini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_slider_value_set(
    GX_SLIDER *slider,
    GX_SLIDER_INFO *info, 
    INT new_value);
```

### <a name="description"></a>Açıklama

Bu hizmet kaydırıcı değerini ayarlar. Bu API, uygulama tarafından, kaydırıcı iğne 'yi sürüklemek için Kullanıcı girişi gereksinimini atlayarak program denetimi altına bir kaydırıcı iğne taşımak için çağrılabilir.

### <a name="parameters"></a>Parametreler

- **kaydırıcı**: kaydırıcı pencere öğesi denetim bloğu
- **bilgi**: kaydırıcı bilgi yapısına yönelik işaretçi. **Ek ı** GX_SLIDER_INFO yapısına tanım içeriyor
- **new_value**: yeni kaydırıcı değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı kaydırıcı değer kümesi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set new value for slider “my_slider”. */
status = gx_slider_value_set(&my_slider,
    &my_slider.gx_slider_info, new_value);

/* If status is GX_SUCCESS the new value has been set for slider “my_slider”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_pixelmap_slider_create
- gx_pixelmap_slider_draw
- gx_pixelmap_slider_event_process
- gx_pixelmap_slider_pixelmap_set
- gx_slider_create
- gx_slider_draw
- gx_slider_event_process
- gx_slider_needle_draw
- gx_slider_needle_position_get
- gx_slider_needle_position_get
- gx_slider_tickmarks_draw
- gx_slider_travel_get
- gx_slider_value_calculate

##  <a name="gx_sprite_create"></a>gx_sprite_create

Bir sprite pencere öğesi oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_sprite_create(
    GX_SPRITE *sprite, GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    GX_SPRITE_FRAME *frame_list,
    USHORT frame_count,
    ULONG style, USHORT sprite_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir GX_SPRITE pencere öğesi oluşturur. Bir sprite, bir animasyon içinde olan bir veya birden çok durumlu pixelmap görüntüleme pencere öğesi olarak kullanılabilecek bir dizi pixelharita göstermek için kullanılır.

GX_SPRITE GX_WIDGET türetilir ve tüm gx_widget API hizmetlerini destekler.

GX_SPRITE pencere öğesi, SPRITE animasyonunu tanımlamak için GX_SPRITE_FRAME yapılarından oluşan bir dizi gerektirir. **Ek ı** GX_PRITE_FRAME yapısına yönelik tanımı içerir.

### <a name="parameters"></a>Parametreler

- **Sprite**: sprite pencere öğesi denetim bloğu
- **ad**: isteğe bağlı Sprite adı
- **Parent**: üst pencere öğesi işaretçisi
- **frame_list**: GX_SPRITE_FRAME yapılarının dizisi
- **frame_count**: Çerçeve listesi dizisindeki giriş sayısını belirtir
- **Stil**: sprite stili. **Ek D** , tüm pencere öğeleri için önceden tanımlanmış genel stilleri ve pencere öğesine özgü stilleri içerir.
- **sprite_id**: uygulama TANıMLı Sprite kimliği
- **Boyut**: Hareketli grafiğin boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarıyla Sprite oluştur
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED**: (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_WIDGET**: (0x12) üst pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create sprite “my_sprite”. */

status = gx_sprite_create(&my_sprite, “my_sprite”,
    &my_parent,
    sprite_frame_list, frame_count,
    GX_STYLE_SPRITE_AUTO|GX_STYLE_SPRITE_LOOP,
    ID_MY_SPRITE, &size);

/* If status is GX_SUCCESS the sprite “my_sprite” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_sprite_start
- gx_sprite_stop
- gx_sprite_current_frame_set
- gx_sprite_frame_list_set

## <a name="gx_sprite_current_frame_set"></a>gx_sprite_current_frame_set

Sprite çerçevesini ata

### <a name="prototype"></a>Prototype

```C
UINT gx_sprite_current_frame_set(
    GX_SPRITE *sprite, 
    USHORT frame);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli Sprite çerçevesini atar. GX_SPRITE pencere öğesi otomatik olarak çalışmıyorsa, bir program denetimli durum ışığı olarak kullanılabilir ve bu da commanded çerçeve pixelmap 'i görüntülüyor.

### <a name="parameters"></a>Parametreler

- **Sprite**: sprite pencere öğesi denetim bloğu
- **çerçeve**: görüntülenecek Sprite çerçevesi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Assign frame number 3 as the current sprite frame */
status = gx_sprite_current_frame_set(&my_sprite, 3);

/* If status is GX_SUCCESS the sprite “my_sprite” will display frame index 3. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_sprite_start
- gx_sprite_stop
- gx_sprite_create
- gx_sprite_frame_list_set

## <a name="gx_sprite_frame_list_set"></a>gx_sprite_frame_list_set

Bir sprite çerçeve listesi atama veya değiştirme

### <a name="prototype"></a>Prototype

```C
UINT gx_sprite_frame_list_set(
    GX_SPRITE *sprite,
    GX_SPRITE_FRAME *frame_list,
    USHORT frame_count);
```

### <a name="description"></a>Açıklama

Bu hizmet, Sprite pencere öğesi oluşturulduktan sonra bir sprite pencere öğesi tarafından kullanılan çerçeve listesini atamak veya yeniden atamak için kullanılabilir. Bir sprite çerçeve listesinin içeriği hakkında daha fazla bilgi için gx_sprite_create API belgelerine bakın.

### <a name="parameters"></a>Parametreler

- **Sprite**: sprite pencere öğesi denetim bloğu
- **frame_list**: GX_SPRITE_FRAME yapılarının dizisi veya çerçeve listesi yoksa GX_NULL.
- **frame_count**: Çerçeve listesi dizisindeki çerçeve sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı Sprite çerçeve listesi kümesi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Assign framelist_1, which has 10 frames, to my_sprite */
status = gx_sprite_frame_list_set(&my_sprite, framelist_1, 10);

/* If status is GX_SUCCESS the new frame list is now associated with this sprite */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_sprite_current_frame_set
- gx_sprite_stop
- gx_sprite_create
- gx_sprite_create

## <a name="gx_sprite_start"></a>gx_sprite_start

Bir sprite çalışma sırası başlatma

### <a name="prototype"></a>Prototype

```C
UINT gx_sprite_start(
    GX_SPRITE *sprite, 
    USHORT frame);
```

### <a name="description"></a>Açıklama

Bu hizmet bir sprite otomatik çalıştırma sırası başlatır. Sprite pencere öğesi, son çerçeveye ulaşılana kadar veya GX_SPRITE_LOOP stili ayarlandıysa sürekli olarak çalışacak şekilde Sprite çerçeveleri boyunca geçiş yapar.

### <a name="parameters"></a>Parametreler

- **Sprite**: sprite pencere öğesi denetim bloğu
- **çerçeve**: görüntülenecek ilk Sprite çerçevesi, genellikle kare 0

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) Sprite çalıştırması başarıyla başlatıldı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Start the sprite “my_sprite” */
status = gx_sprite_start(&my_sprite, 0);

/* If status is GX_SUCCESS the sprite “my_sprite” will start running */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_sprite_current_frame_set
- gx_sprite_stop
- gx_sprite_create
- gx_sprite_frame_list_set

## <a name="gx_sprite_stop"></a>gx_sprite_stop

Bir sprite çalışma sırasını durdur

### <a name="prototype"></a>Prototype

```C
UINT gx_sprite_stop(GX_SPRITE *sprite);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir sprite otomatik çalıştırma sırasını durduruyor.

### <a name="parameters"></a>Parametreler

- **Sprite**: sprite pencere öğesi denetim bloğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) Sprite çalıştırmasını başarıyla durdurdu
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Stop the sprite sequence */
status = gx_sprite_stop(&my_sprite);

/* If status is GX_SUCCESS the sprite “my_sprite” is stopped. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_sprite_current_frame_set
- gx_sprite_start
- gx_sprite_create
- gx_sprite_frame_list_set

## <a name="gx_string_scroll_wheel_create"></a>gx_string_scroll_wheel_create

Dize türü kaydırma tekerleği oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_string_scroll_wheel_create(
    GX_STRING_SCROLL_WHEEL *wheel,
    GX_CONST GX_CHAR *name, 
    GX_WIDGET *parent, 
    INT total_rows,
    GX_CONST GX_CHAR **string_list, 
    ULONG style,
    USHORT Id, 
    GX_CONST GX_RECTANGLE *size)
```

### <a name="description"></a>Açıklama

Bu hizmet bir dize türü kaydırma tekerleği oluşturur.

GX_STRING_SCROLL_WHEEL GX_TEXT_SCROLL_WHEEL türetilir ve bu nedenle tüm gx_text_scroll_wheel API işlevleri GX_STRING_SCROLL_WHEEL pencere öğeleri ile birlikte kullanılabilir.

Uygulama, kaydırma tekerleği tarafından görüntülenecek dizeleri tanımlayan oluşturma işlevine basit bir dize dizisi geçirebilir veya uygulama, string_list parametresi olarak GX_NULL geçirebilir ve `gx_string_scroll_wheel_string_id_list_set()` dize kimlikleri dizisi sağlamak üzere API 'yi çağırabilir. İkinci yöntem kullanılırsa, dize kaydırma tekerleği, etkin uygulama dili değiştirilirse, görüntülenecek dizeleri otomatik olarak geçer.

Alternatif olarak, görüntülenecek dizeler, kaydırma tekerleği oluşturulduğu sırada statik olarak tanımlanmazsa veya bilmiyor ise, uygulama GX_NULL dize listesi parametresi olarak geçirebilir ve bir geri çağırma işlevi tanımlamak için gx_text_scroll_wheel_callback_set () API işlevini çağırıp, dizelerin gerçek zamanlı olarak görüntülenmesini sağlar.

### <a name="parameters"></a>Parametreler

- **tekerlek**: dize kaydırma tekerleği denetim bloğu adresi
- **ad**: uygulama tanımlı pencere öğesi adı
- **üst öğe**: tekerlek üstü veya GX_NULL
- **total_rows**: kullanıcıya sunulacak toplam satır sayısı
- **string_list**: statik olarak tanımlanmış dize dizisi veya GX_NULL
- **Stil**: istenen stil bayrakları
- **Kimlik**: uygulama tanımlı tekerlek stili bayrakları
- **Boyut**: ilk kaydırma tekerleği boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) dize kaydırma tekerleği başarıyla oluşturuldu
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR (0x07)**: geçersiz işaretçi
- **GX_ALREADY_CREATED**: (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CONST GX_CHAR *days[] = {
    “Sunday”,
    “Monday”,
    “Tuesday”,
    “Wednesday”,
    “Thursday”,
    “Friday”,
    “Saturday”
};

GX_STRING_SCROLL_WHEEL wheel;

/* Create the string scroll wheel. */

status = gx_string_scroll_wheel_create(&wheel, “Day Wheel”,
    root, 7, days,
    GX_STYLE_ENABLED|GX_STYLE_TEXT_CENTER|GX_STYLE_TRANSPARENT|
    GX_STYLE_WRAP|GX_STYLE_TEXT_SCROLL_WHEEL_ROUND,
    ID_SCROLL_WHEEL_DAY, &size);

/* If status is GX_SUCCESS the string scroll wheel has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_string_id_list_set
- gx_string_scroll_wheel_string_list_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set

## <a name="gx_string_scroll_wheel_event_process"></a>gx_string_scroll_wheel_event_process


İşlem dizesi kaydırma tekerleği olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_string_scroll_wheel_string_id_list_set(
    GX_STRING_SCROLL_WHEEL *wheel,
    GX_CONST GX_RESOURCE_ID *string_id_list, 
    INT id_count);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen dize kaydırma tekerleği için bir olayı işler. Bu hizmet özel bir dize kaydırma tekerleği olay işleme işlevleri tarafından varsayılan olay işleyicisi olarak çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **tekerlek** Dize kaydırma tekerleği denetim bloğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı dize kaydırma tekerleği olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic string scroll wheel event processing as part of custom event processing function. */

UINT custom_string_scroll_wheel_event_process(GX_STRING_SCROLL_WHEEL *wheel, GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;

    default:
        /* Pass all other events to the default string scroll wheel event processing */
        status = gx_string_scroll_wheel_event_process(wheel, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_string_id_list_set
- gx_string_scroll_wheel_string_list_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set

## <a name="gx_string_scroll_wheel_string_id_list_set"></a>gx_string_scroll_wheel_string_id_list_set

Dize kimlikleri dizisi ata

### <a name="prototype"></a>Prototype

```C
UINT gx_string_scroll_wheel_string_id_list_set(
    GX_STRING_SCROLL_WHEEL *wheel,
    GX_CONST GX_RESOURCE_ID *string_id_list, INT id_count);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir dize bir kaydırma tekerleği pencere öğesine dize kimlikleri dizisi atar. Dizelerin statik olarak tanımlanması ve pencere öğesinin birden çok dilde çalışması gerekiyorsa, dize kaydırma tekerleği için dizeler atama yöntemi önerilir. Bu API kullanılacaksa, önce kaydırma tekerleği pencere öğesi bir GX_NULL dize listesi ile oluşturulmalıdır.

### <a name="parameters"></a>Parametreler

- **tekerlek**: dize kaydırma tekerleği denetim bloğu adresi
- **string_id_list**: dize kimlikleri dizisi
- **id_count**: kimlik listesinin boyutu.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) dize kimliği dizisi başarıyla ayarlandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE**: 0x22) geçersiz kimlik listesi boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CONST RESOURCE_ID wheel_ids[] = {
    GX_STRING_ID_SUNDAY,
    GX_STRING_ID_MONDAY,
    GX_STRING_ID_TUESDAY,
    GX_STRING_ID_WEDNESDAY,
    GX_STRING_ID_THURSDAY,
    GX_STRING_ID_FRIDAY,
    GX_STRING_ID_SATURDAY
};

GX_STRING_SCROLL_WHEEL wheel;

/* Stop the sprite sequence */

status = gx_string_scroll_wheel_string_id_list_set(&wheel, wheel_ids, 7);

/* If status is GX_SUCCESS the ID list has been assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_string_list_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set

## <a name="gx_string_scroll_wheel_string_list_set"></a>gx_string_scroll_wheel_string_list_set

Dize dizisi ata

### <a name="prototype"></a>Prototype

```C
UINT gx_string_scroll_wheel_string_list_set(
    GX_STRING_SCROLL_WHEEL *wheel,
    GX_CONST GX_CHAR *string_list, 
    INT string_count);
```

### <a name="description"></a>Açıklama

Bu, dize kaydırma tekerleği pencere öğesine bir dize dizisi atar. Pencere öğesi başlangıçta oluşturulduktan sonra görüntülenecek dizeleri değiştirmek için bu kullanılabilir.

String_scroll_wheel GX_STYLE_TEXT_COPY desteklemediğini ve bu işleve geçirilen dizelerin dizisinin, uygulama tarafından statik olarak tanımlanması gerektiğini unutmayın.

### <a name="parameters"></a>Parametreler

- **tekerlek**: dize kaydırma tekerleği denetim bloğu adresi
- **string_list**: dize işaretçileri dizisi
- **string_count**: dize dizisinin boyutu.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) kaydırma tekerleği Için dizeleri başarıyla değiştirdi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE**: (0x22) geçersiz dize listesi boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CONST GX_CHAR *days[] = {
    “Sunday”,
    “Monday”,
    “Tuesday”,
    “Wednesday”,
    “Thursday”,
    “Friday”,
    “Saturday”
};

GX_STRING_SCROLL_WHEEL wheel;

/* Set the array of strings to the scroll wheel. */

status = gx_string_scroll_wheel_string_list_set(&wheel, days, 7);

/* If status is GX_SUCCESS the string array has been assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_string_scroll_wheel_create
- gx_string_scroll_wheel_event_process
- gx_string_scroll_wheel_string_list_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set

## <a name="gx_studio_widget_create"></a>gx_studio_widget_create

Studio tarafından oluşturulan belirtim dosyasında tanımlı pencere öğesi oluştur

### <a name="prototype"></a>Prototype

```C
GX_WIDGET *gx_studio_widget_create(
    GX_BYTE *control,
    GX_CONST GX_STUDIO_WIDGET *definition, 
    GX_WIDGET *parent);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir pencere öğesi ve pencere öğesinin alt öğelerini Gux Studio tarafından üretilen belirtim dosyası içinde tanımlanan pencere öğesi belirtimini kullanarak oluşturur. Bu işlev, benzer işlevin "ada göre" aramasını önler `gx_studio_named_widget_create()` .

GX_STUDIO_WIDGET yapısı, GUıDX Studio tarafından oluşturulan uygulama belirtimleri üstbilgi dosyasında tanımlanmıştır.

Statik olarak ayrılan pencere öğeleri için pencere öğesi denetim bloğu, oluşturulan belirtimler. c dosyasında tanımlanır ve Gux Studio içinde tanımlanan pencere öğesi adı verilir. Dinamik olarak ayrılan pencere öğeleri için, uygulama pencere öğesi denetim bloğu adresi olarak GX_NULL geçirmeli ve işlev, `gx_system_memory_allocate()` tarafından da tanımlanan ve uygulama tarafından belirtilen işlevi kullanarak pencere öğesi denetim bloğunu dinamik olarak ayırmaya çalışır.

Bir uygulamanın, oluşturulan belirtimler dosyası içindeki Gux Studio pencere öğesi tanımına doğrudan başvurması için, GUI Studio kod üreticisi tarafından kullanılan adlandırma kuralını izlemeniz gerekir. Belirtimleri. c dosyasında oluşturulan GX_STUDIO_WIDGET yapısı şu kurala göre her zaman adlandırılır: pencere öğesi alt pencere öğesinin alt öğesi ise, <widget_name> alanının birden çok kez tekrarlanbildiği widget_name>_define <.

### <a name="parameters"></a>Parametreler

- **Denetim** Pencere öğesi denetim bloğu işaretçisi veya dinamik olarak ayrılmışsa GX_NULL.
- **tanım** Studio tarafından oluşturulan pencere öğesi tanım yapısı
- varsa pencere öğesi üst öğesine ait **üst** işaretçi

### <a name="return-values"></a>Dönüş Değerleri

Oluşturulan pencere öğesi denetim bloğuna yönelik işaretçi veya oluşturma işlemi başarılı olmazsa GX_NULL.

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create the widget “playlist_screen”, which is statically allocated. */

widget = gx_studio_widget_create(&playlist_screen,
    &playlist_screen_define,
    root_window);

/* If widget != GX_NULL the widget was created. */

/* create the widget “songs_screen”, which is dynamically allocated */

widget = gx_studio_widget_create(GX_NULL,
    &songs_screen_define, root_window);
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_studio_named_widget_create

## <a name="gx_studio_named_widget_create"></a>gx_studio_named_widget_create

Studio tarafından oluşturulan belirtim dosyasında tanımlı pencere öğesi oluştur

### <a name="prototype"></a>Prototype

```C
UINT *gx_studio_named_widget_create(
    char *name, 
    GX_WIDGET *parent,
    GX_WIDGET **new_widget);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir pencere öğesi ve pencere öğesinin alt öğelerini Gux Studio tarafından üretilen belirtim dosyası içinde tanımlanan pencere öğesi belirtimini kullanarak oluşturur.

Bu API işlevi, pencere öğesi tanım tanımlayıcısı olarak Gux Studio uygulamasında belirtilen ekran adını kullanarak en üst düzey ekranları oluşturmak için kullanılır.

### <a name="parameters"></a>Parametreler

- **ad**: ekran adı Gux Studio uygulaması içinde tanımlandığı şekilde.
- **Parent**: varsa pencere öğesi üst öğesine işaretçi
- **new_widget**: oluşturulan pencere öğesi işaretçisini döndürecek konum

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı
- **GX_FAILURE**: (0x11) adlandırılmış pencere öğesi bulunamadı

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create the widget named “child_popup”,
   which is a child of the top-level screen “main_screen”. */

GX_WIDGET *menu_screen;

status = gx_studio_named_widget_create(“main_menu”,
    &root_window, &menu_screen);

/* If status == GX_SUCCESS the screen was created
   and linked to the root window. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_studio_widget_create

## <a name="gx_studio_display_configure"></a>gx_studio_display_configure

GUX Studio projesinde tanımlanan ekranı Yapılandır

### <a name="prototype"></a>Prototype

```C
UINT *gx_studio_display_configure(
    USHORT display,
    UINT (*driver)(GX_DISPLAY *),
    USHORT language, 
    USHORT theme,
    GX_WINDOW_ROOT **return_root);
```

### <a name="description"></a>Açıklama

Bu hizmet, kullanıma hazırlanabilmesi için bir GX_DISPLAY başlatır. Bu işlev, GX_DISPLAY bir denetim bloğu başlatmak, ekrana sığacak bir tuval oluşturmak ve tuval için bir kök pencere oluşturmak üzere işlevleri birleştirir. Bu işlev Ayrıca, görüntüleme başlatıldıktan sonra istenen dili ve kaynak temasını da yükleyecek.

Bu işlev, bir ekranı kullanıma hazırlamak için en yaygın olarak gereken programlama çabayı birleştirir. İşlev, gx_display_create (), gx_display_color_table_set, gx_display_font_table_set, gx_display_pixelmap_table_set, gx_system_language_table_set, gx_system_active_language_set, gx_system_scroll_appearance_set, gx_canvas_create ve gx_window_root_create işlevlerini, diğer bir deyişle uygulama programı için gerekli olacak şekilde çağırır.

### <a name="parameters"></a>Parametreler

- **görüntüle**: Studio proje dosyasındaki görüntüleme tanımlarına karşılık gelen görüntüleme tablosuna dizin.
- **sürücü**: görüntü sürücüsü başlatma işlevine yönelik işaretçi. Bu işlev, GX_DISPLAY denetim bloğunun dolaylı işlev işaretçilerini başlatmak için çağrılır ve gerekli tüm donanım ayarlarını gerçekleştirir.
- **dil**: ilk dil tablosu dizini
- **dil**: ilk tema dizini
- **root**: kök pencere adresinin döndürüleceği değişken işaretçisi veya GX_NULL.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı
- **GX_FAILURE**: (0x11) ekran başlatılamadı

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create the widget named “child_popup”, which is a child of the
   top-level screen “main_screen”. */

GX_WIDGET *menu_screen;

status = gx_studio_display_configure(MAIN_DISPLAY,
    my_driver_setup, LANGUAGE_ENGLISH, DEFAULT_THEME, GX_NULL);

/* If status == GX_SUCCESS the display was initialized, a canvas was
created for the display, a root window was created for the canvas, and
the requested language and theme have been installed.
*/
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_create
- gx_display_color_table_set
- gx_display_font_table_set
- gx_display_pixelmap_table_set
- gx_system_language_table_set
- gx_system_active_language_set
- gx_system_scroll_appearance_set
- gx_canvas_create
- gx_window_root_create

## <a name="gx_system_active_language_set"></a>gx_system_active_language_set

Etkin dili ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_system_active_language_set(GX_UBYTE language);
```

### <a name="description"></a>Açıklama

Bu hizmet geçerli dili ayarladı. Dil dizini, uygulama dizesi tablosundaki sütun sayısından küçük olmalıdır. Bu işlev, gx_display_active_language_set kullanım dışı bırakılmıştır. Tüm yeni uygulamalar gx_display_active_langauge_set kullanmalıdır.

### <a name="parameters"></a>Parametreler

- **dil**: dil dizini, kaynak üst bilgi dosyasında tanımlı.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) etkin Dili başarıyla ayarladı
- **GX_CALLER_ERROR**: * * (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: * * (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE**: * * (0x22) geçersiz dil dizini

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set active language and mark widget canvas as dirty. */
status = gx_system_active_language_set(ID_LANGUAGE_ENGLISH);

/* If status is GX_SUCCESS the active language has been assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_language_table_set
- gx_display_active_langauge_set
- gx_display_string_get

## <a name="gx_system_animation_get"></a>gx_system_animation_get

Sistem havuzundan animasyon denetim bloğu al

### <a name="prototype"></a>Prototype

```C
UINT gx_system_animation_get(GX_ANIMATION **animation);
```

### <a name="description"></a>Açıklama

Bu hizmet, gx_system bileşeni tarafından tutulan böyle bir denetim bloğu havuzundan bir animasyon denetim bloğu elde etmek için kullanılabilir. Animasyon denetim bloğu havuzu ve ilgili API hizmetleri yalnızca sabit GX_ANIMATION_POOL_SIZE 0 değeri ile tanımlandığında sağlanır. Bu değer için varsayılan ayar 6 ' dır, yani sistem animasyon denetim blok havuzu boyut GX_ANIMATION denetim bloğu içerir.

Bu API kullanılarak ayrılan bir animasyon denetim bloğu, animasyon tamamlanmaya çalışırsa otomatik olarak boş havuza döndürülür. Animasyon gx_animation_stop kullanılarak durdurulmuşsa veya bazı döndürülen bir hata nedeniyle başlatılamazsa, Animasyon denetim bloğunun, uygulama tarafından gx_system_animation_free kullanılarak boş havuza döndürülmesi gerekir.

### <a name="parameters"></a>Parametreler

- **animasyon**: GX_ANIMATION işaretçiyi alacak işaretçinin adresi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) animasyon denetim bloğu başarıyla alındı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz animasyon işaretçisi
- **GX_OUT_OF_ANIMATIONS**: (0x31) sistem animasyon havuzu tükendi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ANIMATION *animation;

UINT status = gx_system_animation_get(&animation);

if (status == GX_SUCCESS)
{
    gx_animation_start(animation, animation_info);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_animation_create
- gx_animation_start
- gx_animation_stop
- gx_system_animation_free

## <a name="gx_system_animation_free"></a>gx_system_animation_free

Sistem havuzuna bir animasyon denetim bloğu döndürme

### <a name="prototype"></a>Prototype

```C
UINT gx_system_animation_free(GX_ANIMATION *animation);
```

### <a name="description"></a>Açıklama

Bu hizmet, sistem havuzuna bir animasyon denetim bloğu döndürmek için kullanılabilir. Animasyon denetim bloğu havuzu ve ilgili API hizmetleri yalnızca sabit GX_ANIMATION_POOL_SIZE 0 değeri ile tanımlandığında sağlanır. Bu değer için varsayılan ayar 6 ' dır, yani sistem animasyon denetim blok havuzu boyut GX_ANIMATION denetim bloğu içerir.

Animasyon tamamlanmayı çalıştırıyorsa, gx_system_animation_get () kullanılarak ayrılmış bir animasyon denetim bloğu otomatik olarak boş havuza döndürülür. Boş havuza zaten döndürülen boş havuza bir animasyon denetim bloğu döndürme girişimi hiçbir etkiye sahip değildir.

Animasyon gx_animation_stop kullanılarak durdurulmuşsa veya bazı döndürülen bir hata nedeniyle başlatılamıyorsa, gx_system_animation_get () kullanılarak edinilen animasyon denetim bloğu, uygulama tarafından gx_system_animation_free () kullanılarak boş havuza döndürülmelidir.

Bir animasyon, ücretsiz havuza döndürülmeden önce boşta durumunda olmalıdır. Bir animasyon, başlatılmamışsa, durdurulduğunda veya tamamlanmaya çalıştırıldığında boşta durumundadır.

### <a name="parameters"></a>Parametreler

- **animasyon**: GX_ANIMATION denetim bloğuna yönelik işaretçi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) uccessfully çıkarılan animasyon bloğu
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz animasyon işaretçisi
- **GX_INVALID_ANIMATION**: (0x32) animasyon boşta değil veya sistem havuzundan ayrılmadı

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ANIMATION *animation;

UINT status = gx_system_animation_get(&animation);

if (status == GX_SUCCESS)
{
    status = gx_animation_start(animation, animation_info);

    if (status != GX_SUCCESS)
    {
        /* animation did not start, return it to the free pool */
        gx_system_animation_free(animation);
    }
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_animation_create
- gx_animation_start
- gx_animation_stop
- gx_system_animation_get

## <a name="gx_system_bidi_text_disable"></a>gx_system_bidi_text_disable

Dinamik iki yönlü metin desteğini devre dışı bırak

### <a name="prototype"></a>Prototype

```C
UINT gx_system_bidi_text_disable(VOID);
```

### <a name="description"></a>Açıklama

Bu hizmet, dinamik iki yönlü metin desteğini devre dışı bırakır. Bu hizmet, Gux kitaplığı oluşturulurken GX_DYNAMIC_BIDI_TEXT_SUPPORT tanımlanması gerekir ve yalnızca BiDi dize verilerinin çalışma zamanı yeniden sıralanması gerekliyse gereklidir. Çoğu uygulama, doğru reorderd BiDi metin dizelerini oluşturmak için Gux Studio 'Yu kullanır.

### <a name="parameters"></a>Parametreler

**Hiçbiri**

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) bidi metin desteğini başarıyla devre dışı bıraktı

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* GX_DYNAMIC_BIDI_TEXT_SUPPORT is defined. */

/* Diable bidi text support. */
status = gx_system_bidi_text_disable();

/* If status is GX_SUCCESS, bidi text support was disabled. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_bidi_text_enable

## <a name="gx_system_bidi_text_enable"></a>gx_system_bidi_text_enable

Dinamik bidi metin desteğini etkinleştir

### <a name="prototype"></a>Prototype

```C
UINT gx_system_bidi_text_enable(VOID);
```

### <a name="description"></a>Açıklama

Bu hizmet, dinamik iki yönlü metin desteğini sunar. Bu hizmet, Gux kitaplığı oluşturulurken GX_DYNAMIC_BIDI_TEXT_SUPPORT tanımlanması gerekir ve yalnızca BiDi dize verilerinin çalışma zamanı yeniden sıralanması gerekliyse gereklidir. Çoğu uygulama, doğru yeniden düzenlenen BiDi metin dizelerini oluşturmak için Gux Studio 'Yu kullanır.

### <a name="parameters"></a>Parametreler

**Hiçbiri**

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) bidi metin desteğini başarıyla etkinleştirdi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* GX_DYNAMIC_BIDI_TEXT_SUPPORT is defined. */

/* Enable bidi text support. */
status = gx_system_bidi_text_enable();

/* If status is GX_SUCCESS, bidi text support was enabled. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_bidi_text_disable

## <a name="gx_system_canvas_refresh"></a>gx_system_canvas_refresh

Tüm kirli canvaonları Yenile

### <a name="prototype"></a>Prototype

```C
UINT gx_system_canvas_refresh(VOID);
```

### <a name="description"></a>Açıklama

Bu hizmet, tüm kirli pencere öğelerinin ve canvalerin hemen yeniden çizilmesini zorlar. Bu hizmet normalde Gux sistem bileşeni tarafından dahili olarak çağrılır, ancak uygulama tarafından, bir sistem yeniden çizim işlemini zorlamak için çağrılabilir.

### <a name="parameters"></a>Parametreler

**Hiçbiri**

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) animasyon bloğunu başarıyla yayımladı
- **GX_INVALID_CANVAS**: (0x20) tuval oluşturulmadı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Force immediate redraw operation. */
status = gx_system_canvas_refresh();

/* If status is GX_SUCCESS, canvas has been redraw. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_dirty_mark"></a>gx_system_dirty_mark

Alanı kirli olarak işaretle

### <a name="prototype"></a>Prototype

```C
UINT gx_system_dirty_mark(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet, bu pencere öğesinin alanını kirli olarak işaretler. Bu, sistem olay işleme tamamlandığında yeniden çizim için pencere öğesini etkili bir şekilde kuyruğa alır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi**: pencere öğesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarıyla işaretlenmiş pencere öğesi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Mark widget “my_widget” as dirty. */
status = gx_system_dirty_mark(&my_widget);

/* If status is GX_SUCCESS the area associated
   with “my_widget” has been marked as dirty. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_dirty_partial_add"></a>gx_system_dirty_partial_add

Kısmi alanı kirli olarak işaretle

### <a name="prototype"></a>Prototype

```C
UINT gx_system_dirty_partial_add(
    GX_WIDGET *widget,
    GX_RECTANGLE *dirty_area);
```

### <a name="description"></a>Açıklama

Bu hizmet, bu pencere öğesinin kısmi alanını kirli olarak işaretler. Bu işlem, sistem olay işleme tamamlandığında Gux tuval yenileme işlemi tarafından yeniden çizim için pencere öğesini kuyruğa alır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi**: pencere öğesi denetim bloğu işaretçisi
- **dirty_area**: kirli olarak işaretlemek için pencere öğesinin kirli alanı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı kısmi kirli alan işareti
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_INVALID_SIZE**: (0x19) kirli alanın geçersiz boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Mark widget “my_widget” partial area as dirty. */

status = gx_system_dirty_partial_add(&my_widget,
    &partial_area);

/* If status is GX_SUCCESS the partial area “partial_area”
associated with “my_widget” has been marked as dirty. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_draw_context_get"></a>gx_system_draw_context_get

Çizim bağlamını al

### <a name="prototype"></a>Prototype

```C
UINT gx_system_draw_context_get(GX_DRAW_CONTEXT **current_context);
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli çizim bağlamına bir işaretçi döndürür.

### <a name="parameters"></a>Parametreler

- **current_context**: geçerli çizim bağlamı işaretçisi için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı geçerli bağlamı al
- **GX_PTR_ERROR**: 0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_DRAW_CONTEXT *current_context;

/* Get current drawing context. */

status = gx_system_draw_context_get(&current_context);

/* If status is GX_SUCCESS the current drawing context
   is contained in “current_context”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_event_fold"></a>gx_system_event_fold

Olayı gönder

### <a name="prototype"></a>Prototype

```C
UINT gx_system_event_fold(GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet, aynı türdeki bir olay için Gux olay kuyruğu arar. Aynı türde bir olay varsa, olay yükü yeni olayla eşleşecek şekilde güncelleştirilir. Eşleşen bir olay bulunmazsa, yeni olayı olay sırasının sonuna eklemek için gx_system_event_send işlevi çağırılır.

Bu işlev, birden çok PEN_DRAG olayına olay sırasının doldurulmasını engellemek için hızlı dokunmatik giriş sürücüleri tarafından yaygın olarak kullanılır. Bu işlev, aynı türde birden fazla olayın Gux olay kuyruğuna eklenmesini engellemek için uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **olay**: olay işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı olay gönderme
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_EVENT my_event;

memset(&my_event, 0, sizeof(GX_EVENT));

my_event.gx_event_type = GX_EVENT_PEN_DOWN;

my_event.gx_event_payload.gx_event_pointdata.gx_point_x = 100;
my_event.gx_event_payload.gx_event_pointdata.gx_point_y = 200;

/* Send “my_event” for processing. */
status = gx_system_event_fold(&my_event);

/* If status is GX_SUCCESS the event has been sent for processing. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_event_send"></a>gx_system_event_send

Olayı gönder

### <a name="prototype"></a>Prototype

```C
UINT gx_system_event_send(GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen olayı Gux sistem olay kuyruğuna gönderir. Yeni olay sıranın sonuna yerleştirilir.

### <a name="parameters"></a>Parametreler

- **olay**: olay işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı olay gönderme
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Send “new_event” for processing. */

GX_EVENT new_event;

new_event.gx_event_target = widget ->gx_widget_parent;
new_event.gx_event_type = MY_EVENT_TYPE;

/* Set optional param. */
new_event.gx_event_payload.xxxx = yyyy
new_event.gx_event_sender = widget->gx_widget_id;

/* Push the event to event pool. */
status = gx_system_event_send(&new_event);

/* If status is GX_SUCCESS the event has been sent for processing. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_focus_claim"></a>gx_system_focus_claim

Talep odaklı

### <a name="prototype"></a>Prototype

```C
UINT gx_system_focus_claim(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencere öğesi için odağı talep ediyor. Pencere öğesi daha önce odağa sahip değilse, GX_EVENT_FOCUS_GAINED bir olay alır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi**: odağı talep etmek için pencere öğesi denetim bloğunun işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı odak talebi
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_NO_CHANGE**: (0x08) zaten odağa sahip pencere öğesi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_INVALID_WIDGET**: (0X12 pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Claim focus for widget “my_widget”. */
status = gx_system_claim_focus(&my_widget);

/* If status is GX_SUCCESS the focus has been claimed for
   “my_widget”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_initialize"></a>gx_system_initialize

GUX 'i Başlat

### <a name="prototype"></a>Prototype

```C
UINT gx_system_initialize(VOID);
```

### <a name="description"></a>Açıklama

Bu hizmet, GUıDX 'i başlatır. Bu hizmetin diğer bir Gux API hizmetinden önce çağrılması ve sistem başlangıcında yalnızca bir kez çağrılması gerekir.

### <a name="parameters"></a>Parametreler

- **Hiçbiri**

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı sistem başlatması
- **GX_SYSTEM_ERROR**: (0xFE) geçersiz GX_EVENT denetim bloğu boyutu veya olay kuyruğu/Mutex/iş parçacığı oluşturma başarısız oldu.
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Initialize GUIX. */
status = gx_system_initialize();

/* If status is GX_SUCCESS, GUIX has been initialized. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_language_table_get"></a>gx_system_language_table_get

Etkin dil tablosunu al

### <a name="prototype"></a>Prototype

```C
UINT gx_system_language_table_get( 
    GX_CHAR ****language_table,
    GX_UBYTE *languages_count, 
    UINT *string_count);
```

### <a name="description"></a>Açıklama

Bu hizmet, etkin dil tablosunu alır. Bu işlev, gx_display_language_table_get yararına kullanım dışıdır. Tüm yeni uygulamalar gx_display_language_table_get kullanmalıdır.

### <a name="parameters"></a>Parametreler

- **language_table**: dil tablosunun döndürdüğü işaretçinin adresi.
- **languages_count**: tablo sütunlarının döndürülme değişkeninin adresi.
- **string_count**: tablo satırları döndüren işaretçinin adresi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) etkin dil tablosu başarıyla alındı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR ***language_table;

GX_UBYTE language_count;

UINT string_count;

/* Retrieve the language table */

status = gx_system_language_table_get(&language_table,
    &language_count, &string_count);
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_language_table_get
- gx_display_language_table_set

## <a name="gx_system_language_table_set"></a>gx_system_language_table_set

Etkin dil tablosu ata

### <a name="prototype"></a>Prototype

```C
UINT gx_system_language_table_set(
    GX_CHAR ***language_table,
    GX_UBYTE languages_count, 
    UINT string_count);
```

### <a name="description"></a>Açıklama

Bu hizmet, etkin dil tablosunu yüklüyor. Bu işlev, gx_display_language_table_set kullanım dışı bırakılmıştır. Tüm yeni uygulamalar gx_display_language_table_set kullanmalıdır.

### <a name="parameters"></a>Parametreler

- **language_table**: dil tablosu işaretçisi.
- **languages_count**: tablodaki dillerin sayısı.
- **string_count**: dize tablosu satır sayısı.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) dil tablosu başarıyla ayarlandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Retrieve the language table */

status = gx_system_language_table_set(language_table,
    language_count, string_count);
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_language_table_set
- gx_display_language_table_get
- gx_display_active_language_set

## <a name="gx_system_memory_allocator_set"></a>gx_system_memory_allocator_set

Bellek ayırma, serbest ayırma için işlevler atama

### <a name="prototype"></a>Prototype

```C
UINT gx_system_memory_allocator_set(VOID *(allocate)(ULONG size),
    VOID(*release)(VOID *));
```

### <a name="description"></a>Açıklama

Bu hizmet, dinamik bellek ayırma ve ayırmayı ayırma için uygulama tarafından sağlanan geri çağırma işlevini atar.

Uygulama için dinamik bellek ayırma kullanan bir Gux hizmeti gerekmiyorsa, bu hizmetin çağrılması gerekmez.

Kullanılıyorsa, bu hizmetin, Gux hizmet işaretçilerini ve dinamik bellek ayırmayı kullanması gereken Gux hizmetinden önce, gx_system_initialize () sonra çağrılması gerekir.

Çalışma zamanı belleği ayırmayı ve ayırmayı kaldırma hizmetini gerektiren GUıDX Hizmetleri şunları içerir:

- Dış depolamadan Gux çalışma zamanı ortamına ikili kaynakları yükleme.
- Yazılım çalışma zamanı JPEG görüntü kod çözücüsü.
- Yazılım çalışma zamanı PNG resmi kod çözücüsü.
- GX_STYLE_TEXT_COPY ile metin pencere öğeleri kullanma.
- Çalışma zamanı Pikselleştirme yeniden boyutlandırma ve döndürme yardımcı programı işlevleri.
- Çalışma zamanı ekranı ve pencere öğesi denetim bloğu ayırması.

### <a name="parameters"></a>Parametreler

- **ayırıcı**: bellek ayırıcı işlevi
- **yayın**: bellek boş işlevi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) bellek ayırma işlevi başarıyla atandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

Aşağıdaki örnek, bir ThreadX Byte havuzunu bir threadsafe dinamik bellek ayırma ve bellek ayırma hizmeti uygulamak için kullanır.

```C
TX_BYTE_POOL memory_pool;

#define SCRATCHPAD_SIZE (1024 * 4)

ULONG scratchpad[SCRATCHPAD_SIZE];

/* define memory allocation service */

VOID *memory_allocate(ULONG size)
{
    VOID *memptr;

    if (tx_byte_allocate(&memory_pool, &memptr, size, TX_NO_WAIT) == TX_SUCCESS)
    {
        return memptr;
    }
    return NULL;
}

/* define memory de-allocation service */
void memory_free(VOID *mem)
{
    tx_byte_release(mem);
}

/* create byte pool and install our dynamic memory services with GUIX
*/

VOID tx_application_define(void *first_unused_memory)
{
    /* create byte pool for GUIX to use */
    tx_byte_pool_create(&memory_pool, "scratchpad", scratchpad,
        SCRATCHPAD_SIZE * sizeof(ULONG));

    guix_setup();

    /* install our memory allocator and de-allocator */
    gx_system_memory_allocator_set(memory_allocate, memory_free);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_pen_configure"></a>gx_system_pen_configure

Kalem yapılandırmasını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_system_pen_configure(GX_PEN_CONFIGURATION *pen_configuration);
```

### <a name="description"></a>Açıklama

Bu hizmet, GX_EVENT_FLICK olay türlerinin oluşturulmasını tetiklemek için kullanılan kalem hızını ve uzaklık parametrelerini denetlemek için kalem yapılandırmasını ayarlar.

GX_PEN_CONFIGURATION gx_pen_configuration_min_drag_dist üyesi sabit bir nokta veri türüdür ve INT 'den GX_FIXED_VAL 'e dönüştürmek için GX_FIXED_VAL_MAKE (değer) kullanmanız gerekir. Örneğin, değer başına en az 0,5 piksel bir sürükleme değeri ayarlamak istiyorsanız gx_pen_configuration_min_drag_dist olarak ayarlamanız gerekir `GX_FIXED_VAL_MAKE(1) / 2` .

GUX yayınları 5.4.0 ve daha eski sürümlerde, GX_PEN_CONFIGURATION gx_pen_configuration_min_drag_dist üyesi, GX_FIXED_VAL türü yerine (INT << 8) türüdür. 5.4.0 Version Gux kitaplığı olan projeniz bu API kullanıyorsa, Gux kitaplığı oluştururken min_drag_dist parametresini veya GUIX_5_4_0_COMPATIBILITY #define değiştirmeniz gerekir.

### <a name="parameters"></a>Parametreler

- **pen_configuration** Kalem yapılandırma yapısına yönelik işaretçi. **Ek ı** GX_PEN_CONFIGURATION yapısına tanım içeriyor

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) kalem yapılandırması başarıyla ayarlandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define pen configuration, set minimum drag distance to 0.5 pixel
per tick, maximum pen speed to 10 ticks. That means GUIX will trigger
a vertical or horizontal flick event if the drag time is smaller than
10 ticks and the drag distance is bigger than 0.5 * drag_ticks. */

GX_PEN_CONFIGURATION pen_configuration;

#if defined(GUIX_5_4_0_COMPATIBILITY)
Pen_configuration.gx_pen_configuration_min_drag_dist = (1 << 8)/ 2;
#else
pen_configuration.gx_pen_configuration_min_drag_dist = GX_FIXED_VAL_MAKE(1) / 2;
#endif

pen_configuration.gx_pen_configuration_max_pen_speed_ticks = 10;

/* Set the pen configuration. */
status = gx_system_pen_configure(&pen_configuration);

/* If status is GX_SUCCESS the touch configure has been set. */
```

## <a name="gx_system_screen_stack_create"></a>gx_system_screen_stack_create

Sistem ekran yığınını oluşturma ve başlatma

### <a name="prototype"></a>Prototype

```C
UINT gx_system_screen_stack_create(
    GX_WIDGET **memory, 
    INT size);
```

### <a name="description"></a>Açıklama

Bu hizmet, sistem ekran yığını için kullanılacak bir bellek havuzunu tanımlar. Sistem ekran yığını uygulama ekran akışı görünümünü yönetmek için uygulama tarafından kullanılabilen isteğe bağlı bir özelliktir.

Uygulama, ekran yığını hizmetlerini kullanmayı amaçladığında, önce ekran yığını bellek bölgesini ayarlamak için gx_system_screen_stack_create işlevin çağrılması gerekir.

### <a name="parameters"></a>Parametreler

- **bellek**: ayrılmış bellek bloğuna yönelik işaretçi.
- **Boyut**: ayrılan bellek bloğunun bayt cinsinden boyutu.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarıyla oluşturuldu
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
#define SCREEN_STACK_DEPTH 8
GX_WIDGET *screen_stack[SCREEN_STACK_DEPTH * 2];

UINT status;

/* Get the scrollbar appearance. */

status = gx_system_screen_stack_create(screen_stack,
    sizeof(GX_WIDGET *) * SCREEN_STACK_DEPTH * 2);

/* If status is GX_SUCCESS the system screen stack is initialized
and ready for use. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_screen_stack_get
- gx_system_screen_stack_pop
- gx_system_screen_stack_push
- gx_system_screen_stack_reset

## <a name="gx_system_screen_stack_get"></a>gx_system_screen_stack_get

En üstteki ekran yığını işaretçilerini aç

### <a name="prototype"></a>Prototype

```C
UINT gx_system_screen_stack_get(
    GX_WIDGET **popped_parent,
    GX_WIDGET **popped_screen);
```

### <a name="description"></a>Açıklama

Bu işlev en üstteki ekran yığını işaretçilerini ve bu işaretçileri çağırıcı için döndürür. Bu işlev, pomış ekranın önceki üst öğeye otomatik olarak yeniden iliştirilmesi için gx_system_screen_stack_pop () öğesinden farklıdır. Bunun yerine, işaretçiler yığından alınır ve çağrıyı yapana döndürülür. Bu, çağıranın döndürülen ekranı eklemek veya atmak için istendiği gibi.

### <a name="parameters"></a>Parametreler

- **popped_parent**: üst pencere öğesi işaretçisinin depolandığı konum.
- **popped_screen**: pomış ekran işaretçisinin depolandığı konum.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) ekran yığını işaretçilerinin başarıyla alımı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_FAILURE**: (0x10) geçersiz veya boş ekran yığını

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT status;

GX_WIDGET *parent_screen;

GX_WIDGET *popped_screen;

/* Pop a screen stack entry. */
status = gx_system_screen_stack_get(&parent_screen, &popped_screen);

/* If status is GX_SUCCESS, parent_screen and
popped_screen hold the topmost screen stack pointers. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_screen_stack_create
- gx_system_screen_stack_pop
- gx_system_screen_stack_push
- gx_system_screen_stack_reset

## <a name="gx_system_screen_stack_pop"></a>gx_system_screen_stack_pop

Sistem ekran yığınından en üstteki girişi aç

### <a name="prototype"></a>Prototype

```C
UINT gx_system_screen_stack_pop();
```

### <a name="description"></a>Açıklama

Bu işlev, ekran yığınında en üstteki girdiyi otomatik olarak ekler ve basamaklı ekranı otomatik olarak posolanan üst pencere öğesine ekler.

### <a name="parameters"></a>Parametreler

**yok**

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) ekran yığını işaretçilerinin başarıyla alımı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_FAILURE**: (0x10) geçersiz veya boş ekran yığını

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT status;

/* Pop a screen stack entry. */
status = gx_system_screen_stack_pop();

/* If status is GX_SUCCESS, the topmost screen stack entry has been
popped from the stack and re-attached to the previous parent. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_screen_stack_get
- gx_system_screen_stack_create
- gx_system_screen_stack_push
- gx_system_screen_stack_reset

## <a name="gx_system_screen_stack_push"></a>gx_system_screen_stack_push

Ekran yığınına bir pencere öğesi ve üst işaretçi gönder

### <a name="prototype"></a>Prototype

```C
UINT gx_system_screen_stack_push(GX_WIDGET *screen)
```

### <a name="description"></a>Açıklama

Bu hizmet, genellikle üst düzey bir ekran olan belirtilen pencere öğesine, ekran yığınına bir işaretçi koyar. Pencere öğesinin bir üst öğesi varsa üst öğeden ayrılır. Üst pencere öğesi işaretçisi de ekran yığınına gönderilir. Üst pencere öğesi NULL olabilir, yani görünmeyen veya herhangi bir üst öğeye bağlı olmayan bir ekran, ekran yığınına itilmiş olabilir. Üst öğeye sahip olmayan bir pencere öğesi, ekran yığınına itilmiş ise, screen_stack_get () API 'sinin, screen_stack_pop () API 'sini kullanmak yerine, önceki üst öğeye yeniden iliştirmeye çalışır.

### <a name="parameters"></a>Parametreler

- **ekran**: ekran yığınına itilmiş pencere öğesinin işaretçisi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) kaydırma çubuğu görünümü başarıyla al
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Get the scrollbar appearance. */
status = gx_system_screen_stack_push(window);

/* If status is GX_SUCCESS, the widget pointed to by “window” has
been pushed to the screen stack, along with the widget’s parent
ponter. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_screen_stack_get
- gx_system_screen_stack_pop
- gx_system_screen_stack_create
- gx_system_screen_stack_reset

## <a name="gx_system_screen_stack_reset"></a>gx_system_screen_stack_reset

Sistem ekran yığınını sıfırlama

### <a name="prototype"></a>Prototype

```C
UINT gx_system_screen_stack_reset();
```

### <a name="description"></a>Açıklama

Bu işlev, sistem ekran yığınından tüm girdileri kaldırır. Yığından oluşan ekranlarda, GUıDX Studio tarafından ayrılan dinamik olarak ayrılmış denetim blokları varsa, bu denetim blokları için bellek serbest bırakılır.

### <a name="parameters"></a>Parametreler

**yok**

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) kaydırma çubuğu görünümü başarıyla al
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Get the scrollbar appearance. */
status = gx_system_screen_stack_reset();

/* If status is GX_SUCCESS the system screen stack has been cleared
of entries. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_screen_stack_get
- gx_system_screen_stack_pop
- gx_system_screen_stack_push
- gx_system_screen_stack_create

## <a name="gx_system_scroll_appearance_get"></a>gx_system_scroll_appearance_get

Kaydırma görünümü al

### <a name="prototype"></a>Prototype

```C
UINT gx_system_scroll_appearance_get(
    ULONG style,
    GX_SCROLLBAR_APPEARANCE *return_appearance);
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırma çubuğu görünümünü alır.

### <a name="parameters"></a>Parametreler

- **Stil**: kaydırma çubuğu stili: `GX_SCROLLBAR_HORIZONTAL` veya `GX_SCROLLBAR_VERTICAL`
- **return_appearance**: görünüm için hedefe yönelik işaretçi. **Ek ı** GX_SCROLLBAR_APPERANCE tanım içeriyor

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) kaydırma çubuğu görünümü başarıyla al
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_SCROLLBAR_APPEARANCE my_appearance;

/* Get the scrollbar appearance. */

status = gx_system_scroll_appearance_get(style, &my_appearance);

/* If status is GX_SUCCESS “my_appearance” now contains the scroll
appearance. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_set
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_scroll_appearance_set"></a>gx_system_scroll_appearance_set

Kaydırma görünümünü ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_system_scroll_appearance_set(
    ULONG style,
    GX_SCROLLBAR_APPEARANCE *appearance);
```

### <a name="description"></a>Açıklama

Bu hizmet varsayılan kaydırma görünümünü ayarlar. Bir kaydırma oluşturulduğunda, uygulama özel bir sürüm sunmadığı takdirde bu görünüm yapısı kullanılır.

### <a name="parameters"></a>Parametreler

- **Stil**: kaydırma stili `GX_SCROLLBAR_HORIZONTAL` veya `GX_SCROLLBAR_VERTICAL`
- **Görünüm**: farklı ScrollBar görünümü öznitelikleriyle başlatılan görünüm yapısına yönelik işaretçi. GX_SCROLLBAR_APPEARANCE yapısının tanımı için **Ek I** ' ye başvurun.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) kaydırma görünümü kümesi başarıyla ayarlandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_SCROLLBAR_APPEARANCE my_appearance;

memset(&my_appearance, 0, sizeof(GX_SCROLLBAR_APPEARANCE));

my_appearance.gx_scroll_width = 20;
my_appearance.gx_scroll_thumb_width = 18;

my_appearance.gx_scroll_thumb_color = GX_COLOR_ID_SCROLL_BUTTON;
my_appearance.gx_scroll_thumb_border_color = GX_COLOR_ID_SCROLL_BUTTON;
my_appearance.gx_scroll_button_color = GX_COLOR_ID_SCROLL_BUTTON;
my_appearance.gx_scroll_thumb_travel_min = 20;
my_appearance.gx_scroll_thumb_travel_max = 20;
my_appearance.gx_scroll_thumb_border_style = GX_STYLE_BORDER_THIN;

/* Set the scroll appearance. */

status = gx_system_scroll_appearance_set(GX_SCROLLBAR_VERTICAL, &my_appearance);

/* If status is GX_SUCCESS the scroll appearance has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_start"></a>gx_system_start

GUX 'i Başlat

### <a name="prototype"></a>Prototype

```C
UINT gx_system_start(VOID);
```

### <a name="description"></a>Açıklama

Bu hizmet, GUıDX işlemesini başlatır. Normal koşullarda, bu işlev hiçbir şekilde döndürmez, bunun yerine Gux olay kuyruğunu işlemeye başlar. GUX olay kuyruğu boş olduğunda, bu hizmet, yeni olaylar Gux olay kuyruğuna gelene kadar çağıran iş parçacığını askıya alır.

### <a name="parameters"></a>Parametreler

- **Hiçbiri**

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı sistem başlatması
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Start GUIX. */
status = gx_system_start();

/* If status is GX_SUCCESS . GUIX has been started. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_string_get"></a>gx_system_string_get

Dizeyi al

### <a name="prototype"></a>Prototype

```C
UINT gx_system_string_get(
    GX_RESOURCE_ID string_id,
    GX_CHAR **return_string);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen kaynak KIMLIĞI için dizeyi, ilk tanımlanan görüntüyü ve şu anda etkin dili kullanarak alır. Bu işlev, gx_display_string_get kullanım dışı bırakılmıştır. Tüm yeni uygulamalar gx_display_string_get kullanmalıdır.

### <a name="parameters"></a>Parametreler

- **string_id**: DIZE kaynak kimliği
- **return_string**: dize hedefi işaretçisine yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı dize al
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR (0x07)**: geçersiz işaretçi
- **GX_INVALID_RESOURCE_ID**: (0x33) GEÇERSIZ kaynak kimliği

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Get the string associated with MY_STRING_ID. */

status = gx_system_string_get(MY_STRING_RESOURCE_ID, &my_string);

/* If status is GX_SUCCESS the string is contained in “my_string”.
*/
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_string_get
- gx_display_string_table_get
- gx_display_language_table_set

## <a name="gx_system_string_table_get"></a>gx_system_string_table_get

Dize tablosunu alır

### <a name="prototype"></a>Prototype

```C
UINT gx_system_string_table_get(
    GX_UBYTE language,
    GX_CHAR ***string_table,
    UINT *get_size);
```

### <a name="description"></a>Açıklama

Bu hizmet, istenen dilin dize tablosunu ilk ekranda alır. Bu işlev, gx_display_string_table_get kullanım dışı bırakılmıştır. Tüm yeni uygulamalar gx_display_string_table_get kullanmalıdır.

### <a name="parameters"></a>Parametreler

- **dil**: dil dizini
- **string_table**: dize tablo işaretçisinin depolama alanı işaretçisi veya çağıranın dize tablosuna yönelik işaretçiyi ALMASı gerekmiyorsa null.
- **get_size**: dize tablosundaki dize sayısı için depolama alanı işaretçisi veya çağıranın dize tablosundaki dize sayısını ALMASı gerekmiyorsa null.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı dize tablosu al
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Get the string table. */

CHAR **my_string_table; UINT table_size;

status = gx_system_string_table_get(LANGUAGE_ID_ENGLISH,
    &my_string_table, &table_size);

/* If status is GX_SUCCESS . the pointer to the string table has
been obtained. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_string_table_get
- gx_display_string_get
- gx_display_active_language_set
- gx_display_language_table_set

## <a name="gx_system_string_width_get"></a>gx_system_string_width_get

Dize genişliğini al (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_system_string_width_get(
    GX_FONT *font, GX_CHAR *string,
    INT string_length,
    GX_VALUE *return_width);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_system_string_width_get_ext () kullanımı için kullanım dışıdır.

Bu hizmet, belirtilen yazı tipini kullanarak sağlanan dizenin piksel cinsinden görüntüleme genişliğini hesaplar. String_length parametresi >= 0 ise, hesaplamaya yalnızca karakter istek sayısı dahil edilir. String_length parametresi-1 ise, hesaplamada, NULL sonlandırıcıya kadar olan tüm dize kullanılır.

### <a name="parameters"></a>Parametreler

- **yazı tipi**: dizenin yazı tipine yönelik işaretçi
- **dize**: dize işaretçisi
- **string_length**: dize uzunluğu
- **return_width**: dizenin genişliği için hedef

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı dize genişliği al
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_INVALID_FONT**: (0x16) geçersiz Yazı tipi
- **GX_INVALID_STRING_LENGTH**: (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Get the string width of “my_string”. */

status = gx_system_string_width_get(&my_font, &my_string,
    strlen(my_string), &my_width);

/* If status is GX_SUCCESS . “my_width” contains the string width.
*/
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_string_width_get_ext

## <a name="gx_system_string_width_get_ext"></a>gx_system_string_width_get_ext

Dize genişliğini al

### <a name="prototype"></a>Prototype

```C
UINT gx_system_string_width_get_ext(
    GX_FONT *font,
    GX_STRING *string,
    GX_VALUE *return_width);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen yazı tipini kullanarak sağlanan dizenin piksel cinsinden görüntüleme genişliğini hesaplar.

### <a name="parameters"></a>Parametreler

- **yazı tipi**: dizenin yazı tipine yönelik işaretçi
- **dize**: dize işaretçisi
- **return_width**: dizenin genişliği için hedef

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı dize genişliği al
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR**: 0x11) bu işlevin çağıranı geçersiz
- **GX_INVALID_FONT**: (0x16) geçersiz Yazı tipi
- **GX_INVALID_STRING_LENGTH**: (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING my_string; my_string.gx_string_ptr = “Monday”;

my_string.gx_string_length = strlen(my_string.gx_string_ptr);

/* Get the string width of “my_string”. */

status = gx_system_string_width_get_ext(&my_font,
    &my_string, &my_width);

/* If status is GX_SUCCESS . “my_width” contains the string width.
*/
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_event_fold
- gx_system_focus_claim
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_timer_start"></a>gx_system_timer_start

Zamanlayıcıyı Başlat

### <a name="prototype"></a>Prototype

```C
UINT gx_system_timer_start(
    GX_WIDGET *owner, 
    UINT timer_id,
    UINT initial_ticks,
    UINT reschedule_ticks);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencere öğesi için bir süreölçer başlatır. Sabit GX_MAX_ACTIVE_TIMERS desteklenen en fazla etkin Zamanlayıcı sayısını tanımladı. Bu değer için varsayılan ayar 32 ' dir.

### <a name="parameters"></a>Parametreler

- **sahip**: pencere öğesi denetim bloğu işaretçisi
- **timer_id**: zamanlayıcının kimliği
- **initial_ticks**: ilk süre sonu işaretleri
- **reschedule_ticks**: düzenli süre sonu işaretleri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı süreölçer başlangıcı
- **GX_OUT_OF_TIMERS**: (0x04) daha fazla Zamanlayıcı yok
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE**: (0X22) Zamanlayıcı değerleri geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Start a periodic timer for the widget “my_widget”. */
status = gx_system_timer_start(&my_widget, MY_TIMER_ID, 10, 20);

/* If status is GX_SUCCESS . the timer for “my_widget” has been
started. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_event_fold
- gx_system_focus_claim
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_timer_stop"></a>gx_system_timer_stop

Zamanlayıcıyı durdur

### <a name="prototype"></a>Prototype

```C
UINT gx_system_timer_stop(
    GW_WIDGET *owner, 
    UINT timer_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, çağırma pencere öğesiyle ilişkili belirtilen timer_id zamanlayıcıyı durduruyor. Belirli bir pencere öğesine bağlı tüm zamanlayıcıları durdurmak için, uygulama 0 ' ın timer_id değerini geçirebilir.

### <a name="parameters"></a>Parametreler

- **sahip**: pencere öğesi denetim bloğu işaretçisi
- **timer_id**: Zamanlayıcı kimliği veya tüm zamanlayıcılar için 0

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı süreölçer durağı
- **GX_NOT_FOUND**: (0x09) Zamanlayıcı kimliği bulunamadı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Stop the periodic timer for the widget “my_widget”. */
status = gx_system_timer_stop(&my_widget, MY_TIMER_ID);

/* If status is GX_SUCCESS . the timer for “my_widget” has been
stopped. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_event_fold
- gx_system_focus_claim
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_pen_configure
- gx_system_version_string_get
- gx_system_widget_find

## <a name="gx_system_version_string_get"></a>gx_system_version_string_get

GUX kitaplığı sürüm dizesini al (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_system_version_string_get(GX_CHAR **version);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_system_version_string_get_ext () kullanımı için kullanım dışıdır.

Bu hizmet, GUıDX kitaplığı sürüm dizesini alır.

### <a name="parameters"></a>Parametreler

- **Sürüm**: Return dize değeri döndürür.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) sürüm dizesi başarıyla alındı
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR *version;

/* get the library version string. */

status = gx_system_verrsion_string_get(&version);
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_version_string_get_ext ()

## <a name="gx_system_version_string_get_ext"></a>gx_system_version_string_get_ext

GUX kitaplığı sürüm dizesini al

### <a name="prototype"></a>Prototype

```C
UINT gx_system_version_string_get(GX_STRING *version);
```

### <a name="description"></a>Açıklama

Bu hizmet, GUıDX kitaplığı sürüm dizesini alır.

### <a name="parameters"></a>Parametreler

- **Sürüm**: Return dize değeri döndürür.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) sürüm dizesi başarıyla alındı
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_STRING_LENGTH**: (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING version;

/* get the library version string. */

status = gx_system_version_string_get_ext(&version);
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_widget_find

## <a name="gx_system_widget_find"></a>gx_system_widget_find

Pencere öğesi bul

### <a name="prototype"></a>Prototype

```C
UINT gx_system_widget_find(
    USHORT widget_id,
    INT search_level, 
    GX_WIDGET **return_search_result);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencere öğesi KIMLIĞINI arar. Gx_widget_find () aksine, bu işlev sistemde tanımlanan tüm kök pencerelerin alt öğelerini arar, yani bu, tüm görünür pencere öğelerinin ayrıntılı bir aradır. Aradığınız pencere öğesinin üst öğesini biliyorsanız bunun yerine gx_widget_find () kullanın.

### <a name="parameters"></a>Parametreler

- **widget_id**: aranacak pencere öğesi kimliği
- **search_level**: alt pencere öğelerinin aranacağı özyinelemeli iç içe geçme düzeyini tanımlar. Bu değer 0 ise, her bir kök pencerenin yalnızca anlık alt öğeleri aranır. Bu değer GX_SEARCH_DEPTH_INFINITE ise, işlev, istenen pencere öğesi KIMLIĞINI arayan tüm alt öğeleri arar. Başka herhangi bir değer > 0 ' da, arama düzeyi bu işlevin istenen pencere öğesi KIMLIĞI için ne kadar fazla arama yapılacağını tanımlar.
- **return_search_result**: pencere öğesi için hedef işaretçisi bulundu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı pencere öğesi araması
- **GX_NOT_FOUND**: (0x09) pencere öğesi kimliği bulunamadı
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Search recursively from the top level widget for the widget with
ID of MY_WIDGET_ID. */

status = gx_system_widget_find(MY_WIDGET_ID,
    GX_SEARCH_DEPTH_INFINITE,
    &my_widget);

/* If status is GX_SUCCESS . the search was successful and
“my_widget” contains the pointer to the widget. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_system_active_language_set
- gx_system_canvas_refresh
- gx_system_dirty_mark
- gx_system_dirty_partial_add
- gx_system_draw_context_get
- gx_system_event_fold
- gx_system_event_send
- gx_system_focus_claim
- gx_system_initialize
- gx_system_initialize
- gx_system_language_table_get
- gx_system_language_table_set
- gx_system_memory_allocator_set
- gx_system_scroll_appearance_get
- gx_system_scroll_appearance_get
- gx_system_start
- gx_system_string_get
- gx_system_string_table_get
- gx_system_string_width_get
- gx_system_timer_start
- gx_system_timer_stop
- gx_system_pen_configure
- gx_system_version_string_get

## <a name="gx_text_button_create"></a>gx_text_button_create

Metin oluştur düğmesi

### <a name="prototype"></a>Prototype

```C
UINT gx_text_button_create(
    GX_TEXT_BUTTON *text_button,
    GX_CONST GX_CHAR *name, 
    GX_WIDGET *parent,
    GX_RESOURCE_ID text_id, 
    ULONG style,
    USHORT text_button_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir metin düğmesi pencere öğesi oluşturur.

GX_TEXT_BUTTON GX_BUTTON türetilir ve tüm gx_button API hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **text_button**: metin düğmesi denetim bloğuna işaretçi
- **ad**: metin düğmesinin mantıksal adı
- **Parent**: düğmenin üst pencere öğesine işaretçi
- **text_id**: METNIN kaynak kimliği
- **Stil**: metin düğmesi stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **text_button_id**: metin düğmesinin uygulama tanımlı kimliği
- **Boyut**: düğmenin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı metin düğmesi oluştur
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED**: (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE**: (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET**: (0x12) üst pencere öğesi geçerli değil


### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_TEXT_BUTTON my_text_button;

GX_RECTANGLE size;

/* Define widget size. */

gx_utility_rectangle_define(&size, 0, 0, 100, 100);

/* Create text button “my_text_button”. */

status = gx_text_button_create(&my_text_button, "my text button",
    &my_parent_window, MY_TEXT_RESOURCE_ID,
    GX_STYLE_BUTTON_TOGGLE, MY_TEXT_BUTTON_ID, &size);

/* If status is GX_SUCCESS, the text button “my_text_button” was
created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_color_set
- gx_text_button_draw
- gx_text_button_event_process
- gx_text_button_font_set
- gx_text_button_text_get
- gx_text_button_text_set
- gx_text_button_text_id_set

## <a name="gx_text_button_draw"></a>gx_text_button_draw

Metin çiz düğmesi

### <a name="prototype"></a>Prototype

```C
VOID gx_text_button_draw(GX_TEXT_BUTTON *button);
```

### <a name="description"></a>Açıklama

Bu hizmet metin düğmesini çizer. Bu hizmet, genellikle tuval yenilemesi sırasında dahili olarak çağrılır, ancak özel metin düğmesi çizim işlevlerinden de çağrılabilir.

### <a name="parameters"></a>Parametreler

- **düğme**: metin düğmesi denetim bloğuna işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom text button draw function. */

VOID my_text_button_draw(GX_TEXT_BUTTON *text_button)
{
    /* Call default text button draw. */
    gx_text_button_draw(text_button);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_event_process
- gx_text_button_color_set
- gx_text_button_font_set
- gx_text_button_text_get
- gx_text_button_text_set
- gx_text_button_text_id_set

## <a name="gx_text_button_event_process"></a>gx_text_button_event_process


İşlem metni düğmesi olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_text_button_event_process(GX_TEXT_BUTTON *text_button, GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen metin düğmesi için bir olayı işler. Bu hizmet, özel metin düğmesi olay işleme işlevleri tarafından varsayılan olay işleyicisi olarak çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **text_button** Metin düğmesi denetim bloğuna işaretçi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı metin düğmesi olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic text button event processing as part of custom event processing function. */

UINT custom_text_button_event_process(GX_TEXT_BUTTON *text_button, GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;

    default:
        /* Pass all other events to the default text button event processing */
        status = gx_text_button_event_process(wheel, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_draw
- gx_text_button_color_set
- gx_text_button_font_set
- gx_text_button_text_get
- gx_text_button_text_set
- gx_text_button_text_id_set

## <a name="gx_text_button_font_set"></a>gx_text_button_font_set

Yazı tipini metin düğmesine ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_text_button_font_set(
    GX_TEXT_BUTTON *button,
    GX_RESOURCE_ID font_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen düğmeye bir yazı tipi atar.

### <a name="parameters"></a>Parametreler

- **düğme**: metin düğmesi denetim bloğuna işaretçi
- **font_id**: yazı tipi ıNFO kaynak kimliği

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) yazı tipi başarıyla ayarlandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the text button with the font ID MY_FONT. */
status = gx_text_button_font_set(&my_text_button, MY_FONT);

/* If status is GX_SUCCESS, the font of the text button
“my_text_button” was set to MY_FONT. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create
- gx_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_draw
- gx_text_button_event_process
- gx_text_button_color_set
- gx_text_button_text_get
- gx_text_button_text_set
- gx_text_button_text_id_set

## <a name="gx_text_button_text_color_set"></a>gx_text_button_text_color_set

Metin düğmesi rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_text_button_text_color_set(
    GX_TEXT_BUTTON *text_button,
    GX_RESOURCE_ID normal_text_color_id,
    GX_RESOURCE_ID selected_text_color_id,
    GX_RESOURCE_ID disabled_text_color_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin düğmesinin rengini ayarlar.

### <a name="parameters"></a>Parametreler

- **text_button**: metin düğmesi denetim bloğuna işaretçi
- **normal_text_color_id**: normal METNIN kaynak kimliği. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **selected_text_color_id**: seçili METNIN kaynak kimliği. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **disabled_text_color_id**: devre dışı bırakılan metnin renk kaynak kimliği. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı metin düğmesi renk kümesi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the color of the text button “my_text_button”. */
status = gx_text_button_text_color_set(&my_text_button,
    GX_COLOR_ID_NORMAL_TEXT,
    GX_COLOR_ID_SELECTED_TEXT,
    GX_COLOR_ID_DISABLED_TEXT);

/* If status is GX_SUCCESS, the text color of “my_text_button” was
set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create, x_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_draw
- gx_text_button_event_process
- gx_text_button_font_set
- gx_text_button_text_get
- gx_text_button_text_set
- gx_text_button_text_id_set

## <a name="gx_text_button_text_draw"></a>gx_text_button_text_draw

Düğme metni çizmek için destek işlevi

### <a name="prototype"></a>Prototype

```C
VOID gx_text_button_text_draw(GX_TEXT_BUTTON *text_button);
```

### <a name="description"></a>Açıklama

Bu destek işlevi bir metin düğmesinin metin bölümünü çizer. Bu işlev, gx_text_button_draw tarafından dahili olarak çağrılır ve özel bir düğme çizim işlevi tanımlayan uygulamalar için kolaylık olarak ayrı bir API olarak sağlanır. Düğme arka plan çizimini özelleştirmek isteyen uygulamalar kendi özel çizim işlevlerini sağlayabilir ve gx_text_button_text_draw hizmetini özel çiziminin bir parçası olarak çağırarak arka plan üzerinde düğme metnini çizin.

### <a name="parameters"></a>Parametreler

- **text_button**: metin düğmesi denetim bloğuna işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Define a custom drawing function */

VOID my_button_draw(GX_TEXT_BUTTON *button)
{
    /* Insert code here to draw button background */

    /* Call support function to do text drawing */
    gx_text_button_text_draw(button);

    /* Draw child widgets */
    gx_widget_children_draw((GX_WIDGET *) button);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create, x_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_draw
- gx_text_button_event_process
- gx_text_button_font_set
- gx_text_button_text_color_set
- gx_text_button_text_set
- gx_text_button_text_id_set

## <a name="gx_text_button_text_get"></a>gx_text_button_text_get

Metin düğmesinden metin al (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_text_button_text_get(
    GX_TEXT_BUTTON *text_button,
    GX_CHAR **return_text);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_text_button_text_get_ext () kullanımı için kullanım dışıdır.

Bu hizmet, metin düğmesinden belirtilen dizeyi alır.

### <a name="parameters"></a>Parametreler

- **text_button**: metin düğmesi denetim bloğuna işaretçi
- **return_text**: metin düğmesinden alınan dizenin işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) düğmeden metin başarıyla alınır
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CHAR *string;

/* Get the string from the text button “my_text_button”. */
status = gx_text_button_text_get(&my_text_button, &string);

/* If status is GX_SUCCESS, the string pointer from
“my_text_button” is retrieved and stored in string. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_button_text_get_ext

## <a name="gx_text_button_text_get_ext"></a>gx_text_button_text_get_ext

Metin düğmesinden metin al

### <a name="prototype"></a>Prototype

```C
UINT gx_text_button_text_get_ext(
    GX_TEXT_BUTTON *text_button,
    GX_STRING *return_string);
```

### <a name="description"></a>Açıklama

Bu hizmet, metin düğmesinden belirtilen dizeyi alır.

### <a name="parameters"></a>Parametreler

- **text_button**: metin düğmesi denetim bloğuna işaretçi
- **return_string**: metin düğmesinden alınan dizenin işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) düğmeden metin başarıyla alınır
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING string;

/* Get the string from the text button “my_text_button”. */
status = gx_text_button_text_get_ext(&my_text_button, &string);

/* If status is GX_SUCCESS, the string pointer and length from
“my_text_button” is retrieved and stored in string. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create, x_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_draw
- gx_text_button_event_process
- gx_text_button_font_set
- gx_text_button_text_color_set
- gx_text_button_text_set
- gx_text_button_text_id_set

## <a name="gx_text_button_text_id_set"></a>gx_text_button_text_id_set

Metin düğmesi için metin kaynak KIMLIĞI ayarlama

### <a name="prototype"></a>Prototype

```C
UINT gx_text_button_text_id_set(
    GX_TEXT_BUTTON *text_button,
    RESOURCE_ID string_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen dize kaynak KIMLIĞINI metin düğmesine ayarlar.

### <a name="parameters"></a>Parametreler

- **text_button**: metin düğmesi denetim bloğuna işaretçi
- **string_id**: DIZENIN kaynak kimliği

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) DIZE kaynak kimliği 'ni metin düğmesine başarıyla ayarladı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_INVALID_RESOURCE_ID**: (0x33) dize kimliği geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the string ID ”MY_STRING_ID” to the text button
“my_text_button”. */

status = gx_text_button_text_id_set(&my_text_button,
    MY_STRING_ID);

/* If status is GX_SUCCESS, the string ID MY_STRING_ID was set to
“my_text_button”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create, x_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_draw
- gx_text_button_event_process
- gx_text_button_font_set
- gx_text_button_text_color_set
- gx_text_button_text_get

## <a name="gx_text_button_text_set"></a>gx_text_button_text_set

Metin düğmesine metin ata (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_text_button_text_set(
    GX_TEXT_BUTTON *text_button,
    GX_CHAR *text);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_text_button_text_set_ext () kullanımı için kullanım dışıdır.

Bu hizmet, belirtilen dizeyi metin düğmesine atar. Text_button pencere öğesi stil GX_STYLE_TEXT_COPY ile oluşturulduysa pencere öğesi, atanan metin dizesinin özel bir kopyasını oluşturur. GX_STYLE_TEXT_COPY etkin değilse, pencere öğesi gelen dizenin özel bir kopyasını oluşturmaz, bu nedenle dize statik veya genel olarak ayrılmış olmalıdır, yani bu bir otomatik veya geçici değişken olmayabilir.

### <a name="parameters"></a>Parametreler

- **text_button**: metin düğmesi denetim bloğuna işaretçi
- **metin**: null ile sonlandırılmış dizeye yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) metin düğmeye başarıyla ayarlandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_SYSTEM_MEMORY_ERROR**: (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu
- **GX_INVALID_STRING_LENGTH**: (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the string “my string” to the text button “my_text_button”.
*/

status = gx_text_button_text_set(&my_text_button, “my string”);

/* If status is GX_SUCCESS, the string “my_text_button” was set.
*/
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_button_event_process
- gx_text_button_text_set_ext
- gx_text_button_text_id_set

## <a name="gx_text_button_text_set_ext"></a>gx_text_button_text_set_ext

Metin düğmesine metin atama

### <a name="prototype"></a>Prototype

```C
UINT gx_text_button_text_set_ext(
    GX_TEXT_BUTTON *text_button,
    GX_STRING *string);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen dizeyi metin düğmesine atar. Text_button pencere öğesi stil GX_STYLE_TEXT_COPY ile oluşturulduysa pencere öğesi, atanan metin dizesinin özel bir kopyasını oluşturur. GX_STYLE_TEXT_COPY etkin değilse, pencere öğesi gelen dizenin özel bir kopyasını oluşturmaz, bu nedenle dize statik veya genel olarak ayrılmış olmalıdır, yani bu bir otomatik veya geçici değişken olmayabilir.

### <a name="parameters"></a>Parametreler

- **text_button**: metin düğmesi denetim bloğuna işaretçi
- **String**: GX_STRING değişkenine yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) metin düğmeye başarıyla ayarlandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil
- **GX_SYSTEM_MEMORY_ERROR**: (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu
- **GX_INVALID_STRING_LENGTH**: (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING new_string; new_string.gx_string_ptr = “Monday”;

new_string.gx_string_length = strlen(new_string.gx_string_ptr);

/* Assign the string “new_string” to the text button
“my_text_button”. */

status = gx_text_button_text_set_ext(&my_text_button, &new_string);

/* If status is GX_SUCCESS, the string “my_text_button” was set.
*/
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_button_background_draw
- gx_button_create
- gx_button_deselect
- gx_button_draw
- gx_button_event_process
- gx_button_select
- gx_icon_button_create, x_pixelmap_button_create
- gx_pixelmap_button_draw
- gx_text_button_create
- gx_text_button_draw
- gx_text_button_event_process
- gx_text_button_font_set
- gx_text_button_text_color_set
- gx_text_button_text_get
- gx_text_button_text_id_set

## <a name="gx_text_input_cursor_blink_interval_set"></a>gx_text_input_cursor_blink_interval_set

İmleç yanıp sönme aralığını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_text_input_cursor_blink_interval_set(
    GX_TEXT_INPUT_CURSOR *cursor_input,
    GX_UBYTE blink_interval);
```

### <a name="description"></a>Açıklama

Bu hizmet, İmlecin yanıp sönme aralığı değerini ayarlar.

### <a name="parameters"></a>Parametreler

- **cursor_input** İmleç denetim bloğu
- **blink_interval** Ayarlanacak değer

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) imleç yanıp sönme aralığını başarıyla ayarladı
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE**: (0x22) yanıp sönen Aralık değeri geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_TEXT_INPUT_CURSOR *input_cursor;

/* Pointer the input cursor to the cursor instance of single/multi
line text input widget. */

input_cursor = &sl_input.gx_single_line_text_input_cursor_instance;

/* Set the blink interval value of “input_cursor” to 2. */
status = gx_text_input_cursor_blink_interval_set(input_cursor, 2);

/* If status is GX_SUCCESS, the blink interval value of
“input_cursor” has been successfully set to 2. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_input_cursor_height_set
- gx_text_input_cursor_width_set

## <a name="gx_text_input_cursor_height_set"></a>gx_text_input_cursor_height_set

İmleç yüksekliğini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_text_input_cursor_height_set(
    GX_TEXT_INPUT_CURSOR *cursor_input,
    GX_UBYTE height);
```

### <a name="description"></a>Açıklama

Bu hizmet, imlecin yüksekliğini ayarlar.

### <a name="parameters"></a>Parametreler

- **cursor_input**: imleç denetim bloğu
- **Yükseklik** Ayarlanacak değer

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) Imleç yüksekliği başarıyla ayarlandı
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE**: (0x22) yükseklik değeri geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_TEXT_INPUT_CURSOR *input_cursor;

/* Pointer the input cursor to the cursor instance of single/multi
line text input widget. */

input_cursor = &sl_input.gx_single_line_text_input_cursor_instance;

/* Set height value of “input_cursor”. */
status = gx_text_input_cursor_height_set(&input_cursor, 15);

/* If status is GX_SUCCESS, the height value of “input_curosr” has
been successfully set to 15. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_input_cursor_blink_interval_set
- gx_text_input_cursor_width_set

## <a name="gx_text_input_cursor_width_set"></a>gx_text_input_cursor_width_set

İmleç genişliğini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_text_input_cursor_blink_width_set(
    GX_TEXT_INPUT_CURSOR *cursor_input,
    GX_UBYTE *width);
```

### <a name="description"></a>Açıklama

Bu hizmet, imlecin genişliğini ayarlar.

### <a name="parameters"></a>Parametreler

- **cursor_input**: imleç denetim bloğu
- **Width**: ayarlanacak değer

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) Imleç genişliği başarıyla ayarlandı
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_VALUE**: (0x22) genişlik değeri geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_TEXT_INPUT_CURSOR *input_cursor;

/* Pointer the input cursor to the cursor instance of single/multi
line text input widget. */

input_cursor = &sl_input.gx_single_line_text_input_cursor_instance;

/* Set width of “input_curosr” to 2. */

status = gx_text_input_cursor_blink_width_set(&input_cursor, 2);

/* If status is GX_SUCCESS, the width of “input_cursor” has been
successfully set to 2. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_text_input_cursor_blink_interval_set
- gx_text_input_cursor_height_set

## <a name="gx_text_scroll_wheel_callback_set"></a>gx_text_scroll_wheel_callback_set

Metin türü kaydırma tekerinin geri çağırma işlevini ata (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_text_scroll_wheel_callback_set(
    GX_TEXT_SCROLL_WHEEL *wheel,
    GX_CONST GX_CHAR *(*callback)(GX_TEXT_SCROLL_WHEEL *, int));
```

### <a name="description"></a>Açıklama

Bu hizmet gx_text_scroll_wheel_callback_set_ext () kullanımı için kullanım dışıdır.

Bu hizmet, kaydırma tekerleğinin her satırında görüntülenecek metin dizesini belirleyebilmek için bir metin türü kaydırma tekerinin çağıracağı geri çağırma işlevini atar.

GX_NUMERIC_SCROLL_WHEEL ve GX_STRING_SCROLL_WHEEL için, varsayılan geri çağırma işlevleri sağlanır ve uygulamanın bu varsayılan uygulamaları kullanmak için herhangi bir değişiklik yapması gerekmez.

Bu API, uygulamanın, kaydırma tekerleği pencere öğesinin her satırında görüntülenen biçimlendirme veya dizenin diğer parametrelerini özelleştirmesini sağlamak için sağlanır.

Geri çağırma işlevi, kaydırma tekerleği denetim bloğuna ve görüntülenen satır numarasına bir işaretçi girişi olarak gönderilir. İşlev, bir metin dizesine bir işaretçi döndürmelidir.

### <a name="parameters"></a>Parametreler

- **tekerlek** Dize kaydırma tekerleği denetim bloğu adresi
- **geri arama** Geri çağırma işlevine işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) geri çağırma başarıyla ayarlandı
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_TEXT_SCROLL_WHEEL wheel;

GX_CHAR string_buffer[20];

GX_CHAR *my_wheel_callback(GX_TEXT_SCROLL_WHEEL *wheel, int row)
{
    /* Just for an example, return row number as string for rows
    >= 0, and return text “Invalid” otherwise */
    if (row >= 0)
    {
        gx_utility_ltoa(row, string_buffer, 20);
    }
    else
    {
        return(“Invalid”);
    }
}

gx_text_scroll_wheel_create(&wheel, “my wheel”, root, 10,
    GX_STYLE_ENABLED|GX_STYLE_TEXT_CENTER|GX_STYLE_TRANSPARENT|
    GX_STYLE_WRAP|ID_MY_WHEEL, &size);

status = gx_text_scroll_wheel_callback_set(&wheel,
    my_wheel_callback);

/* If status is GX_SUCCESS, the scroll whell callback function has
been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_event_process
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set

## <a name="gx_text_scroll_wheel_callback_set_ext"></a>gx_text_scroll_wheel_callback_set_ext

Metin türü kaydırma tekerleğinin geri çağırma işlevini ata

### <a name="prototype"></a>Prototype

```C
UINT gx_text_scroll_wheel_callback_set_ext(
    GX_TEXT_SCROLL_WHEEL *wheel,
    UINT *(*callback)(GX_TEXT_SCROLL_WHEEL *, int, GX_STRING *));
```

### <a name="description"></a>Açıklama

Bu hizmet, kaydırma tekerleğinin her satırında görüntülenecek metin dizesini belirleyebilmek için bir metin türü kaydırma tekerinin çağıracağı geri çağırma işlevini atar.

GX_NUMERIC_SCROLL_WHEEL ve GX_STRING_SCROLL_WHEEL için, varsayılan geri çağırma işlevleri sağlanır ve uygulamanın bu varsayılan uygulamaları kullanmak için herhangi bir değişiklik yapması gerekmez.

Bu API, uygulamanın, kaydırma tekerleği pencere öğesinin her satırında görüntülenen biçimlendirme veya dizenin diğer parametrelerini özelleştirmesini sağlamak için sağlanır.

Geri çağırma işlevi, kaydırma tekerleği denetim bloğuna ve görüntülenen satır numarasına bir işaretçi girişi olarak gönderilir. İşlev, bir metin dizesine bir işaretçi döndürmelidir.

### <a name="parameters"></a>Parametreler

- **tekerlek** Dize kaydırma tekerleği denetim bloğu adresi
- **geri arama** Geri çağırma işlevine işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) geri çağırma başarıyla ayarlandı
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_TEXT_SCROLL_WHEEL wheel;

GX_CHAR string_buffer[20];

UINT *my_wheel_callback(GX_TEXT_SCROLL_WHEEL *wheel, int row,
    GX_STRING *return_string)
{
    /* Just for an example, return row number as string for rows
    >= 0, and return text “Invalid” otherwise */
    if (row >= 0)
    {
        gx_utility_ltoa(row, string_buffer, 20);
        return_string->gx_string_ptr = string_buffer;
        return_string->gx_string_length = strlen(string_buffer);
    }
    else
    {
        return_string->gx_string_ptr = “Invalid”;
        return_string->gx_string_length = strlen(“Invalid”);
    }

    return GX_SUCCESS;
}

gx_text_scroll_wheel_create(&wheel, “my wheel”, root, 10,
    GX_STYLE_ENABLED|GX_STYLE_TEXT_CENTER|GX_STYLE_TRANSPARENT|
    GX_STYLE_WRAP|ID_MY_WHEEL, &size);

status = gx_text_scroll_wheel_callback_set_ext(&wheel,
    my_wheel_callback);

/* If status is GX_SUCCESS, the scroll whell callback function has
been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_event_process
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set

## <a name="gx_text_scroll_wheel_create"></a>gx_text_scroll_wheel_create

Metin kaydırma tekerleği oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_text_scroll_wheel_create(
    GX_TEXT_SCROLL_WHEEL *wheel,
    GX_CONST GX_CHAR *name, 
    GX_WIDGET *parent, 
    INT total_rows,
    ULONG style, 
    USHORT Id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir metin kaydırma tekerleği oluşturur. Metin kaydırma tekerleği, GX_STRING_SCROLL_WHEEL ve GX_NUMERIC_SCROLL_WHEEL türü pencere öğeleri için temel pencere öğesi. Bu işlev, gx_string_scroll_wheel_create ve gx_numeric_scroll_wheel_create tarafından dahili olarak çağrılır ve özel bir kaydırma tekerleği pencere öğesi tanımlayan uygulamalar için kolaylık olarak ayrı bir API olarak sağlanır.

### <a name="parameters"></a>Parametreler

- **tekerlek**: metin kaydırma tekerleği denetim bloğu adresi
- **ad**: uygulama tanımlı pencere öğesi adı
- **üst öğe**: tekerlek üstü veya GX_NULL
- **total_rows**: kullanıcıya sunulacak toplam satır sayısı
- **Stil**: istenen stil bayrakları
- **Kimlik**: uygulama tanımlı tekerlek stili bayrakları
- **Boyut**: ilk kaydırma tekerleği boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) metin kaydırma tekerleği başarıyla oluşturuldu
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED**: (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil


### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define a custom scroll wheel widget. */
typedef MY_SCROLL_WHEEL_STRUCT
{
    GX_TEXT_SCROLL_WHEEL text_scroll_wheel;

    /* Add custom members here. */

} MY_SCROLL_WHEEL;

MY_SCROLL_WHEEL my_scroll_wheel;

UINT my_scroll_wheel_create(MY_SCROLL_WHEEL *wheel,
    GX_CONST GX_CHAR *name, GX_WIDGET *parent,
    INT total_rows, ULONG style, USHORT Id,
    GX_CONST GX_RECTANGLE *size)
{
    /* Call base creation. */
    status = gx_text_scroll_wheel_create(
        &wheel.text_scroll_wheel,
        ”my_text_scroll_wheel”, GX_NULL, 7,
        GX_STYLE_ENABLED, ID_MY_SCROLL_WHEEL, &size);

    if (status == GX_SUCCESS)
    {
        /* Add custom initialization here. */
        if(parent)
        {
            gx_widget_link(parent, (GX_WIDGET *)wheel);
        }
    }
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_string_scroll_wheel_string_id_list_set
- gx_string_scroll_wheel_string_list_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_event_process
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set

## <a name="gx_text_scroll_wheel_draw"></a>gx_text_scroll_wheel_draw

Metin kaydırma tekerleği çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_text_scroll_wheel_draw(GX_TEXT_SCROLL_WHEEL *wheel);
```

### <a name="description"></a>Açıklama

Bu, GX_TEXT_SCROLL_WHEEL dayalı tüm tekerlek türleri için varsayılan çizim işlevidir. Bu işlev, metin kaydırma tekerleği çizim görünümünü özelleştirmeyi gerektiren uygulamalar tarafından geçersiz kılınabilir.

GX_STRING_SCROLL_WHEEL ve GX_NUMERIC_SCROLL_WHEEL, GX_TEXT_SCROLL_WHEEL dayanır veya türetilir.

### <a name="parameters"></a>Parametreler

- **tekerlek**: dize kaydırma tekerleği denetim bloğu adresi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom wheel draw function. */
UINT my_wheel_draw(GX_TEXT_SCROLL_WHEEL *wheel)
{
    /* Perform default drawing */
    gx_text_scroll_wheel_draw(wheel);

    /* Add custom drawing here */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_event_process
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set

## <a name="gx_text_scroll_wheel_event_process"></a>gx_text_scroll_wheel_event_process


Metin kaydırma tekerleği olayını işle

### <a name="prototype"></a>Prototype

```C
UINT gx_text_scroll_wheel_event_process(GX_TEXT_SCROLL_WHEEL *wheel, GX_EVENT *event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen metin kaydırma tekerleği için bir olayı işler. Bu hizmet, özel metin kaydırma tekerleği olay işleme işlevleri tarafından varsayılan olay işleyicisi olarak çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **tekerlek** Metin kaydırma tekerleği denetim bloğu işaretçisi
- **event_ptr** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı metin kaydırma tekerleği olay işlemi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic text scroll wheel event processing as part of custom event processing function. */

UINT custom_text_scroll_wheel_event_process(GX_TEXT_SCROLL_WHEEL *wheel, GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;

    default:
        /* Pass all other events to the default text scroll wheel event processing */
        status = gx_text_scroll_wheel_event_process(wheel, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_font_set
- gx_text_scroll_wheel_text_color_set

## <a name="gx_text_scroll_wheel_font_set"></a>gx_text_scroll_wheel_font_set

Kaydırma tekerleği satırlarını çizmek için kullanılan yazı tiplerini atama

### <a name="prototype"></a>Prototype

```C
UINT gx_text_scroll_font_set(
    GX_TEXT_SCROLL_WHEEL *wheel,
    GX_RESOURCE_ID normal_font, 
    GX_RESOURCE_ID selected_font);
```

### <a name="description"></a>Açıklama

Metin kaydırma tekerleği tabanlı pencere öğesinin metnini çizmek için kullanılacak yazı tiplerini atayın.

### <a name="parameters"></a>Parametreler

- **tekerlek**: dize kaydırma tekerleği denetim bloğu adresi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) tekerlek yazı tipi başarıyla atandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_NUMERIC_SCROLL_WHEEL wheel;

status = gx_text_scroll_wheel_font_set(&wheel,
    GX_FONT_ID_WHEEL_NORMAL,
    GX_FONT_ID_WHEEL_SELECTED);

/* If status is GX_SUCCESS, the scroll wheel fonts have been assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_event_process
- gx_text_scroll_wheel_text_color_set

## <a name="gx_text_scroll_wheel_text_color_set"></a>gx_text_scroll_wheel_text_color_set

Kaydırma tekerleği satırlarını çizmek için kullanılan renkleri atama

### <a name="prototype"></a>Prototype

```C
UINT gx_text_scroll_wheel_text_color_set(
    GX_TEXT_SCROLL_WHEEL *wheel,
    GX_RESOURCE_ID normal_text_color,
    GX_RESOURCE_ID selected_text_color,
    GX_RESOURCe_ID disabled_text_color);
```

### <a name="description"></a>Açıklama

Bu işlev metin tabanlı bir kaydırma tekerleği satırları çizmek için kullanılan metin renklerini atar.

### <a name="parameters"></a>Parametreler

- **tekerlek**: dize kaydırma tekerleği denetim bloğu adresi
- **normal_text_color**: seçili olmayan satırları çizmek için kullanılan renk
- **selected_text_color**: seçili satırı çizmek için kullanılan renk.
- **disabled_text_color**: devre dışı pencere öğesi için metin çizmek için kullanılan renk.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) kaydırma tekerleği metin rengi başarıyla atandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING_SCROLL_WHEEL wheel;

UINT status = gx_text_scroll_wheel_text_color_set(&wheel,
    GX_COLOR_ID_NORMAL_TEXT,
    GX_COLOR_ID_SELECTED_TEXT,
    GX_COLOR_ID_DISABLED_TEXT);

/* If status is GX_SUCCESS, the colors used to draw the wheel text have been assigned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_numeric_scroll_wheel_create
- gx_numeric_scroll_wheel_range_set
- gx_scroll_wheel_create
- gx_scroll_wheel_event_process
- gx_scroll_wheel_gradient_alpha_set
- gx_scroll_wheel_row_height_set
- gx_scroll_wheel_selected_background_set
- gx_scroll_wheel_selected_get
- gx_scroll_wheel_selected_set
- gx_scroll_wheel_total_rows_set
- gx_text_scroll_wheel_callback_set
- gx_text_scroll_wheel_create
- gx_text_scroll_wheel_draw
- gx_text_scroll_wheel_event_process
- gx_text_scroll_wheel_font_set

## <a name="gx_tree_view_create"></a>gx_tree_view_create

Ağaç görünümü oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_tree_view_create(
    GX_TREE_VIEW *tree,
    GX_CONST GX_CHAR *name, 
    GX_WIDGET *parent,
    ULONG style, 
    USHORT tree_view_id,
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet belirtildiği şekilde bir ağaç görünümü oluşturur ve ağaç görünümünü sağlanan üst pencere öğesiyle ilişkilendirir. Alt menü öğesi olarak tüm pencere öğesi türlerini kabul eder. GX_MENU türü pencere öğesinin alt menü öğesi olarak kullanılması önerilir.

GX_TREE_VIEW GX_WINDOW türetilir ve tüm gx_window API hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **ağaç**: ağaç görünümü denetim bloğu işaretçisi
- **ad**: ağaç görünümünün adı
- **Parent**: üst pencere öğesi işaretçisi
- **Stil**: pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **menu_id**: ağaç görünümünün uygulama tanımlı kimliği
- **Boyut**: ağaç görünümünün boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı ağaç görünümü oluşturma
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED**: (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE**: (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
status = gx_tree_view_create(&my_tree_view,
    “my_tree_view”, parent,
    GX_STYLE_ENABLED, MY_TREE_VIEW_ID,
    &size);

/* If status is GX_SUCCESS the tree view was successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set
- gx_tree_view_draw
- gx_tree_view_event_process
- gx_tree_view_indentation_set
- gx_tree_view_position
- gx_tree_view_root_line_color_set
- gx_tree_view_root_pixelmap_set
- gx_tree_view_selected_get
- gx_tree_view_selected_set

## <a name="gx_tree_view_draw"></a>gx_tree_view_draw

Ağaç görünümünü çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_tree_view_draw(GX_TREE_VIEW *tree);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen ağaç görünümünü çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel ağaç görünümü pencere öğeleri için özel çizim işlevleri uygulamaya yardımcı olmak üzere uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **ağaç** Ağaç görünümü denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom tree view draw function. */
UINT my_tree_view_draw(GX_TREE_VIEW *tree_view)
{
    /* Perform default drawing */
    gx_tree_view_draw(tree_view);

    /* Add custom drawing here */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set
- gx_tree_view_create
- gx_tree_view_event_process
- gx_tree_view_indentation_set
- gx_tree_view_position
- gx_tree_view_root_line_color_set
- gx_tree_view_root_pixelmap_set
- gx_tree_view_selected_get
- gx_tree_view_selected_set

## <a name="gx_tree_view_event_process"></a>gx_tree_view_event_process

İşlem Ağacı Görünümü olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_tree_view_event_process(
    GX_TREE_VIEW *tree, 
    GX_EVENT event_ptr);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen ağaç görünümü için bir olayı işler. Bu hizmet özel ağaç görünümü olay işleme işlevleri tarafından varsayılan olay işleyicisi olarak çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **ağaç**: ağaç görünümü denetim bloğu işaretçisi
- **event_ptr**: işlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı işlem ağacı görünümü olayı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic tree view event processing as part of custom event
    processing function. */

UINT custom_tree_view_event_process(GX_TREE_VIEW *tree_view,
    GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
        case xyz:
            /* Insert custom event handling here */
            break;
        default:
            /* Pass all other events to the default tree view
                event processing */
            status = gx_tree_view_event_process(tree_view, event);
            break;
    }
}
return status;
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set
- gx_tree_view_create
- gx_tree_view_draw
- gx_tree_view_indentation_set
- gx_tree_view_position
- gx_tree_view_root_line_color_set
- gx_tree_view_root_pixelmap_set
- gx_tree_view_selected_get
- gx_tree_view_selected_set

## <a name="gx_tree_view_indentation_set"></a>gx_tree_view_indentation_set

Ağaç görünümü girintisini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_tree_view_indentation_set(
    GX_TREE_VIEW *tree,
    GX_VALUE indentation);
```

### <a name="description"></a>Açıklama

Bu hizmet, ağaç görünümü için Girintiyi belirler.

### <a name="parameters"></a>Parametreler

- **ağaç**: ağaç görünümü denetim bloğu işaretçisi
- **girintileme**: ayarlanacak girintileme

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) ağaç görünümü girintisi başarıyla ayarlandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set tree view “my_tree” indentation to 10. */
status = gx_tree_view_indentation_set(&my_tree, 10);

/* If status is GX_SUCCESS the indentation of tree view “my_tree”
has been set to 10. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set
- gx_tree_view_create
- gx_tree_view_draw
- gx_tree_view_event_process
- tree_view_position
- gx_tree_view_root_line_color_set
- gx_tree_view_root_pixemlap_set
- gx_tree_view_selected_get
- gx_tree_view_selected_set

## <a name="gx_tree_view_position"></a>gx_tree_view_position

Ağaç Görünüm öğelerini Konumlandır

### <a name="prototype"></a>Prototype

```C
UINT gx_tree_view_position(GX_TREE_VIEW *tree);
```

### <a name="description"></a>Açıklama

Bu hizmet, ağaç görünümü öğelerini konumlandırır.

### <a name="parameters"></a>Parametreler

- **ağaç**: ağaç görünümü denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) ağaç görünümü öğeleri başarıyla yerleştirildi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Position tree view “my_tree” items. */
status = gx_tree_view_position(&my_tree);

/* If status is GX_SUCCESS the items of tree view “my_tree” has
been positioned. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set
- gx_tree_view_create
- gx_tree_view_draw
- gx_tree_view_event_process
- gx_tree_view_indentation_set
- gx_tree_view_root_line_color_set
- gx_tree_view_root_pixelmap_set
- gx_tree_view_selected_get
- gx_tree_view_selected_set

## <a name="gx_tree_view_root_line_color_set"></a>gx_tree_view_root_line_color_set

Ağaç görünümü kök çizgi rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_tree_view_root_line_color_set(
    GX_TREE_VIEW *tree,
    GX_RESOURCE_ID color_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, ağaç görünümü için kök çizgi rengi atar.

### <a name="parameters"></a>Parametreler

- **ağaç**: ağaç görünümü denetim bloğu işaretçisi
- **color_id**: kök çizgi renginin kaynak kimliği

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı küme kök çizgisi rengi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set root line color for tree view “my_tree”. */

status = gx_tree_view_root_line_color_set(&my_tree,
    MY_ROOT LINE_COLOR_ID);

/* If status is GX_SUCCESS the root line color of the tree view
“my_tree” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set
- gx_tree_view_create
- gx_tree_view_draw
- gx_tree_view_event_process
- gx_tree_view_indentation_set
- gx_tree_view_position
- gx_tree_view_root_pixelmap_set
- gx_tree_view_selected_get
- gx_tree_view_selected_set

## <a name="gx_tree_view_root_pixelmap_set"></a>gx_tree_view_root_pixelmap_set

Ağaç görünümü kök pixelmap ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_tree_view_root_pixelmap_set(
    GX_TREE_VIEW *tree,
    GX_RESOURCE_ID expand_map_id,
    GX_RESOURCE_ID collapse_map_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, ağaç görünümü için bir Genişlet ve Daralt pixelmap 'e atar.

### <a name="parameters"></a>Parametreler

- **ağaç**: ağaç görünümü denetim bloğu işaretçisi
- **expand_map_id**: ' nin Genişlet pixelmap kaynak kimliği
- **collapse_map_id**: pixelmap 'i daraltma kaynak kimliği

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) kök pixelmap başarıyla ayarlandı
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set root pixelmaps for tree view “my_tree”. */

status = gx_tree_view_root_pixelmap_set(&my_tree,
    MY_EXPAND_MAP_ID,
    MY_COLLAPSE_MAP_ID);

/* If status is GX_SUCCESS the root pixelmaps of tree view
“my_tree” has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set
- gx_tree_view_create
- gx_tree_view_draw
- gx_tree_view_event_process
- gx_tree_view_indentation_set
- gx_tree_view_position
- gx_tree_view_selected_get
- gx_tree_view_selected_set

## <a name="gx_tree_view_selected_get"></a>gx_tree_view_selected_get

Seçili öğeyi al

### <a name="prototype"></a>Prototype

```C
UINT gx_tree_view_selected_get(
    GX_TREE_VIEW *tree,
    GX_WIDGET **selected);
```

### <a name="description"></a>Açıklama

Bu hizmet, ağaç görünümünün geçerli seçili öğesini alır.

### <a name="parameters"></a>Parametreler

- **ağaç**: ağaç görünümü denetim bloğu işaretçisi
- **Seçili**: seçili pencere öğesi işaretçisine işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) seçili öğe başarıyla alındı
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Retrieve selected item of tree view “my_tree”. */

GX_WIDGET *selected;

status = gx_tree_view_selected_get(&my_tree, &selected);

/* If status is GX_SUCCESS the selected item of tree view “my_tree”
has been retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set
- gx_tree_view_create
- gx_tree_view_draw
- gx_tree_view_event_process
- gx_tree_view_indentation_set
- gx_tree_view_position
- gx_tree_view_root_line_color_set
- gx_tree_view_root_pixelmap_set
- gx_tree_view_selected_set

## <a name="gx_tree_view_selected_set"></a>gx_tree_view_selected_set

Seçili öğeyi ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_tree_view_selected_set(
    GX_TREE_VIEW *tree,
    GX_WIDGET *selected);
```

### <a name="description"></a>Açıklama

Bu hizmet, ağaç görünümü için seçili öğeyi ayarlar.

### <a name="parameters"></a>Parametreler

- **ağaç**: ağaç görünümü denetim bloğu işaretçisi
- **Seçili**: seçilen yeni öğeye yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı Çiz Menüsü
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET**: (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set selected item of tree view “my_tree” to “tree_view_item’. */
status = gx_tree_view_selected_set(&my_tree, &tree_view_item);

/* If status is GX_SUCCESS selected item of tree view “my_menu” has
been set to “tree_view_item”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_menu_draw
- gx_menu_insert
- gx_menu_remove
- gx_menu_text_draw
- gx_menu_text_offset_set
- gx_tree_view_create
- gx_tree_view_draw
- gx_tree_view_event_process
- gx_tree_view_indentation_set
- gx_tree_view_position
- gx_tree_view_root_line_color_set
- gx_tree_view_root_pixelmap_set
- gx_tree_view_selected_get

## <a name="gx_utility_canvas_to_bmp"></a>gx_utility_canvas_to_bmp

Tuval anma resmini bit eşleme Dönüştür

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_canvas_to_bmp(
    GX_CANVAS *canvas, 
    GX_RECTANGLE *rect,
    UINT (*write_data)(GX_UBYTE *byte_data, UINT data_count));
```

### <a name="description"></a>Açıklama

Bu hizmet tuval belleğini bit eşlem dosyasına dönüştürür.

### <a name="parameters"></a>Parametreler

- **tuval**: tuval denetim bloğu işaretçisi
- **Rect**: dönüştürülecek dikdörtgen
- **write_data**: verileri yazmak için geri çağırma işlev işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) tam sayı değeri dizeye başarıyla dönüştürüldü
- **GX_PTR_ERROR**: (0x07) geçersiz dönüş arabelleği işaretçisi
- **GX_INVALID_SIZE**: (0x19) geçersiz dönüş arabelleği boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
FILE *fp = GX_NULL;

/* define call back function of how to write the data read from
canvas memory. */

UINT write_data_callback(GX_UBYTE *byte_data, UINT data_count)
{
    if (fp)
    {
        fwrite(byte_data, 1, data_count, fp);
    }
    return GX_SUCCESS;
}

VOID scroll_wheel_screen_draw(GX_WINDOW *window)
{
    UINT status;

    GX_RECTANGLE size = {31,31,610,450};
    gx_window_draw(window);
    if (screenshot)
    {
        fp = fopen("../screenshot.bmp", "wb");
        /* Convert canvas memory to bitmap format.
           Status GX_SUCCESS means operation succeed. */
        status = gx_utility_canvas_to_bmp(root->gx_window_root_canvas,
            &size, write_data_callback);

        fclose(fp);
    }
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_circle_point_get"></a>gx_utility_circle_point_get

Bir daire üzerinde nokta hesaplama

### <a name="prototype"></a>Prototype

```C
INT gx_utility_circle_point_get(
    INT xCenter, 
    INT yCenter,
    UINT radius, 
    INT angle, 
    GX_POINT *point);
```

### <a name="description"></a>Açıklama

Bu hizmet, daire Merkezi, yarıçap ve açı verilen bir daire üzerindeki noktayı hesaplar.

### <a name="parameters"></a>Parametreler

- **Xcenter**: Daire merkezinin x koordinatı
- **YCenter**: Daire merkezinin y koordinatı
- **yarıçap**: Daire yarıçapı
- **açı**: Daire çevre noktasının derece cinsinden hesaplanacağı açı
- **Point**: hesaplanan x, y koordinatını depolayacağınız GX_POINT değişkenin adresi
- **end_alpha**: bitiş alfa değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) gradyanı oluşturuldu
- **GX_PTR_ERROR**: (0x07) geçersiz dönüş noktası adresi
- **GX_INVALID_VALUE**: (0x22) geçersiz radius parametresi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_POINT point;
    UINT status;

        status = gx_utility_circle_point_get(100, 100,
20, 45,
&point);

/* If status is GX_SUCCESS the value of point is the x,y coordinate of a point on the circle perimeter at an angle of 45 degrees, where the circle is centered at (100, 100), has a radius of 20 pixels */

```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_asin
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_gradient_create"></a>gx_utility_gradient_create

Bir gradyan pixelmap oluşturun

### <a name="prototype"></a>Prototype

```C
INT gx_utility_gradient_create(
    GX_GRADIENT *gradient,
    GX_VALUE width, 
    GX_VALUE height,
    UCHAR type, 
    GX_UBYTE start_alpha, 
    GX_UBYTE end_alpha);
```

### <a name="description"></a>Açıklama

Bu hizmet, çalışma zamanında bir gradyan pixelmap oluşturur. Bir gradyan görüntüsü, belirme efektlerini ve diğer ilgi çekici görsel değişiklikleri gerçekleştirmek için kullanılabilir.

İstenen degradenin genişliği ve yüksekliği, 2x2 pikselden az olamaz.

GUX, oluşturulan degradeler listesinin bir listesini tutar ve bu işlev ilk olarak, yeni bir pixelmap oluşturmadan önce eşleşen bir gradyan pixelmap bulmak için gradyan listesinde arama yapar. Diğer bir deyişle, aynı gradyan pixelmap 'i birden çok kez gerekir, yalnızca bir pixelmap oluşturulmuştur ve bu pixelmap 'i gerektiren her degrade oluşturulan pixelmap 'i paylaşır.

Bu API, çalışma zamanı bellek ayırmaya izin vermek için gx_system_memory_allocator işlevinin tanımlanmasını gerektirir.

Gradyan türü bayrakları GX_GRADIENT_TYPE_ALPHA ve GX_GRADIENT_TYPE_MIRROR içerir. Şu anda yalnızca GX_GRADIENT_TYPE_ALPHA tür degradeleri destekleniyor (Yani bu tür bayrağının ayarlanması gerekir). GX_GRADIENT_TYPE_MORROR bayrağı isteğe bağlıdır ve ayarlandığında, gradyan oluşturma mantığının start_alpha end_alpha ve start_alpha olarak değişen bir gradyan oluşturmasını söyler. Aksi halde doğrusal bir gradyan oluşturulur.

### <a name="parameters"></a>Parametreler

- **gradyan**: gradyan denetim bloğu yapısına yönelik işaretçi
- **Genişlik**: istenen pixelmap genişliği
- **Yükseklik**: istenen pixelmap yüksekliği
- **tür**: istenen gradyan türü
- **start_alpha**: alfa değeri başlatılıyor
- **end_alpha**: bitiş alfa değeri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) gradyanı oluşturuldu
- **GX_INVALID_SIZE**: (0x19) gradyan en az 2x2 piksel değil
- **GX_NOT_SUPPORTED**: (0x28) gradyan türünde değil GX_GRADIENT_TYPE_ALPHA
- **GX_FAILURE**: (0x10) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) gradyan işaretçisi geçerli değil<
- **GX_INVALID_VALUE**: (0x22) genişlik ve yükseklik değeri geçerli değil
- **GX_INVALID_TYPE**: (0x1B) gradyan türü geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_GRADIENT gradient;

UINT status;

status = gx_utiity_gradient_create(&gradient, 3, 40,
    GX_GRADIENT_TYPE_ALPHA, 240, 0);

/* If status == GX_SUCCESS the gradient pixelmap has been created */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_asin
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_gradient_delete"></a>gx_utility_gradient_delete

Önceden oluşturulmuş bir degradeyi silme

### <a name="prototype"></a>Prototype

```C
INT gx_utility_gradient_delete(GX_GRADIENT *gradient);
```

### <a name="description"></a>Açıklama

Bu hizmet daha önce oluşturulmuş bir degradeyi siler. Bu degradeyle ilişkilendirilen pixelmap başka degradeler tarafından kullanımda değilse, pixelmap verileri de silinir.

### <a name="parameters"></a>Parametreler

- **gradyan**: gradyan denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) gradyan silindi
- **GX_CALLER_ERROR**: (0x11) bu işlevin çağıranı geçersiz
- **GX_PTR_ERROR**: (0x07) gradyan işaretçisi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_GRADIENT gradient;

UINT status;

/* Delete previously created gradient. */
status = gx_utility_gradient_delete(&gradient);

/* If status == GX_SUCCESS, the gradient has been deleted. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_asin
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_ltoa"></a>gx_utility_ltoa

Uzun tamsayıyı ASCII 'ye Dönüştür

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_itoa(
    LONG value, 
    GX_CHAR *return_buffer,
    UINT seturn_buffer_size);
```

### <a name="description"></a>Açıklama

Bu hizmet uzun bir tamsayı değerini bir ASCII dizesine dönüştürür.

### <a name="parameters"></a>Parametreler

- **değer**: dönüştürülecek Long Integer değeri
- **return_buffer**: ASCII dizesi için hedef arabellek
- **return_buffer_size**: hedef arabelleğin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) tam sayı değeri dizeye başarıyla dönüştürüldü
- **GX_PTR_ERROR**: (0x07) geçersiz dönüş arabelleği işaretçisi
- **GX_INVALID_SIZE**: (0x19) geçersiz dönüş arabelleği boyutu

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
INT my_value = 200;

GX_CHAR string_buffer[10];

UINT status;

/* Convert “my_value” into an ASCII string. */
status = gx_utility_ltoa(my_value, string_buffer, 10);

/* If status is GX_SUCCESS, “string_buffer” contains the ASCII
representation of “my_value”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_math_acos"></a>gx_utility_math_acos

İşlem yay kosinüsü

### <a name="prototype"></a>Prototype

```C
INT gx_utility_math_acos(GX_FIXED_VAL x);
```

### <a name="description"></a>Açıklama

Bu hizmet, ark kosinüs x 'in açı değerini hesaplar.

Giriş değeri sabit bir nokta veri türüdür, INT 'ten GX_FIXED_VAL türüne dönüştürmek için GX_FIXED_VAL_MAKE çağırın. Örneğin, 0,5 'in ark kosinüsünü hesaplamak istiyorsanız, girişi GX_FIXED_VAL_MAKE (1)/2 olarak yapın.

5.4.0 veya daha düşük sürümde, bu işlevin giriş değeri türü INT 'tir ve değer [-256, 256] aralığıyla sınırlıdır. Bu hizmeti çağırmak için uygulama [-1, 1] aralığından [-256, 256] aralığında değeri ölçeklendirmelidir. GUX sürümüne eşit veya daha küçük olan projeniz bu API 'ye başvuru içeriyorsa ve projenizi en son Gux kitaplığıyla yükseltmek istiyorsanız. İki seçenek sunulur.

1. Bu API çağrısının giriş değerini, GX_FIXED_VAL veri türü değerini kullanacak şekilde düzeltir.
1. GUIX_5_4_0_COMPATIBILITY tanımlayın.

### <a name="parameters"></a>Parametreler

- **x**: yay kosinüsü hesaplanan değer

### <a name="return-values"></a>Dönüş Değerleri

- **açı**: ark kosinüs x 'in açı değeri

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
/* Compute the angle value of arc cosine of “0.5”. */

#if defined(GUIX_5_4_0_COMPATIBILITY)
    x = 256 / 2;
#else
    x = GX_FIXED_VAL_MAKE(1) / 2;
#endif

angle = gx_utility_math_acos(x);

/* “angle” contains the angle value of arc cosine “x”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_asin
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_math_asin"></a>gx_utility_math_asin

İşlem yay sinüsü

### <a name="prototype"></a>Prototype

```C
INT gx_utility_math_asin(GX_FIXED_VAL x);
```

### <a name="description"></a>Açıklama

Bu hizmet, ark sinüs x 'in açı değerini hesaplar.

Giriş değeri sabit bir nokta veri türüdür, INT 'ten GX_FIXED_VAL türüne dönüştürmek için GX_FIXED_VAL_MAKE çağırın. Örneğin, 0,5 yay değerini hesaplamak istiyorsanız, girişi GX_FIXED_VAL_MAKE (1)/2 olarak yapın.

5.4.0 veya daha düşük sürümde, bu işlevin giriş değeri türü INT 'tir ve değer [-256, 256] aralığıyla sınırlıdır. Bu hizmeti çağırmak için uygulama [-1, 1] aralığından [-256, 256] aralığında değeri ölçeklendirmelidir. GUX sürümüne eşit veya ondan küçükse ve projenizi en son Gux kitaplığıyla yükseltmek istiyorsanız. İki seçenek sunulur.

1. Bu API çağrısının giriş değerini, GX_FIXED_VAL veri türü değerini kullanacak şekilde düzeltir.
1. GUIX_5_4_0_COMPATIBILITY tanımlayın.

### <a name="parameters"></a>Parametreler

- **x**: yay sinüsü hesaplanan değer

### <a name="return-values"></a>Dönüş Değerleri

- **açı**: Ark sinüsü x açı değeri

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
/* Compute the angle value of arc sine of “x”. */

#if defined GUIX_5_4_0_COMPATIBILITY
    x = 256 / 2;
#else
    X = GX_FIXED_VAL_MAKE(1) / 2;
#endif

angle = gx_utility_math_asin(x);

/* “angle” contains the angle value of arc sine “x”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_acos
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_math_cos"></a>gx_utility_math_cos

İşlem kosinüsü

### <a name="prototype"></a>Prototype

```C
GX_FIXED_VAL gx_utility_math_cos(GX_FIXED_VAL angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, sağlanan açının kosinüsünü hesaplar.

Giriş değeri sabit bir nokta veri türüdür, INT 'ten GX_FIXED_VAL dönüştürmek için GX_FIXED_VAL_MAKE çağırın. Örneğin, 90 derece kosinüsünü hesaplamak istiyorsanız, girişi GX_FIXED_VAL_MAKE (90) olarak yapın.

Dönüş değeri sabit bir nokta veri türüdür, GX_FIXED_VAL ' dan INT 'e dönüştürmek için GX_FIXED_VAL_TO_INT çağırın.

5.4.0 veya daha düşük sürüm Gux sürümünde, bu hizmetin giriş değeri ve dönüş değeri INT 'tir, giriş değeri ve dönüş değeri 256 ile genişletilir. Bu nedenle, uygulamanın bu hizmeti çağırabilmesi için açı değerini 256 ile Ölçeklendirmesi gerekir. GUX sürümüne eşit veya daha küçük bir sürüme sahip projeniz 5.4.0 ve projenizi en son Gux kitaplığıyla yükseltmek istiyorsanız iki seçeneğiniz vardır.

1. GX_FIXED_VAL tarih türü değerini kullanmak için bu API çağrısının dönüş değerine giriş değerini ve işlemeyi düzeltemedi.
1. GUIX_5_4_0_COMPATIBILITY tanımlayın.

### <a name="parameters"></a>Parametreler

- **açı**: öğesinin işlem kosinüsü için açı

### <a name="return-values"></a>Dönüş Değerleri

- **kosinüs**: sağlanan açının kosinüs değeri

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
/* Compute cosine of 90 degree. */

INT angle = 90;

#if defined (GUIX_5_4_0_COMPATIBILITY)
    INT scaled_angle = angle << 8;
#else
    GX_FIXED_VAL scaled_angle = GX_FIXED_VAL_MAKE(angle);
#endif

my_angle_cosine = gx_utility_math_cos(scaled_angle);

/* “my_angle_cosine” contains the cosine of “my_angle”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_acos
- gx_utility_math_asin
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_math_sin"></a>gx_utility_math_sin

İşlem sinüsü

### <a name="prototype"></a>Prototype

```C
GX_FIXED_VAL gx_utility_math_sin(GX_FIXED_VAL angle);
```

### <a name="description"></a>Açıklama

Bu hizmet, sağlanan açının sinüsünü hesaplar.

Giriş değeri sabit bir nokta veri türüdür, INT 'ten GX_FIXED_VAL dönüştürmek için GX_FIXED_VAL_MAKE çağırın. Örneğin, 90 derecelik sinüsü hesaplamak istiyorsanız, girişi GX_FIXED_VAL_MAKE (90) olarak yapın. 

Dönüş değeri sabit bir nokta veri türüdür, GX_FIXED_VAL ' dan INT 'e dönüştürmek için GX_FIXED_VAL_TO_INT çağırın.

5.4.0 veya daha düşük sürümde, giriş değeri ve dönüş değer türü INT 'tir, giriş değeri ve dönüş değeri 256 ile genişletilir. Bu nedenle, uygulamanın bu hizmeti çağırabilmesi için açı değerini 256 ile Ölçeklendirmesi gerekir. GUX sürümüne eşit veya daha küçük bir sürüme sahip projeniz 5.4.0 ve projenizi en son Gux kitaplığıyla yükseltmek istiyorsanız iki seçeneğiniz vardır.

1. GX_FIXED_VAL veri türü değerini kullanmak için bu API çağrısının giriş değerini ve dönüş değerine teslim etme değerini onarın.
1. GUIX_5_4_0_COMPATIBILITY tanımlayın.

### <a name="parameters"></a>Parametreler

- **açı**: işlem sinüsü için açı

### <a name="return-values"></a>Dönüş Değerleri

- **sinüs**: sağlanan açının sinüsü

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
INT my_angle = 80;

/* Compute sine of “my_angle”. */

#if defined(GUIX_5_4_0_COMPATIBILITY)
    INT scaled_angle = my_angle << 8;
#else
    GX_FIXED_VAL = GX_FIXED_VAL_MAKE(my_angle);
#endif

my_angle_sine = gx_utility_math_sin(scaled_angle);

/* “my_angle_sine” contains the sine of “my_angle”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_acos
- gx_utility_asin
- gx_utility_math_cos
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_math_sqrt"></a>gx_utility_math_sqrt

İşlem kare kökü

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_math_sqrt(UINT value);
```

### <a name="description"></a>Açıklama

Bu hizmet, sağlanan değerin kare kökünü hesaplar.

### <a name="parameters"></a>Parametreler

- **değer**: hesaplama kare kökünün değeri

### <a name="return-values"></a>Dönüş Değerleri

- **kare kök**: sağlanan değerin kare kökü

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
/* Compute square root of “my_value”. */
my_square_root = gx_utility_math_sqrt(my_value);

/* “my_square_root” contains the square root of “my_value”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_bidi_paragraph_reorder"></a>gx_utility_bidi_paragraph_reorder

BiDi metnini görüntüleme sırasına göre yeniden sırala

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_bidi_paragraph_reorder(GX_BIDI_TEXT_INFO *input_info, 
                                       GX_BIDI_RESOLVED_TEXT_INFO **resolved_info_head)
```

### <a name="description"></a>Açıklama

Bu hizmet, BiDi metnini görüntüleme sırasına yeniden sıralar. Metin çizim yazı tipi ve görüntüleme genişliği sağlanmışsa, ilk olarak satır bölünmesi uygulanır, her satıra göre işlem yeniden sıralama işlemi uygulanır. Girilen metin birden fazla paragraf içeriyorsa, hizmet metni paragraflarına keser, her bir paragrafın satır sonu ve yeniden sipariş sonucu bir liste olarak bağlanır.

### <a name="parameters"></a>Parametreler

- **input_info**: satır sonu ve metin yeniden sıralama için bilgi işaretçisi
- **resolved_info_head**: satır sonu ve belirtilen metnin her paragrafında oluşan sonuçları içeren bağlantılı listeye yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı bidi metin yeniden sıralama
- **GX_PTR_ERROR**: (0x07) geçersiz giriş işaretçileri
- **GX_SYSTEM_MEMORY_ERROR**: (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek
#### <a name="draw-single-line-bidi-text-to-canvas"></a>Tuvale tek hatlı bidi metni çiz
```C
VOID custom_widget_draw(GX_WIDGET *widget)
{
    GX_BIDI_TEXT_INFO input_info;
    GX_BIDI_RESOLVED_TEXT_INFO *resolved_info;
    GX_CHAR bidi_text[] = "Single Line String";
    
    input_info.gx_bidi_text_info_text.gx_string_ptr = bidi_text;
    input_info.gx_bidi_text_info_text.gx_string_length = sizeof(bidi_text) - 1;
    input_info.gx_bidi_text_info_font = GX_NULL;
    input_info.gx_bidi_text_info_display_width = -1;
    
    /* Reordering BiDi text. */
    status = gx_utility_bidi_paragraph_reorder(&input_info, &resolved_info);
    
    if(status == GX_SUCCESS)
    {
        /* Draw reordered bidi text to canvas. */
        gx_canvas_text_draw_ext(widget->gx_widget_size.gx_rectangle_left,
                                widget->gx_widget_size.gx_rectangle_top,
                                resolved_info.gx_bidi_resolved_text_info_text);

        /* Delete resolved information list. */
        gx_utility_bidi_resolved_text_info_delete(&resolved_info);
    }
}
```
#### <a name="draw-multi-line-bidi-text-to-canvas"></a>Tuvale çoklu satır bidi metni çiz
```C
VOID custom_widget_draw(GX_WIDGET *widget)
{
    GX_BIDI_TEXT_INFO input_info;
    GX_BIDI_RESOLVED_TEXT_INFO *resolved_info;
    GX_CHAR bidi_text[] = "Multi Line BiDi Text Display Example";
    GX_FONT *font;
    GX_RECTANGLE client;
    GX_VALUE display_width;
    INT index;
    GX_VALUE xpos;
    GX_VALUE ypos;
    
    /* Pickup the font. */
    gx_context_font_get(font_id, &font);
    gx_widget_client_get(widget, 2, &client);
    
    display_width = (GX_VALUE)(client.gx_rectangle_right - client.gx_rectangle_left + 1);
    
    input_info.gx_bidi_text_info_text.gx_string_ptr = bidi_text;
    input_info.gx_bidi_text_info_text.gx_string_length = sizeof(bidi_text) - 1;
    input_info.gx_bidi_text_info_font = font;
    input_info.gx_bidi_text_info_display_width = display_width;
    
    /* Reordering BiDi text. */
    status = gx_utility_bidi_paragraph_reorder(&input_info, &resolved_info);
    
    if(status == GX_SUCCESS)
    {
        xpos = client.gx_rectangle_left;
        ypos = client.gx_rectangle_top;
        
        /* Draw reordered bidi text to canvas. */
        for(index = 0; index < resolved_info.gx_bidi_resolved_text_info_total_lines; index++)
        {
            gx_canvas_text_draw_ext(xpos, ypos, &resolved_info.gx_bidi_resolved_text_info_text[index]);
        
            ypos += font->gx_font_line_height;
        }
        
        /* Delete resolved information list. */
        gx_utility_bidi_resolved_text_info_delete(&resolved_info);
    }
}
```

#### <a name="draw-multi-paragraph-bidi-text-to-canvas"></a>Tuvale çoklu paragraf bidi metni çiz
```C
VOID custom_widget_draw(GX_WIDGET *widget)
{
    GX_BIDI_TEXT_INFO input_info;
    GX_BIDI_RESOLVED_TEXT_INFO *resolved_info;
    GX_BIDI_RESOLVED_TEXT_INFO *next;
    GX_CHAR bidi_text[] = "Multi Paragraph\r BiDi Text Display Example";
    GX_FONT *font;
    GX_RECTANGLE client;
    GX_VALUE display_width;
    INT index;
    GX_VALUE xpos;
    GX_VALUE ypos;
    
    /* Pickup the font. */
    gx_context_font_get(font_id, &font);
    gx_widget_client_get(widget, 2, &client);
    
    display_width = (GX_VALUE)(client.gx_rectangle_right - client.gx_rectangle_left + 1);
    
    
    input_info.gx_bidi_text_info_text.gx_string_ptr = bidi_text;
    input_info.gx_bidi_text_info_text.gx_string_length = sizeof(bidi_text) - 1;
    input_info.gx_bidi_text_info_font = font;
    input_info.gx_bidi_text_info_display_width = display_width;
    
    /* Reordering BiDi text. */
    status = gx_utility_bidi_paragraph_reorder(&input_info, &resolved_info);
    
    if(status == GX_SUCCESS)
    {
        xpos = client.gx_rectangle_left;
        ypos = client.gx_rectangle_top;
        
        next = resolved_info;
        
        /* Draw reordered bidi text to canvas. */
        while(next)
        {
            for(index = 0; index < next.gx_bidi_resolved_text_info_total_lines; index++)
            {
                gx_canvas_text_draw_ext(xpos, ypos, &next.gx_bidi_resolved_text_info_text[index]);
            
                ypos += font->gx_font_line_height;
            }
            
            next = next->gx_bidi_resolved_text_info_next;
        }
        
        /* Delete resolved information list. */
        gx_utility_bidi_resolved_text_info_delete(&resolved_info);
    }
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_bidi_resolved_text_info_delete

## <a name="gx_utility_bidi_resolved_text_info_delete"></a>gx_utility_bidi_resolved_text_info_delete

Çözümlenen BiDi metin bilgisi listesini sil

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_bidi_resolved_text_info_delete(GX_BIDI_RESOLVED_TEXT_INFO **resolved_info_head)
```

### <a name="description"></a>Açıklama

Bu hizmet, gx_utility_bidi_paragraph_reorder tarafından döndürülen çözümlenmiş bilgi listesini siler.

### <a name="parameters"></a>Parametreler

- **resolved_info_head**: çözümlenen bidi metin bilgisi listesine yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı çözümlenmiş metin silme
- **GX_PTR_ERROR**: (0x07) geçersiz giriş işaretçileri
- **GX_SYSTEM_MEMORY_ERROR**: (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek
```C
VOID custom_widget_draw(GX_WIDGET *widget)
{
    GX_BIDI_TEXT_INFO input_info;
    GX_BIDI_RESOLVED_TEXT_INFO *resolved_info;
    GX_CHAR bidi_text[] = "Single Line String";
    
    input_info.gx_bidi_text_info_text.gx_string_ptr = bidi_text;
    input_info.gx_bidi_text_info_text.gx_string_length = sizeof(bidi_text) - 1;
    input_info.gx_bidi_text_info_font = GX_NULL;
    input_info.gx_bidi_text_info_display_width = -1;
    
    /* Reordering BiDi text. */
    status = gx_utility_bidi_paragraph_reorder(&input_info, &resolved_info);
    
    if(status == GX_SUCCESS)
    {
        /* Draw reordered bidi text to canvas. */
        gx_canvas_text_draw_ext(widget->gx_widget_size.gx_rectangle_left,
                                widget->gx_widget_size.gx_rectangle_top,
                                resolved_info.gx_bidi_resolved_text_info_text);

        /* Delete resolved information list. */
        gx_utility_bidi_resolved_text_info_delete(&resolved_info);
    }
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_bidi_paragraph_reorder

## <a name="gx_utility_pixelmap_resize"></a>gx_utility_pixelmap_resize

Pixelmap 'i yeniden boyutlandır

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_pixelmap_resize(
    GX_PIXELMAP *src,
    GX_PIXELMAP *destination, 
    INT width, 
    INT height);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pixelmap 'i yeniden boyutlandırır ve yeni bir pixelmap için bir işaretçi döndürür. Bu, pixelmap yeniden boyutlandırmanın sonucudur.

Bu hizmet, yeniden boyutlandırılan pixelmap verilerini tutmak için belleğin ayrılmasına izin vermek üzere gx_system_memory_allocator_set önceki kullanımını gerektirir.

### <a name="parameters"></a>Parametreler

- **src**: yeniden boyutlandırmak için pixelmap işaretçisine
- **hedef**: elde edilen pixelmap için hedef arabellek
- **Width**: elde edilen pixelmap 'in piksel cinsinden genişliği
- **Yükseklik**: elde edilen pixelmap 'in piksel cinsinden uzunluğu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı pixelmap yeniden boyutlandırma
- **GX_PTR_ERROR**: (0x07) geçersiz kaynak veya hedef pixelmap işaretçisi
- **GX_INVALID_VALUE**: (0x22) Genişlik veya yükseklik değeri geçerli değil
- **GX_NOT_SUPPORTED**: (0x28) kaynak pixelmap sıkıştırılmış biçimde
- **GX_SYSTEM_MEMORY_ERROR**: (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
GX_PIXLEMAP *des_pixelmap;

/* Resize “src_pixelmap” with specifiy width and height. */
status = gx_utility_pixelmap_resize(src_pixelmap,
    &des_pixelmap, 100, 200);

/* If status is GX_SUCCESS. “des_pixelmap” successfully load the
resulting pixelmap of resize. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift
- gx_canvas_pixelmap_rotate

## <a name="gx_utility_pixelmap_rotate"></a>gx_utility_pixelmap_rotate

Pixelmap 'i döndür

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_pixelmap_rotate(
    GX_PIXELMAP *src, INT angle,
    GX_PIXELMAP *destination,
    UINT *rot_cx, 
    UINT *rot_cy);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pixelmap döndürür ve pixelmap dönüşünün sonucu olan yeni bir pixelmap için bir işaretçi döndürür. Bir pixelmap 'i doğrudan tuvale döndürmek için gx_canvas_pixelmap_rotate () kullanın.

Bu hizmet, döndürülen pixelmap verilerini tutmak için belleğin ayrılmasına izin vermek üzere gx_system_memory_allocator_set önceki kullanımını gerektirir.

### <a name="parameters"></a>Parametreler

- **src**: döndürülecek pixelmap
- **açı**: dönüşünün derece cinsinden açısı
- **hedef**: elde edilen pixelmap için hedef arabellek
- **rot_cx**: hedef pixelmap 'e göre döndürme merkezinin x koordinatı alındı. Kaynak pixelmap 'e göre döndürme merkezinin x koordinatı ile başlatılmalıdır. Rot_cx GX_NULL, değer alınmayacak.
- **rot_cy**: hedef pixelmap 'e göre döndürme merkezinin y koordinatı alındı. Kaynak pixelmap 'e göre döndürme merkezinin y koordinatı ile başlatılmalıdır. Rot_cy GX_NULL, değer alınmayacak.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı pixelmap döndürme
- **GX_PTR_ERROR**: (0x07) geçersiz kaynak veya hedef pixelmap işaretçisi
- **GX_INVALID_VALUE**: (0x22) açı değeri 0
- **GX_INVALID_FORMAT**: (0x28) kaynak pixelmap sıkıştırılmış biçimde, bu desteklenmez
- **GX_SYSTEM_MEMORY_ERROR**: (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
rot_cx = source_rotate_center_x;
rot_cy = source_rotate_center_y;

/* rotate “src_pixelmap” by 30 degree in clockwise direction. */
status = gx_utility_pixelmap_rotate(src_pixelmap, 30,
    &des_pixelmap, &rot_cx, &rot_cy);

/* If status is GX_SUCCESS. “des_pixelmap” successfully load the
resulting pixelmap of rotation. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift
- gx_canvas_pixelmap_rotate

## <a name="gx_utility_pixelmap_simple_rotate"></a>gx_utility_pixelmap_simple_rotate

Pixelmap 'i döndür

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_pixelmap_simple_rotate(
    GX_PIXELMAP *src,
    INT angle,
    GX_PIXELMAP *destination,
    UINT *rot_cx,
    UINT *rot_cy);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir pixelmap 'i 90 derece, 180 derece veya 270 derecesi ile döndürür.

### <a name="parameters"></a>Parametreler

- **src**: döndürülecek pixelmap
- **açı**: dönüşünün derece cinsinden açısı
- **hedef**: elde edilen pixelmap için hedef arabellek
- **rot_cx**: hedef pixelmap 'e göre döndürme merkezinin x koordinatı alındı. Kaynak pixelmap 'e göre döndürme merkezinin x koordinatı ile başlatılmalıdır. Rot_cx GX_NULL, değer alınmayacak.
**rot_cy**: hedef pixelmap 'e göre döndürme merkezinin y koordinatı alındı. Kaynak pixelmap 'e göre döndürme merkezinin y koordinatı ile başlatılmalıdır. Rot_cy GX_NULL, değer alınmayacak.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) başarılı pixelmap döndürme
- **GX_PTR_ERROR**: (0x07) geçersiz kaynak veya hedef pixelmap işaretçisi
- **GX_INVALID_VALUE**: (0x22) açı değeri 0 veya 90, 180, 270 gibi basit bir açı değil
- **GX_INVALID_FORMAT**: (0x28) kaynak pixelmap sıkıştırılmış biçimde, bu desteklenmez
- **GX_SYSTEM_MEMORY_ERROR**: (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
rot_cx = source_rotate_center_x;
rot_cy = source_rotate_center_y;

/* rotate “src_pixelmap” by 90 degree in clockwise direction. */
status = gx_utility_pixelmap_simple_rotate(src_pixelmap, 90,
    &des_pixelmap,
    &rot_cx, &rot_cy);

/* If status is GX_SUCCESS. “des_pixelmap” successfully load the
resulting pixelmap of rotation. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_rectangle_center"></a>gx_utility_rectangle_center

Dikdörtgeni başka bir dikdörtgen içinde ortala

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_rectangle_center(
    GX_RECTANGLE *rectangle,
    GX_RECTANGLE *within_rectangle);
```

### <a name="description"></a>Açıklama

Bu hizmet dikdörtgeni başka bir dikdörtgen içinde ortalar.

### <a name="parameters"></a>Parametreler

- **dikdörtgen**: ortata dikdörtgen
- **within_rectangle**: içinde ortaya dikdörtgen

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) dikdörtgeni başarıyla ortalandı
- **GX_PTR_ERROR**: (0x07) geçersiz giriş dikdörtgeni işaretçisi
- **GX_INVALID_SIZE**: (0x19) geçersiz dikdörtgen boyutu

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
UINT status;

/* Center “my_inner_rectangle” inside of “my_outer_rectangle”.*/
status = gx_utility_rectangle_center(&my_inner_rectangle,
    &my_outer_rectangle);

/* Is status is GX_SUCCESS, “my_inner_rectangle” is centered
within “my_other_rectangle”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_rectangle_center_find"></a>gx_utility_rectangle_center_find

Dikdörtgenin merkezini bul

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_rectangle_center_find(
    GX_RECTANGLE *rectangle,
    GX_POINT *return_center);
```

### <a name="description"></a>Açıklama

Bu hizmet, dikdörtgenin merkezini bulur.

### <a name="parameters"></a>Parametreler

- **dikdörtgen**: dikdörtgen
- **return_center**: merkez noktası işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) dikdörtgenin merkezini başarıyla buldu
- **GX_PTR_ERROR**: (0x07) geçersiz giriş işaretçisi
- **GX_INVALID_SIZE**: (0x19) geçersiz dikdörtgen boyutu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT status;

GX_RECTANGLE my_rectangle;

GX_POINT my_center_point;

gx_utility_define(&my_rectangle, 0, 0, 100, 100);

/* Find center of “my_rectangle””. */

status = gx_utility_rectangle_center_find(&my_rectangle,
    &my_center_point);

/* If status is GX_SUCCESS, “my_center_point” is the center point
of “my_rectangle” (50, 50). */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_rectangle_combine"></a>gx_utility_rectangle_combine

İlk olarak iki dikdörtgeni birleştirin

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_rectangle_combine(
    GX_RECTANGLE *first_rectangle,
    GX_RECTANGLE *second_rectangle);
```

### <a name="description"></a>Açıklama

Bu hizmet birinci ve İkinci dikdörtgeni ilk dikdörtgende birleştirir. İlk dikdörtgen, ikincisini içerecek şekilde genişletilir.

### <a name="parameters"></a>Parametreler

- **first_rectangle**: ilk dikdörtgen ve Birleşik dikdörtgen
- **second_rectangle**: ikinci dikdörtgen

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) Iki dikdörtgeni başarıyla birleştirildi
- **GX_PTR_ERROR**: (0x07) geçersiz giriş işaretçisi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT status;

GX_RECTANGLE rect_a;

GX_RECTANGLE rect_b;

gx_utility_rectangle_define(&rect_a, 0, 0, 100, 100);
gx_utility_rectangle_define(&rect_b, 50, 50, 200, 200);

/* Combine “my_rectangle_a” to “my_rectangle_b”. */
status = gx_utility_rectangle_combine(&rect_a, &rect_b);

/* If status is GX_SUCCESS, “rect_a” is (0, 0, 200, 200) the merger
of the original “rect_a” and “rect_b”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_rectangle_compare"></a>gx_utility_rectangle_compare

İki dikdörtgeni karşılaştırın

### <a name="prototype"></a>Prototype

```C
GX_BOOL gx_utility_rectangle_compare( 
    GX_RECTANGLE *first_rectangle,
    GX_RECTANGLE *second_rectangle);
```

### <a name="description"></a>Açıklama

Bu hizmet, birinci ve İkinci dikdörtgeni karşılaştırır. Eşitse, bir GX_TRUE değeri döndürülür.

### <a name="parameters"></a>Parametreler

- **first_rectangle**: ilk dikdörtgen
- **second_rectangle**: ikinci dikdörtgen

### <a name="return-values"></a>Dönüş Değerleri

- **sonuç**: dikdörtgenler eşitse GX_TRUE, aksi takdirde GX_FALSE döndürülür.

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Compare “my_rectangle_a” to “my_rectangle_b”. */
result = gx_utility_rectangle_compare(&my_rectangle_a,
    &my_rectangle_b);

/* If result is GX_TRUE, the two rectangles are equal. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_rectangle_define"></a>gx_utility_rectangle_define

Dikdörtgen tanımlama

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_rectangle_define(
    GX_RECTANGLE *rectangle,
    GX_VALUE left,
    GX_VALUE top, 
    GX_VALUE right, 
    GX_VALUE bottom);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen şekilde bir dikdörtgen tanımlar.

### <a name="parameters"></a>Parametreler

- **dikdörtgen**: dikdörtgen denetim bloğu
- **sol**: sol üst koordinat
- **üst**: en üstteki koordinat
- **sağ**: en sağ koordinat
- **alt**: en altta bulunan koordinat

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) bir dikdörtgeni başarıyla tanımladı
- **GX_PTR_ERROR**: (0x07) geçersiz dikdörtgen işaretçisi

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
UINT status;

GX_RECTANGLE my_rect;

/* Define “my_rect”. */

status = gx_utility_rectangle_define(&my_rect, 10, 5, 200, 100);

/* If status is GX_SUCCESS, “my_rect” is defined. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_rectangle_overlap_detect"></a>gx_utility_rectangle_overlap_detect

Dikdörtgenlerin çakışmasını Algıla

### <a name="prototype"></a>Prototype

```C
GX_BOOL gx_utility_rectangle_overlap_detect(
    GX_RECTANGLE *first_rectangle,
    GX_RECTANGLE *second_rectangle,
    GX_RECTANGLE *return_overlap_area);
```

### <a name="description"></a>Açıklama

Bu hizmet, sağlanan dikdörtgenlerin çakışmasını algılar. Çakışma bulunursa, hizmet GX_TRUE ve çakışan dikdörtgeni döndürür.

### <a name="parameters"></a>Parametreler

- **first_rectangle**: ilk dikdörtgen
- **second_rectangle**: ikinci dikdörtgen
- **return_overlap_area**: örtüşen dikdörtgen alanı

### <a name="return-values"></a>Dönüş Değerleri

- **sonuç**: dikdörtgenler çakıştığında GX_TRUE, aksi takdirde GX_FALSE.

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
/* Detect overlap of “my_rectangle_a” and “my_rectangle_b”. */
result = gx_utility_rectangle_overlap_detect(&my_rectangle_a,
    &my_rectangle_b,
    &my_overlap_area);

/* If result is GX_TRUE, “my_overlap_area” specifies the area the
rectangles overlap. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_rectangle_point_detect"></a>gx_utility_rectangle_point_detect

Noktanın dikdörtgende yer alıyorsa Algıla

### <a name="prototype"></a>Prototype

```C
GX_BOOL gx_utility_rectangle_point_detect(
    GX_RECTANGLE *rectangle,
    GX_POINT point);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen noktanın dikdörtgen içinde olup olmadığını algılar. Nokta dikdörtgende yer alıyorsa, hizmet GX_TRUE döndürür.

### <a name="parameters"></a>Parametreler

- **dikdörtgen**: dikdörtgen
- **nokta**: nokta

### <a name="return-values"></a>Dönüş Değerleri

- **sonuç**: nokta dikdörtgende yer alıyorsa GX_TRUE, aksi takdirde GX_FALSE

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```c
GX_RECTANGLE my_rectangle;

GX_POINT my_point;

gx_utility_rectangle_define(&my_rectangle, 0, 0, 100, 100);

my_point.gx_point_x = 20; my_point.gx_point_y = 20;

/* Detect if point “my_point” is within “my_rectangle””. */
result = gx_utility_rectangle_point_detect(&my_rectangle,
    &my_point);

/* If result is GX_TRUE, “my_point” resides in the rectangle. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_rectangle_resize"></a>gx_utility_rectangle_resize

Dikdörtgeni büyüt

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_rectangle_resize(
    GX_RECTANGLE *rectangle,
    GX_VALUE adjust);
```

### <a name="description"></a>Açıklama

Bu hizmet, dikdörtgenin boyutunu belirtilen şekilde artırır.

### <a name="parameters"></a>Parametreler

- **dikdörtgen**: dikdörtgenin işaretçisi
- **Ayarla**: dikdörtgeni ayarlanacak miktar

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) dikdörtgeni başarıyla yeniden boyutlandırıldı
- **GX_PTR_ERROR**: (0x07) geçersiz giriş dikdörtgeni işaretçisi

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
UINT status;

/* Adjust “my_rectangle” by increasing 20 pixels on four sides */
status = gx_utility_rectangle_resize(&my_rectangle, 20);

/* If status is GX_SUCCESS, “my_rectangle” is 20 pixels larger. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect
- gx_utility_rectangle_shift

## <a name="gx_utility_rectangle_shift"></a>gx_utility_rectangle_shift

Kaydırma dikdörtgeni

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_rectangle_shift(
    GX_RECTANGLE *rectangle,
    GX_VALUE x_shift,
    GX_VALUE y_shift);
```

### <a name="description"></a>Açıklama

Bu hizmet, dikdörtgeni belirtilen değerlere kaydırır.

### <a name="parameters"></a>Parametreler

- **dikdörtgen**: SHIFT için dikdörtgen
- **x_shif**: x ekseninde kaydırma yapılacak piksel sayısı
- **y_shift**: y ekseninde kaydırma yapılacak piksel sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) dikdörtgeni başarıyla kaydırın
- **GX_PTR_ERROR**: (0x07) geçersiz giriş dikdörtgeni işaretçisi

### <a name="allowed-from"></a>İzin verilen

Tümü

### <a name="example"></a>Örnek

```C
UINT status;

/* Shift “my_rectangle”. */

status = gx_utility_rectangle_shift(&my_rectangle, 10, 20);

/* If status is GX_SUCCESS, “my_rectangle” has been shifted. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect

## <a name="gx_utility_string_to_alphamap"></a>gx_utility_string_to_alphamap

Dizeyi 8bpp bir String eşleme türü pixelmap (kullanım dışı) olarak işle

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_string_to_alphamap(
    const GX_CHAR *text, const
    GX_FONT *font, 
    GX_PIXELMAP *return_map);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_utility_string_to_alphamap_ext () kullanım dışı bırakılmıştır.

Bu hizmet, yalnızca alfa değerlerini içeren bir 8bpp pixelmap özel biçimi olan bir alfamap 'e bir metin dizesi işler. Bu hizmet genellikle gx_utility_pixelmap_rotate ve gx_canvas_pixelmap_draw ile birlikte kullanılarak döndürülen metni tuvale çizmektir.

Bu hizmet, sonuçta elde edilen harflerden eşleşme için gereken bellek boyutunu hesaplar ve dinamik olarak bellek ayırmak için uygulama tarafından tanımlanan gx_system_memory_allocator () işlevini çağırır. Uygulamanın bu hizmeti kullanmadan önce, genellikle program başlangıcında, bir noktada gx_system_memory_allocator_set () çağrısı gerekir.

Bir metin dizesi döndürülecektir ve tek bir kez tuvale çizildiyse, hizmet gx_canvas_rotated_text_draw () alternatif olarak sağlanır. gx_canvas_rotated_text_draw (), döndürülen metni tek bir işlemde işlemek için gx_utility_string_to_alphamap (), gx_utility_pixelmap_rotate () ve gx_canvas_pixelmap_draw () çağırır. Ancak, aynı metin çeşitli açılarda birden çok kez döndürülürse, gx_utility_string_to_alphmap API 'sini kullanarak bir kez daha verimli bir şekilde çizilecektir ve sonra sonuçta elde edilen harflerden oluşan Haritayı gerektiği gibi döndürün.

### <a name="parameters"></a>Parametreler

- **metin**: harflerden haritaya işlenecek metin dizesi
- **yazı tipi**: metni işlemek için kullanılacak yazı tipi
- **return_map**: çağırana döndürülecek GX_PIXELMAP işaretçisi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) bir metin dizesini bir alfamap 'e başarıyla işlendi
- **GX_PTR_ERROR**: (0x07) geçersiz giriş işaretçisi
- **GX_SYSTEM_MEMORY_ERROR**: (0x30) bellek ayırma/serbest bırakma işlevi tanımlı değil
- **GX_INVALID_STRING_LENGTH**: (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_PIXELMAP alphamap;

GX_PIXELMAP rotated_text;

INT xpos;

INT ypos;

gx_widget_font_get(widget, GX_FONT_ID_SCREEN_LABEL, &font);

/* render string to alphamap once */

gx_utility_string_to_alphamap("Hello World", font, &alphamap);

/* rotate and render the alphmap at multiple angles */

gx_utility_pixelmap_rotate(&alphamap, 45, &rotated_text,
    &xpos, &ypos);

gx_canvas_pixelmap_draw(10, 10, &rotated_text);

gx_utility_pixelmap_rotate(&alphamap, 135, &rotated_text,
    &xpos, &ypos);

gx_canvas_pixelmap_draw(100, 100, &rotated_text);

gx_utility_pixelmap_rotate(&alphamap, 300, &rotated_text,
    &xpos, &ypos);

gx_canvas_pixelmap_draw(200, 200, &rotated_text);
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_string_to_alphamap_ext

## <a name="gx_utility_string_to_alphamap_ext"></a>gx_utility_string_to_alphamap_ext

Dizeyi bir 8bpp harfler eşleme türü pixelmap olarak işle

### <a name="prototype"></a>Prototype

```C
UINT gx_utility_string_to_alphamap_ext(
    GX_CONST GX_STRING *string,
    GX_CONST GX_FONT *font, 
    GX_PIXELMAP *return_map);
```

### <a name="description"></a>Açıklama

Bu hizmet, yalnızca alfa değerlerini içeren bir 8bpp pixelmap özel biçimi olan bir alfamap 'e bir metin dizesi işler. Bu hizmet genellikle gx_utility_pixelmap_rotate ve gx_canvas_pixelmap_draw ile birlikte kullanılarak döndürülen metni tuvale çizmektir.

Bu hizmet, sonuçta elde edilen harflerden eşleşme için gereken bellek boyutunu hesaplar ve dinamik olarak bellek ayırmak için uygulama tarafından tanımlanan gx_system_memory_allocator () işlevini çağırır. Uygulamanın bu hizmeti kullanmadan önce, genellikle program başlangıcında, bir noktada gx_system_memory_allocator_set () çağrısı gerekir.

Bir metin dizesi döndürülecektir ve tek bir kez tuvale çizildiyse, hizmet gx_canvas_rotated_text_draw () alternatif olarak sağlanır. gx_canvas_rotated_text_draw (), döndürülen metni tek bir işlemde işlemek için gx_utility_string_to_alphamap (), gx_utility_pixelmap_rotate () ve gx_canvas_pixelmap_draw () çağırır. Ancak, aynı metin çeşitli açılarda birden çok kez döndürülürse, gx_utility_string_to_alphmap API 'sini kullanarak bir kez daha verimli bir şekilde çizilecektir ve sonra sonuçta elde edilen harflerden oluşan Haritayı gerektiği gibi döndürün.

### <a name="parameters"></a>Parametreler

- **dize**: harflerden haritaya işlenecek metin dizesi
- **yazı tipi**: metni işlemek için kullanılacak yazı tipi
- **return_map**: çağırana döndürülecek GX_PIXELMAP işaretçisi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS**: (0x00) bir metin dizesini bir alfamap 'e başarıyla işlendi
- **GX_PTR_ERROR**: (0x07) geçersiz giriş işaretçisi
- **GX_SYSTEM_MEMORY_ERROR**: (0x30) bellek ayırma/serbest bırakma işlevi tanımlı değil
- **GX_INVALID_STRING_LENGTH**: (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING string;

GX_PIXELMAP alphamap;

GX_PIXELMAP rotated_text;

INT xpos;

INT ypos;

gx_widget_font_get(widget, GX_FONT_ID_SCREEN_LABEL, &font);

string.gx_string_ptr = “Hello World”;

string.gx_string_length = strlen(string.gx_string_ptr);

/* render string to alphamap once */
gx_utility_string_to_alphamap_ext(&string, font, &alphamap);

/* rotate and render the alphmap at multiple angles */
gx_utility_pixelmap_rotate(&alphamap, 45, &rotated_text,
    &xpos, &ypos);

gx_canvas_pixelmap_draw(10, 10, &rotated_text);

gx_utility_pixelmap_rotate(&alphamap, 135, &rotated_text,
    &xpos, &ypos);

gx_canvas_pixelmap_draw(100, 100, &rotated_text);

gx_utility_pixelmap_rotate(&alphamap, 300, &rotated_text,
    &xpos, &ypos);

gx_canvas_pixelmap_draw(200, 200, &rotated_text);
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_utility_ltoa
- gx_utility_math_cos
- gx_utility_math_sin
- gx_utility_math_sqrt
- gx_utility_pixelmap_rotate
- gx_utility_pixelmap_simple_rotate
- gx_utility_rectangle_center
- gx_utility_rectangle_center_find
- gx_utility_rectangle_combine
- gx_utility_rectangle_compare
- gx_utility_rectangle_define
- gx_utility_rectangle_grow
- gx_utility_rectangle_overlap_detect
- gx_utility_rectangle_point_detect

## <a name="gx_vertical_list_children_position"></a>gx_vertical_list_children_position
### <a name="position-children-for-the-vertical-list"></a>Dikey liste için alt öğe Konumlandır

### <a name="prototype"></a>Prototype

```C
UINT gx_vertical_list_children_position(
    GX_VERTICAL_LIST *vertical_list)
```

### <a name="description"></a>Açıklama

Bu işlev, dikey liste için alt öğeleri konumlandırır.

### <a name="parameters"></a>Parametreler

- **vertical_list** Dikey liste denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) dikey listenin alt öğeleri başarıyla yerleştirildi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Position children in the vertical list */
status = gx_vertical_list_children_position (&vertical_list);

/* If status is GX_SUCCESS the children in the vertical list are positioned.. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_vertical_list_create
- gx_vertical_list_event_process
- gx_vertical_list_page_index_set
- gx_vertical_list_selected_index_get
- gx_vertical_list_selecgted_widget_get
- gx_vertical_list_selected_widget_get
- gx_vertical_list_selected_set
- gx_vertical_list_total_rows_set

## <a name="gx_vertical_list_create"></a>gx_vertical_list_create
### <a name="create-vertical-list"></a>Dikey liste oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_vertical_list_create(
    GX_VERTICAL_LIST *vertical_list,
    GX_CONST GX_CHAR *name, 
    GX_WIDGET *parent, 
    INT total_rows,
    VOID (*callback)(GX_VERTICAL_LIST *, GX_WIDGET *, INT),
    ULONG style, USHORT vertical_list_id,
    GX_CONST GX_RECTANGLE *size);
```
### <a name="description"></a>Açıklama

Bu hizmet dikey bir liste oluşturur.

GX_VERTICAL_LIST GX_WINDOW türetilir ve tüm gx_window API hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **vertical_list** Dikey liste pencere öğesi denetim bloğu
- **ad** Dikey listenin adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **total_rows** Dikey listedeki toplam satır sayısı
- **geri arama** Liste kaydırıldığında dikey liste tarafından çağrılacak bir işlev. Çağıran, başlangıçta görünür liste satırlarını dolduracak yeterli GX_WIDGET tabanlı alt öğe oluşturmamalıdır. Liste kaydırıldığında, bu işlev, sağlanan liste dizinine karşılık gelen liste alt öğelerini yeniden oluşturmak için çağrılır
- **Stil** ScrollBar pencere öğesinin stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **vertical_list_id** Uygulama tanımlı dikey listenin KIMLIĞI
- **Boyut** Dikey liste boyutları

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) dikey liste başarıyla oluşturuldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_VALUE** (0x22) satır sayısı geçerli değil
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create vertical list “my_list” with 20 rows. */
status = gx_vertical_list_create(&my_list, “my_list”, &my_parent,
                    20, callback, GX_STYLE_WRAP, MY_LIST_ID,
                    &size);

/* If status is GX_SUCCESS the vertical list “my_list” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_vertical_list_children_position
- gx_vertical_list_event_process
- gx_vertical_list_page_index_set
- gx_vertical_list_selected_index_get
- gx_vertical_list_selected_widget_get
- gx_vertical_list_selected_set
- gx_vertical_list_total_rows_set

## <a name="gx_vertical_list_event_process"></a>gx_vertical_list_event_process
### <a name="process-vertical-list-event"></a>Dikey liste olayını işle

### <a name="prototype"></a>Prototype

```C
UINT gx_vertical_list_event_process(GX_VERTICAL_LIST *list,
                                                      GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet dikey liste için bir olayı işler.

### <a name="parameters"></a>Parametreler

- **liste** Dikey liste pencere öğesi denetim bloğu
- **olay** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) dikey liste olayını başarıyla işledi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Process “my_event” for vertical list “my_list”. */
status = gx_vertical_list_event_process(&my_list, &my_event);

/* If status is GX_SUCCESS the event for vertical list “my_list” has been processed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_vertical_list_children_position
- gx_vertical_list_create
- gx_vertical_list_page_index_set
- gx_vertical_list_selected_index_get
- gx_vertical_list_selected_widget_get
- gx_vertical_list_selected_set
- gx_vertical_list_selected_set

## <a name="gx_vertical_list_page_index_set"></a>gx_vertical_list_page_index_set
### <a name="set-starting-page-index"></a>Başlangıç sayfası dizinini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_vertical_list_page_index_set(
    GX_VERTICAL_LIST *list,
    INT index);
```
### <a name="description"></a>Açıklama

Bu hizmet dikey liste için başlangıç dizinini ayarlar.

### <a name="parameters"></a>Parametreler

- **liste** Dikey liste pencere öğesi denetim bloğu
- **Dizin** Yeni üst Dizin

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) dikey liste için başlangıç sayfası dizinini başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi
- **GX_INVALID_VALUE** (0x22) geçersiz dizin değeri
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the starting page index of vertical list “my_list” to 4. */
status = gx_vertical_list_page_index_set(&my_list, 4);

/* If status is GX_SUCCESS the starting page index of “my_list” has
been set to 4. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_vertical_list_children_position
- gx_vertical_list_create
- gx_vertical_list_event_process
- gx_vertical_list_selected_index_get
- gx_vertical_list_selected_widget_get
- gx_vertical_list_selected_set
- gx_vertical_list_total_rows_set

## <a name="gx_vertical_list_selected_index_get"></a>gx_vertical_list_selected_index_get
### <a name="get-selected-index-from-vertical-list"></a>Seçili dizini dikey listeden Al

### <a name="prototype"></a>Prototype

```C
UINT gx_vertical_list_selected_index_get(
    GX_VERTICAL_LIST *vertical_list,
    INT *return_index);
```
### <a name="description"></a>Açıklama

Bu hizmet dikey listenin seçili dizinini döndürür

### <a name="parameters"></a>Parametreler

- **vertical_list** Dikey liste pencere öğesi denetim bloğu
- **return_index** Seçili dizinin dönüşü için hedef

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) dikey liste girişini başarıyla al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
INT current_selected_index;

/* Get the list entry at the current index of vertical list “my_list”. */
status = gx_vertical_list_selected_index_get(&my_list, &current_selected_index);

/* If status is GX_SUCCESS, “current_list_index” contains the index of the selected list item. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_vertical_list_children_position
- gx_vertical_list_create
- gx_vertical_list_event_process
- gx_vertical_list_page_index_set
- gx_vertical_list_selected_widget_get
- gx_vertical_list_selected_set
- gx_vertical_list_total_rows_set

## <a name="gx_vertical_list_selected_set"></a>gx_vertical_list_selected_set
### <a name="assign-the-selected-entry-in-a-vertical-list"></a>Seçili girdiyi dikey bir listede ata

### <a name="prototype"></a>Prototype

```C
UINT gx_vertical_list_selected_set(
    GX_VERTICAL_LIST *vertical_list,
    INT index);
```

### <a name="description"></a>Açıklama

Bu hizmet seçili girdiyi dikey bir listede atar. Gerekirse dikey liste, seçili girişi görünür hale getirmek için kayar.

### <a name="parameters"></a>Parametreler

- **vertical_list** Dikey liste pencere öğesi denetim bloğu
- **Dizin** Yeni liste girişinin dizin tabanlı konumu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) dikey liste girişini başarıyla ayarladı
- **GX_FAILURE** (0x10) giriş dizini listede bulunamadı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) dikey liste veya liste girişi pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the list entry of “my_list” to the child in line 12. */
status = gx_vertical_list_selected_set(&my_list, 12);

/* If status is GX_SUCCESS, the list entry of “my_list” has been successfully set to 12. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_vertical_list_children_position
- gx_vertical_list_create
- gx_vertical_list_event_process
- gx_vertical_list_page_index_get
- gx_vertical_list_selected_index_get
- gx_vertical_list_selected_widget_get
- gx_vertical_list_total_rows_set

## <a name="gx_vertical_list_selected_widget_get"></a>gx_vertical_list_selected_widget_get
### <a name="get-selected-widget-from-vertical-list"></a>Seçili pencere öğesini dikey listeden Al

### <a name="prototype"></a>Prototype

```C
UINT gx_vertical_list_selected_widget_get(
    GX_VERTICAL_LIST *vertical_list,
    GX_WIDGET **return_list_entry);
```
### <a name="description"></a>Açıklama

Bu hizmet dikey listenin seçili pencere öğesini döndürür. Listede alt pencere öğelerinin daha fazla satır varsa ve seçili alt pencere öğesi görünümden kaydırıldığında, pencere öğesi yeni bir liste girişi görüntüleyecek şekilde yeniden kullanıldığından, bu işlev GX_WIDGET işaretçi olarak GX_NULL döndürür.

### <a name="parameters"></a>Parametreler

- **vertical_list** Dikey liste pencere öğesi denetim bloğu
- **return_list_entry** Dönüş listesi girdisi pencere öğesi hedefi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) dikey liste girişini başarıyla al
- **GX_FAILURE** (0x10) seçili pencere öğesi görünümden kaydırıldı.
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_WIDGET *current_selected_widget;

/* Get the list entry at the current index of vertical list “my_list”. */
status = gx_vertical_list_selected_widget_get(&my_list, &current_selected_widget);

/* If status is GX_SUCCESS, “current_list_entry” contains a pointer to the currently selected widget. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_vertical_list_children_position
- gx_vertical_list_create
- gx_vertical_list_event_process
- gx_vertical_list_page_index_set
- gx_vertical_list_selected_index_get
- gx_vertical_list_selected_set
- gx_vertical_list_total_rows_set

## <a name="gx_vertical_list_total_rows_set"></a>gx_vertical_list_total_rows_set
### <a name="set-total-number-of-vertical-list-rows"></a>Dikey liste satırlarının toplam sayısını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_vertical_list_total_rows_set(
    GX_VERTICAL_LIST *vertical_list,
    INT count);
```
### <a name="description"></a>Açıklama

Bu hizmet Toplam liste satırı sayısını atar veya değiştirir.

### <a name="parameters"></a>Parametreler

- **vertical_list** Dikey liste pencere öğesi denetim bloğu
- **sayı** Yeni liste satırı sayısı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) dikey liste satır sayısını başarıyla ayarladı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) satır sayısı değeri geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set the list row count to 20 items. */
status = gx_vertical_list_total_rows_set(&my_list, 20);

/* If status is GX_SUCCESS, the total rows of “my_list” has been set to 20. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_vertical_list_children_position
- gx_vertical_list_create
- gx_vertical_list_event_process
- gx_vertical_list_page_index_set
- gx_vertical_list_selected_index_get
- gx_vertical_list_selected_widget_get
- gx_vertical_list_selected_set

## <a name="gx_vertical_scrollbar_create"></a>gx_vertical_scrollbar_create
### <a name="create-vertical-scrollbar"></a>Dikey kaydırma çubuğu oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_vertical_scrollbar_create(
    GX_SCROLLBAR *scrollbar,
    GX_CONST GX_CHAR *name, 
    GX_WINDOW *parent,
    GX_SCROLLBAR_APPEARANCE *appearance,
    ULONG style);
```
### <a name="description"></a>Açıklama

Bu hizmet dikey bir kaydırma çubuğu oluşturur.

### <a name="parameters"></a>Parametreler

- **kaydırma çubuğu** ScrollBar pencere öğesi denetim bloğu
- **ad** Kaydırma çubuğunun adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **Görünüm** Dikey ScrollBar pencere öğesinin görünümü.
- **Stil** Kaydırma çubuğunun stili.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı dikey kaydırma çubuğu oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET** (0x12) üst pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Create vertical scrollbar “my_scrollbar”. */
status = gx_vertical_scrollbar_create(&my_scrollbar,
                          “my_vertical_scrollbar”,
                          &my_parent, &scrollbar_appearance,
                          GX_STYLE_ENABLED);

/* If status is GX_SUCCESS the vertical scrollbar “my_scrollbar” has been created. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_horizontal_scrollbar_create
- gx_scrollbar_draw
- gx_scrollbar_event_process
- gx_scrollbar_limit_check
- gx_scrollbar_reset

## <a name="gx_widget_allocate"></a>gx_widget_allocate
### <a name="allocate-a-widget-control-block"></a>Pencere öğesi denetim bloğu ayır

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_allocate(
    GX_WIDGET **control_block,
    ULONG memsize);
```
### <a name="description"></a>Açıklama

Bu hizmet, uygulama tanımlı bellek ayırma işlevini çağırarak bir pencere öğesi denetim bloğunu dinamik olarak ayırır. Bu hizmet, Gux Studio özellikleri görünümünde "dinamik ayırma" özelliği seçildiğinde, denetim bloğunu dinamik olarak ayırmak için Gux Studio tarafından oluşturulan işlevler tarafından kullanılır.

### <a name="parameters"></a>Parametreler

- **control_block** Döndürülen denetim bloğu işaretçisine yönelik işaretçi
- **memsize** Denetim blok boyutu, bayt cinsinden

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi ayırma
- **GX_SYSTEM_MEMORY_ERROR** (0x30) bellek ayırıcısı tanımlı değil veya bellek ayırma başarısız oldu
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_MEMORY_SIZE** (0x29) bellek boyutu geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_TEXT_BUTTON *button;

/* Attach “my_widget” to “my_parent”. */
status = gx_widget_allocate(&button, sizeof(GX_TEXT_BUTTON));

/* If status is GX_SUCCESS the button widget control block is allocated. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_attach"></a>gx_widget_attach
### <a name="attach-widget-to-its-parent"></a>Pencere öğesini üst öğesine Ekle

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_attach(
    GX_WIDGET *parent, 
    GX_WIDGET *widget);
```
### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesini belirtilen üst öğeye iliştirir. Pencere öğesi zaten başka bir üst öğeye eklenmişse, ilk olarak ayrılır. Pencere öğesi zaten aynı üst öğeye eklenmişse, işlev hiçbir şey yapmaz.

Pencere öğesi, üstünün z sıralaması bakımından en üst alt öğesi olur. Eşdüzey pencere öğeleri çakışırsa, bu pencere öğesi eşdüzey öğelerinin üzerine çizilir. Yeni pencere öğesini z düzeninin arkasına koymak için gx_widget_back_attach veya gx_widget_back_move kullanın.

### <a name="parameters"></a>Parametreler

- **üst öğe** Üst pencere öğesi işaretçisi
- **pencere öğesi** Alt pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi iliştirme
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) üst öğe veya pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Attach “my_widget” to “my_parent”. */
status = gx_widget_attach(&my_parent, &my_widget);

/* If status is GX_SUCCESS the widget “my_widget” is attached to “my_parent”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_background_draw"></a>gx_widget_background_draw
### <a name="draw-a-widget-background"></a>Pencere öğesi arka planı çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_widget_background_draw(GX_WIDGET *widget);
```
### <a name="description"></a>Açıklama

Bu hizmet, bir pencere öğesi arka planının düz renk doldurmasını gerçekleştirir. Bu hizmet gx_widget_draw işlevi tarafından otomatik olarak çağrılır, ancak özelleştirilmiş bir pencere öğesi çizim işlevinin bir parçası olarak uygulama tarafından da çağrılabilir.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Çizilecek pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom widget draw function. */

VOID my_widget_draw(GX_WIDGET * widget)
{
    /* Call default widget background draw. */
    gx_widget_background_draw(widget);

    /* Add your own drawing here. */

    /* Draw child widgets. */
    gx_widget_children_draw(widget);
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_back_attach"></a>gx_widget_back_attach
### <a name="attach-widget-to-its-parent"></a>Pencere öğesini üst öğesine Ekle

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_back_attach(
    GX_WIDGET *parent, 
    GX_WIDGET *widget);
```
### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesini belirtilen üst öğeye iliştirir. Pencere öğesi zaten başka bir üst öğeye eklenmişse, ilk olarak ayrılır. Pencere öğesi zaten aynı üst öğeye eklenmişse, işlev hiçbir şey yapmaz.

Pencere öğesi, üst öğenin z sıralaması bakımından en alt alt öğesi olur. Eşdüzey pencere öğeleri çakışırsa bu pencere öğesi bu eşdüzey öğelerinin arkasına çizilir. Yeni pencere öğesini z düzeninin önüne koymak için gx_widget_attach veya gx_widget_front_move kullanın.

### <a name="parameters"></a>Parametreler

- **üst öğe** Üst pencere öğesi işaretçisi
- **pencere öğesi** Alt pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi iliştirme
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) üst öğe veya pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Attach “my_widget” to “my_parent”. */
status = gx_widget_back_attach(&my_parent, &my_widget);

/* If status is GX_SUCCESS the widget “my_widget” is attached to “my_parent”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_back_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_back_move"></a>gx_widget_back_move
### <a name="move-widget-to-back"></a>Pencere öğesini arkaya taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_back_move(
    GX_WIDGET *widget,
    GX_BOOL *return_widget_moved);
```
### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesini üst öğe pencere öğelerinin Z düzeninde arka arkaya hareket ettirir.

### <a name="parameters"></a>Parametreler

- **üst öğe** Üst pencere öğesi işaretçisi
- **return_widget_moved** Pencere öğesinin taşındığını belirten bayrak hedefi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi geri git
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_NO_CHANGE** (0x08) hiçbir değişiklik uygulanmadı
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move “my_widget” to the back. */
status = gx_widget_back_move(&my_widget, &moved_flag);

/* If status is GX_SUCCESS and “moved_flag” is GX_TRUE, the widget “my_widget” was moved to the back. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_block_move"></a>gx_widget_block_move
### <a name="move-a-rectangular-block-of-pixels"></a>Dikdörtgen bir piksel bloğunu taşıyın

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_block_move(
    GX_WIDGET *widget,
    GX_RECTANGLE *block,
    INT xshift, INT yshift);
```

### <a name="description"></a>Açıklama

Bu hizmet dikdörtgen bir piksel bloğunu taşıdıkça. Bu hizmet genellikle hızlı kaydırma uygulamak için kullanılır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Blok taşıma isteyen pencere öğesi işaretçisi
- **blok** Taşınacak dikdörtgen sınırlayıcı bloğu
- **xshift** X kaydırma miktarı piksel cinsinden
- **yılötele** Piksel cinsinden y kaydırma miktarı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi geri git
- **GX_INVALID_CANVAS** (0x20) pencere öğesi tuvali bulunamadı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move a block of pixels 20 pixels to the right. */
status = gx_widget_block_move(&my_widget, &size, 20, 0);

/* If status is GX_SUCCESS the block of pixels was moved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_border_draw"></a>gx_widget_border_draw
### <a name="draw-widget-border"></a>Pencere öğesi kenarlığını çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_widget_border_draw(
    GX_WIDGET *widget,
    GX_COLOR border_color,
    GX_COLOR upper_fill, 
    GX_COLOR lower_fill, 
    GX_BOOL fill);
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesi kenarlığını çizer. Bu hizmet normalde pencere öğesi çizim işlevinin bir parçası olarak çağrılır. Bu hizmet, pencere öğesi kenarlık stili bayraklarını hiçbir sınır, ince bir kenarlık, yükseltilmiş bir kenarlık, bir kenar kenarlığı veya kalın bir kenarlık çizmek için yorumlar.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **border_color** Kenarlık rengi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.
- **upper_fill** Üst dolgunun rengi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.
- **lower_fill** Alt dolgunun rengi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.
- **doldur** Bu Boole bayrağı, pencere öğesi alanının sağlanan dolgu renkleriyle doldurulup doldurulmayacağını gösterir. Bu değer GX_FALSE ise yalnızca pencere öğesi kenarlığı çizilir.

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom widget draw function. */

VOID my_widget_draw(GX_WIDGET * widget)
{
      /* Call widget border draw. */
      gx_widget_border_draw(widget, GX_COLOR_BLACK,
                            GX_COLOR_GREEN, GX_COLOR_BLUE,
                            GX_TRUE);

      /* Add your own drawing here. */

      /* Draw child widgets. */
      Gx_widget_children_draw(widget);
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_border_style_set"></a>gx_widget_border_style_set
### <a name="set-widget-border-style"></a>Pencere öğesi kenarlık stilini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_border_style_set(
    GX_WIDGET *widget, 
    ULONG style);
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesi kenarlık stilini ayarlar.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **Stil** Kenarlık stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi kenarlık stili kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set border style of “my_widget”. */
status = gx_widget_border_style_set(&my_widget,
                                    GX_STYLE_BORDER_RAISED);

/* If status is GX_SUCCESS the widget “my_widget” border style has been set. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_border_width_get"></a>gx_widget_border_width_get
### <a name="get-widget-border-width"></a>Pencere öğesi kenarlık genişliğini al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_border_width_get(
    GX_WIDGET *widget,
    GX_VALUE *return_width);
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesi kenarlık genişliğini alır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **return_width** Pencere öğesi kenarlık genişliği için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) kenarlık genişliği başarıyla alındı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_VALUE my_width;

/* Get border width of “my_widget”. */
status = gx_widget_border_width_get(&my_widget, &my_width);

/* If status is GX_SUCCESS, “my_width” contains the border width of the widget “my_widget”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_canvas_get"></a>gx_widget_canvas_get
### <a name="get-widget-canvas"></a>Pencere öğesi tuvali al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_canvas_get(
    GX_WIDGET *widget,
    GX_CANVAS **return_canvas)
```
### <a name="description"></a>Açıklama

Bu hizmet, bu pencere öğesinin üzerinde işlendiği tuvale bir işaretçi döndürür.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **return_canvas** Pencere öğesinin tuvali için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi tuvali al
- **GX_FAILURE** (0x10) pencere öğesi tuvali bulunamadı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Get canvas associated with “my_widget”. */
status = gx_widget_canvas_get(&my_widget, &my_canvas);

/* If status is GX_SUCCESS, “my_canvas” contains the canvas of the widget “my_widget”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_child_detect"></a>gx_widget_child_detect
### <a name="detect-widget-child"></a>Pencere öğesi alt öğesini Algıla

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_child_detect(
    GX_WIDGET *parent, 
    GX_WIDGET *child,
    GX_BOOL *return_detect);
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesinin üst pencere öğesinin bir alt öğesi olup olmadığını algılar. Bu hizmet alt öğeleri aramak için önemlidir ve üst pencere öğesi alt pencere öğesinin bir üst öğesiyse TRUE değerini döndürür.

### <a name="parameters"></a>Parametreler

- **üst öğe** Üst pencere öğesi işaretçisi
- **alt öğe** Alt pencere öğesi işaretçisi
- **return_detect** Algılama için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi alt algılama
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) üst öğe veya alt pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_BOOL detected;

/* Determine if “my_child” is a child of “my_widget”. */
status = gx_widget_child_detect(&my_widget, &my_child, &detected);

/* If status is GX_SUCCESS and “detected” is GX_TRUE, “my_child” is a child of widget “my_widget”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_children_draw"></a>gx_widget_children_draw
### <a name="draw-widget-children"></a>Pencere öğesi alt öğeleri çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_widget_children_draw(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet üst pencere öğesinin tüm alt öğelerini çizer. Bu hizmet, normalde tüm standart pencere öğesi çizim işlevleri tarafından çağrılır ve alt pencere öğelerinin özel ana pencere öğesi türüne eklenmesine izin vermek için herhangi bir özel çizim işlevi tarafından çağrılabilir.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom widget draw function. */

VOID my_widget_draw(GX_WIDGET * widget)
{
        /* Call default widget background draw. */
        gx_widget_background_draw(widget);

        /* Add your own drawing here. */

        /* Draw child widgets. */
        gx_widget_children_draw(widget);
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_client_get"></a>gx_widget_client_get
### <a name="get-widget-client-area"></a>Pencere öğesi istemci alanını al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_client_get(
    GX_WIDGET *widget,
    GX_VALUE border_width,
    GX_RECTANGLE *return_client_area);
```
### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesinin istemci alanını genel pencere öğesi boyutundan pencere öğesi kenarlık genişliğini çıkararak hesaplar.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **border_width** Pencere öğesi kenarlığının genişliği
- **return_client_area** İstemci alanı döndürme hedefi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi istemci alanı Get
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0x22) pencere öğesi kenarlığı geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RECTANGLE client_area
/* Get client area of widget “my_widget”. */
status = gx_widget_client_get(&my_widget, my_widget_width,
                              &client_area);

/* If status is GX_SUCCESS, the “client_area” is the client area of “my_widget”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_color_get"></a>gx_widget_color_get
### <a name="get-color"></a>Renk al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_color_get(
    GX_WIDGET *widget,
    GX_RESOURCE_ID resource_id,
    GX_COLOR *return_color);
```

### <a name="description"></a>Açıklama

Bu hizmet, sağlanan kaynak KIMLIĞIYLE ilişkili rengi alır. Bu hizmet yalnızca görünür pencere öğeleri tarafından çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi denetim bloğu işaretçisi
- **resource_id** Rengin kaynak KIMLIĞI. **Ek B** önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **return_color** Renge yönelik hedefin işaretçisi. **Ek A** önceden tanımlanmış renkler içerir. Uygulamanın de özel renkler ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı renk al
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CANVAS** (0x20) pencere öğesi tuvali geçerli değil veya pencere öğesi görünmez
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_COLOR actual_color;

/* Get color for resource ID MY_FIRST_COLOR_ID. */
status = gx_widget_color_get(my_widget, MY_FIRST_COLOR_RESOURCE_ID,
                            &actual_color);

/* If status is GX_SUCCESS the actual color is contained in “actual_color”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_font_get
- gx_widget_pixelmap_get

## <a name="gx_widget_create"></a>gx_widget_create
### <a name="create-widget"></a>Pencere öğesi oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_create(
    GX_WIDGET *widget, 
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent,
    ULONG style, 
    USHORT widget_id,
    GX_CONST GX_RECTANGLE *size);
```
### <a name="description"></a>Açıklama

Bu hizmet bir pencere öğesi oluşturur.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **ad** Pencere öğesinin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **Stil** Biçim. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **widget_id** Pencere öğesinin uygulama tanımlı KIMLIĞI
- **Boyut** Pencere öğesinin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET** (0x12) üst pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_WIDGET my_widget;
GX_RECTANGLE size;

gx_utility_rectangle_define(&size, 0, 0, 100, 100);

/* Get client area of widget “my_widget”. */
status = gx_widget_create(&my_widget, "my widget",
                          &my_parent_window, GX_STYLE_BORDER_RAISED, MY_WIDGET_ID, &size);

/* If status is GX_SUCCESS, the widget “my_widget” has been created. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_created_test"></a>gx_widget_created_test
### <a name="test-if-widget-created"></a>Pencere öğesi oluşturulduysa test

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_created_test(
    GX_WIDGET *widget,
    GX_BOOL *return_test);
```
### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesinin daha önce oluşturulup oluşturulmadığını belirlemede sınar. Herhangi bir hatayla karşılaşılmadıysa, pencere öğesinin henüz oluşturulup oluşturulmadığına bakılmaksızın bu işlev GX_SUCCESS döndürür. Testin sonucu return_test işaretçisidir.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **return_test** Test sonucu için hedef

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı test tamamlama
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_BOOL was_created;

/* Test to see if widget “my_widget” is created. */
status = gx_widget_created_test(&my_widget, &was_created);

/* If status is GX_SUCCESS, no error occurred. If “was_created” is
GX_TRUE, the widget “my_widget” has been created. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_delete"></a>gx_widget_delete
### <a name="delete-widget"></a>Pencere öğesini Sil

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_delete(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesini siler. Pencere öğesi denetim bloğu dinamik olarak ayrılmışsa gx_system_memory_free hizmeti, dinamik olarak ayrılan depolama alanını serbest bırakmak için çağrılır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi silme GX_CALLER_ERROR (0x11) bu işlevin geçersiz çağıranı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_SYSTEM_MEMORY_ERROR** (0x30) bellek boş işlevi tanımlı değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Delete widget “my_widget”. */
status = gx_widget_delete(&my_widget);

/* If status is GX_SUCCESS the widget “my_widget” has been deleted. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_detach"></a>gx_widget_detach
### <a name="detach-widget-from-parent"></a>Pencere öğesini üst öğeden ayır

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_detach(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesini üst öğesinden ayırır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi ayırma GX_CALLER_ERROR (0x11) bu işlevin geçersiz çağıranı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Detach widget “my_widget” from its parent. */
status = gx_widget_detach(&my_widget);

/* If status is GX_SUCCESS the widget “my_widget” has been detached. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_draw"></a>gx_widget_draw
### <a name="draw-widget"></a>Pencere öğesi çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_widget_draw(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesini çizer. Bu işlev normalde Gux tuval yenileme mekanizması tarafından dahili olarak çağrılır, ancak özel çizim işlevlerini uygulamaya yardımcı olmak için uygulamaya sunulur.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom widget draw function. */

VOID my_custom_widget_draw(GX_WIDGET *widget)
{
      /* Call default widget draw. */
      gx_widget_draw(widget);

      /* Add your own drawing here. */
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_draw_set"></a>gx_widget_draw_set
### <a name="assign-the-widget-drawing-function"></a>Pencere öğesi çizim işlevini ata

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_draw_set(
    GX_WIDGET *widget,
    VOID (*drawing_function) (GX_WIDGET *));
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesinin varsayılan çizim işlevini geçersiz kılar.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **drawing_function** Çizim işlevine yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi çizim işlevi geçersiz kılma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Define a custom drawing function. */
VOID my_drawing_function(GX_WIDGET *widget)
{
      /* Add your own drawing here. */
}

/* Set the drawing function of widget “my_widget” to “my_drawing_function”. */
status = gx_widget_draw_set(&my_widget, my_drawing_function);

/* If status is GX_SUCCESS the widget “my_widget” has the drawning function “my_drawing_function”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_event_generate"></a>gx_widget_event_generate
### <a name="generate-widget-event"></a>Pencere öğesi olayı oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_event_generate(
    GX_WIDGET *widget, 
    USHORT event_type, LONG value);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirli bir tür veya GX_EVENT sınıfı olan GX_SIGNAL bir olay türü oluşturur. gx_widget_event_generate (), 16 bit pencere öğesi KIMLIĞINI, geçirilen event_type ile birlikte tek bir 32 bit GX_EVENT. gx_event_type değerine kodluyor. Değer parametresi, oluşturulan gx_event kodlandı. gx_event_payload gx_event_payload.gx_event_longdata alanı.

Oluşturulan event.gx_event_target alanı her zaman çağıran pencere öğesinin üst öğesi ile yüklenir, yani oluşturulan olay her zaman ilk olarak oluşturma pencere öğesinin üst öğesine gönderilir.

Gx_widget_event_generate yalnızca GX_SIGNAL Range olay türlerini göndermek için kullanılması gerektiğini unutmayın. Kullanıcı tanımlı olay türleri dahil tüm diğer olay türleri için, Gux olay kuyruğuna gönderilen olayın her alanı üzerinde tam denetim veren gx_system_event_send () API 'sini kullanın.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **event_type** Olay türü. **Ek E** , önceden tanımlanmış Gux olaylarını içerir. Uygulama tarafından ek olaylar eklenebilir.
- **değer** Ek olay bilgileri

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi olay oluşturma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Generate a redraw event for widget “my_widget”. */
status = gx_widget_event_generate(&my_widget, GX_EVENT_REDRAW, 0);

/* If status is GX_SUCCESS the redraw event for widget “my_widget” has been generated. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get
- gx_system_event_send

## <a name="gx_widget_event_process"></a>gx_widget_event_process
### <a name="process-widget-event"></a>İşlem pencere öğesi olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_event_process(
    GX_WIDGET *widget, 
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu, tüm pencere öğeleri için varsayılan olay işleme işlevidir. Özel bir olay işleme işlevi yazıldığında, herhangi bir olay türü için varsayılan eylem, her zaman Olayı bir pencere öğesinin temel aldığı pencere öğesi türüne iletmektir. En temel GX_WIDGET türüne dayalı pencere öğeleri varsayılan olay işleme işlevi olarak gx_widget_event_process kullanır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **olay** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi olay işleme
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Process event “my_event” for widget “my_widget”. */
status = gx_widget_event_process(&my_widget, &my_event);

/* If status is GX_SUCCESS the event “my_event” for widget “my_widget” has been processed. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_event_process_set"></a>gx_widget_event_process_set
### <a name="set-event-processing-function-of-widget"></a>Pencere öğesinin olay işleme işlevini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_event_process_set(
    GX_WIDGET *widget,
    UINT (*event_processing) (GX_WIDGET *, GX_EVENT *));
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesinin olay işleme işlevini geçersiz kılar.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **event_processing** Yeni olay işleme işlevine yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi olay işleme geçersiz kılma
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
UINT my_event_process(GX_TREE_VIEW *tree_view,
                      GX_EVENT *event)
{
      UINT status = GX_SUCCESS;

      switch(event->gx_event_type)
      {
      case xyz:
            /* Insert custom event handling here */
            break;

      default:
            /* Pass all other events to the default tree view
               event processing */
            status = gx_tree_view_event_process(tree_view, event);
            break;
      }
      return status;
}

/* Use “my_event_process” to process events for widget “my_tree_view”. */
status = gx_widget_event_process_set((GX_WIDGET *)&my_tree_view,
                    (VOID (*)(GX_WIDGET *))my_event_process);

/* If status is GX_SUCCESS all event processing for widget “my_tree_view” is handled by “my_event_process”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_event_to_parent"></a>gx_widget_event_to_parent
### <a name="send-event-to-widgets-parent"></a>Etkinliği pencere öğesinin üst öğesine gönder

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_event_to_parent(
    GX_WIDGET *widget,
    GX_EVENT *event);
```
### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesinin üst öğesine bir olay gönderir.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **olay** Olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) olayı pencere öğesinin üst öğesine başarıyla gönderildi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Send my_event to the widget’s parent */
status = gx_widget_event_to_parent(&my_widget, my_event);

/* If status is GX_SUCCESS the event has been delivered to the parent of my_widget. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_fill_color_set"></a>gx_widget_fill_color_set
### <a name="set-widget-background-color"></a>Pencere öğesi arka plan rengini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_fill_color_set(
    GX_WIDGET *widget,
    GX_RESOURCE_ID normal_color_id,
    GX_RESOURCE_ID selected_color_id,
    GX_RESOURCE_ID disabled_color_id);
```
### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesi arka plan renklerini ayarlar.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **normal_color_id** Normal durumdaki Fill renginin kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **selected_color_id** Pencere öğesi odaklanıldığında, Fill Color kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.
- **disabled_color_id** Stil GX_STYLE_ENABLED ayarlanmamışsa, Fill Color kaynak KIMLIĞI. **Ek A** , önceden tanımlanmış renk kaynak kimliklerini içerir. Uygulamanın özel renk kaynak kimlikleri de ekleyebileceğini unutmayın.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) pencere öğesi dolgusu rengi başarıyla ayarlandı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set background of “my_widget”. */
status = gx_widget_fill_color_set(&my_widget,
                    GX_COLOR_ID_NORMAL_FILL,
                    GX_COLOR_ID_SELECTED_FILL,
                    GX_COLOR_ID_DISABLED_FILL);

/* If status is GX_SUCCESS the widget “my_widget” background has been set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_create
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_find"></a>gx_widget_find
### <a name="find-child-widget-of-parent-widget"></a>Üst pencere öğesinin alt pencere öğesini bul

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_find(
    GX_WIDGET *parent, 
    USHORT widget_id,
    INT search_depth, 
    GX_WIDGET **return_widget);
```
### <a name="description"></a>Açıklama

Bu hizmet, istenen KIMLIK değeri ile bir pencere öğesi arayan belirtilen üst öğenin alt öğelerinde arama yapar.

### <a name="parameters"></a>Parametreler

- **üst öğe** Aramanın başlatıldığı üst pencere öğesi işaretçisi
- **widget_id** Aranacak pencere öğesi KIMLIĞI
- **search_depth** İşlevin alt pencere öğelerini arayacaktır özyinelemeli iç içe geçme düzeyini tanımlar. Bu değer <= 0 ise, yalnızca üst pencere öğesinin anlık alt öğeleri aranır. Bu değer GX_SEARCH_DEPTH_INFINITE, tüm alt pencere öğelerinin tüm alt öğeleri, göreli olarak aranır. 0 > başka bir değer için bu değer, iç içe geçmiş bu işlevin, istenen pencere öğesi KIMLIĞI için alt pencere öğeleri arasında ne kadar arama yapılacağını sınırlandırır.
- **return_widget** Bulunan pencere öğesi için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi bul
- **GX_NOT_FOUND** (0x09) pencere öğesi kuruluş değil
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_WIDGET *widget_found;

/* Find widget “my_widget”. */
status = gx_widget_find(&my_widget, GX_SEARCH_DEPTH_INFINITE
                        MY_WIDGET_ID, &widget_found);

/* If status is GX_SUCCESS, the pointer “widget_found” contains the pointer to the widget found. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_first_child_get"></a>gx_widget_first_child_get
### <a name="return-pointer-to-first-child-widget"></a>İlk alt pencere öğesine İşaretçiyi döndür

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_first_child_get(
    GX_WIDGET *parent,
    GX_WIDGET **widget_return);
```
### <a name="description"></a>Açıklama

GUX, üst ve alt pencere öğelerinin yapılandırılmış bir listesini tutar. Bu hizmet, üst öğenin ilk alt öğesi için bir işaretçi döndürür.

### <a name="parameters"></a>Parametreler

- **üst öğe** Üst pencere öğesi işaretçisi
- **widget_return** Pencere öğesi işaretçisi döndürme işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) işaretçisi döndü
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Retrieve child widget pointer. */

GX_WIDGET *get_child_widget(GX_WIDGET *parent)
{
      GX_WIDGET *child;
      UINT status;

      status = gx_widget_first_child_get(parent, &child);
      if (status == GX_SUCCESS)
      {
            return child;
      }
      return GX_NULL;
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_last_child_get
- gx_widget_next_sibling_get
- gx_widget_parent_get
- gx_widget_previous_sibling_get
- gx_widget_top_visible_child_find

## <a name="gx_widget_focus_next"></a>gx_widget_focus_next
### <a name="move-focus-to-next-widget-in-navigation-order"></a>Odağı gezinti sırasında sonraki pencere öğesine taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_focus_next(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet, odağı kabul eden pencere öğelerinin bağlantılı listesinde odağı sonraki eşdüzey pencere öğesine kaydırır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) odak taşındı
- **GX_FAILURE** (0x00) odak taşınmadı
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move focus to next widget in navigation order. */ status =
gx_widget_focus_next(&my_widget);

/* If status is GX_SUCCESS the focus has been moved to the next
widget in the navigation order */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_focus_previous

## <a name="gx_widget_focus_previous"></a>gx_widget_focus_previous
### <a name="move-focus-to-previous-widget-in-navigation-order"></a>Odağı gezinti sırasında önceki pencere öğesine taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_focus_previous(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet, odağı gezinti sırasında önceki pencere öğesine kaydırır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Geçerli olan pencere öğesi işaretçisi giriş odağa sahip.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) odak taşındı
- **GX_FAILURE** (0x00) odak taşınmadı

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Move focus to previuos widget in navigation order. */ status =
gx_widget_focus_previous(&my_widget);

/* If status is GX_SUCCESS the input focus has been moved to the
previous widget. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_focus_next

## <a name="gx_widget_font_get"></a>gx_widget_font_get
### <a name="get-font-for-specified-resource-id"></a>Belirtilen kaynak KIMLIĞI için yazı tipi al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_font_get(
    GX_WIDGETG *widget,
    GX_RESOURCE_ID resource_id,
    GX_FONT **return_font);
```
### <a name="description"></a>Açıklama

Bu hizmet, bu pencere öğesinin görünür olduğu ekran yazı tipi tablosundan belirtilen kaynak KIMLIĞIYLE ilişkili yazı tipini alır. Bu işlev yalnızca görünür bir pencere öğesi tarafından çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi denetim bloğu işaretçisi
- **resource_id** Yazı tipinin kaynak KIMLIĞI
- **return_font** Yazı tipi işaretçisi için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) yazı tipi başarıyla alındı
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CANVAS** (0x20) pencere öğesi tuvali geçerli değil veya pencere öğesi görünmez
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_FONT *my_font;
/* Get font for MY_FONT_ID. */
status = gx_widget_font_get(widget, MY_FONT_RESOURCE_ID, &my_font);
/* If status is GX_SUCCESS the font pointer has been retrieved in “my_font”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_color_get
- gx_widget_pixelmap_get

## <a name="gx_widget_free"></a>gx_widget_free
### <a name="release-memory-associated-with-a-widget"></a>Pencere öğesi ile ilişkili yayın belleği

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_free(GX_WIDGETG *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet, bir pencere öğesi denetim bloğu ile ilişkili belleği serbest bırakır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi denetim bloğu işaretçisi
- **resource_id** Yazı tipinin kaynak KIMLIĞI
- **return_font** Yazı tipi işaretçisi için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarıyla serbest bırakıldı pencere öğesi
- **GX_SYSTEM_MEMPRY_ERROR** (0x30) bellek boş işlevi tanımlı değil
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_WIDGET widget;
UINT status;

status = gx_widget_allocate(&widget, sizeof(GX_WIDGET))

/* Free a runtime allocated widget. */
if (status == GX_SUCCESS)
{
      status = gx_widget_free(widget);
}

/* If status is GX_SUCCESS the memory that allocated to the widget has been released. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_front_move"></a>gx_widget_front_move
### <a name="move-widget-to-front"></a>Pencere öğesini öne taşı

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_front_move(
    GX_WIDGET *widget, 
    GX_BOOL *return_moved);
```

### <a name="description"></a>Açıklama

Bu hizmet, alt pencere öğelerinin üst Z sırası listesindeki pencere öğesini öne hareket ettirir.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Taşınacak pencere öğesi işaretçisi
- **return_moved** Gösterge pencere öğesi için hedef işaretçisi taşındı

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi öne taşı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_NO_CHANGE** (0x08) zaten ön pencere öğesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_BOOL widget_moved;

/* Move widget “my_widget” to the front. */
status = gx_widget_front_move(&my_widget, &widget_moved);

/* If status is GX_SUCCESS and “widget_moved” is GX_TRUE, the
widget “my_widget” was moved to the front . */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_height_get"></a>gx_widget_height_get
### <a name="get-widget-height"></a>Pencere öğesi yüksekliğini al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_height_get(
    GX_WIDGET *widget,
    UINT *return_height);
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesi yüksekliğini alır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **return_height** Pencere öğesi yüksekliği için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi yüksekliği al
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_VALUE widget_height;

/* Get height for widget “my_widget”. */
status = gx_widget_height_get(&my_widget, &widget_height);

/* If status is GX_SUCCESS the height of the widget is contained in
“widget_height” . */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_hide"></a>gx_widget_hide
### <a name="hide-widget"></a>Pencere öğesini gizle

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_hide(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesini gizler. Bu pencere öğesi hala üst öğeye eklenmiş, ancak tuval üzerinde çizim yapılmasına izin verilmiyor.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi gizle
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```c
/* Hide widget “my_widget”. */
status = gx_widget_hide(&my_widget);

/* If status is GX_SUCCESS the widget “my_widget” is hidden. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_style_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_last_child_get"></a>gx_widget_last_child_get
### <a name="return-pointer-to-last-child-widget"></a>Son alt pencere öğesine İşaretçiyi döndür

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_last_child_get(
    GX_WIDGET *parent,
    GX_WIDGET **widget_return);
```
### <a name="description"></a>Açıklama

GUX, üst ve alt pencere öğelerinin yapılandırılmış bir listesini tutar. Bu hizmet, üst öğenin son alt pencere öğesine bir işaretçi döndürür.

### <a name="parameters"></a>Parametreler

- **üst öğe** Üst pencere öğesi işaretçisi
- **widget_return** Pencere öğesi işaretçisi döndürme işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) işaretçisi döndü
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Retrieve child widget pointer. */

GX_WIDGET *get_last_child_widget(GX_WIDGET *parent)
{

      GX_WIDGET *child;
      UINT status;

      status = gx_widget_last_child_get(parent, &child);
      if (status == GX_SUCCESS)
      {
              return child;
      }
      return GX_NULL;
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_first_child_get
- gx_widget_next_sibling_get
- gx_widget_parent_get
- gx_widget_previous_sibling_get
- gx_widget_top_visible_child_find

## <a name="gx_widget_next_sibling_get"></a>gx_widget_next_sibling_get
### <a name="return-pointer-to-next-sibling-of-current-widget"></a>Geçerli pencere öğesinin sonraki eşdüzey işaretçisine dön

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_next_sibling_get(
    GX_WIDGET *current,
    GX_WIDGET **widget_return);
```
### <a name="description"></a>Açıklama

GUX, üst ve alt pencere öğelerinin yapılandırılmış bir listesini tutar. Bu hizmet, geçerli pencere öğesinin bir sonraki eşdüzey öğesine bir işaretçi döndürür.

### <a name="parameters"></a>Parametreler

- **geçerli** Geçerli pencere öğesi işaretçisi
- **widget_return** Pencere öğesi işaretçisi döndürme işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) işaretçisi döndü
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Retrieve next sibling widget pointer. */

GX_WIDGET *get_next(GX_WIDGET *current)
{
      GX_WIDGET *sibling;
      UINT status;

      status = gx_widget_next_sibling_get(current, &sibling);
      if (status == GX_SUCCESS)
      {
            return sibling;
      }
      return GX_NULL;
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_first_child_get
- gx_widget_last_child_get
- gx_widget_parent_get
- gx_widget_previous_sibling_get
- gx_widget_top_visible_child_find

## <a name="gx_widget_parent_get"></a>gx_widget_parent_get
### <a name="return-pointer-to-parent-of-current-widget"></a>Geçerli pencere öğesinin üst öğesine İşaretçiyi döndür

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_parent_get(
    GX_WIDGET *current,
    GX_WIDGET **widget_return);
```
### <a name="description"></a>Açıklama

GUX, üst ve alt pencere öğelerinin yapılandırılmış bir listesini tutar. Bu hizmet, geçerli pencere öğesinin üst öğesine bir işaretçi döndürür.

### <a name="parameters"></a>Parametreler

- **geçerli** Geçerli pencere öğesi işaretçisi
- **widget_return** Pencere öğesi işaretçisi döndürme işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) işaretçisi döndü
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Retrieve parent widget */

GX_WIDGET *get_parent(GX_WIDGET *current)
{
      GX_WIDGET *parent;
      UINT status;

      status = gx_widget_parent_get(current, &parent);
      if (status == GX_SUCCESS)
      {
            return parent;
      }
      return GX_NULL;
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_first_child_get
- gx_widget_last_child_get
- gx_widget_next_sibling_get
- gx_widget_previous_sibling_get
- gx_widget_top_visible_child_find

## <a name="gx_widget_pixelmap_get"></a>gx_widget_pixelmap_get
### <a name="get-pixelmap"></a>Pixelmap al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_pixelmap_get(
    GX_WIDGET *widget,
    GX_RESOURCE_ID resource_id,
    GX_PIXELMAP **return_pixelmap);
```

### <a name="description"></a>Açıklama

Bu hizmet, sağlanan kaynak KIMLIĞIYLE ilişkili pixelmap 'i alır. Bu hizmet yalnızca görünür pencere öğeleri için çağrılmalıdır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi denetim bloğu işaretçisi
- **pixelmap_id** Pixelmap kaynak KIMLIĞI
- **return_pixelmap** Pixelmap hedef işaretçisine yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pixelmap al
- **GX_INVALID_RESOURCE_ID** (0x33) GEÇERSIZ kaynak kimliği
- **GX_INVALID_CANVAS** (0x20) pencere öğesi tuvali geçerli değil veya pencere öğesi görünmez
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```c
GX_PIXELMAP *my_pixelmap;

/* Get the pixelmap associated with MY_PIXELMAP_ID. */
status = gx_widget_pixelmap_get(widget, MY_PIXELMAP_RESOURCE_ID,
                                &my_pixelmap);

/* If status is GX_SUCCESS, “my_pixelmap” contains the pixemap pointer. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_color_get
- gx_widget_font_get

## <a name="gx_widget_previous_sibling_get"></a>gx_widget_previous_sibling_get
### <a name="return-pointer-to-previous-sibling-of-the-current-widget"></a>Geçerli pencere öğesinin önceki eşdüzey işaretçisine dön

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_previous_sibling_get(
    GX_WIDGET *current,
    GX_WIDGET **widget_return);
```

### <a name="description"></a>Açıklama

GUX, üst ve alt pencere öğelerinin yapılandırılmış bir listesini tutar. Bu hizmet, geçerli pencere öğesinin önceki eşdüzey öğesine bir işaretçi döndürür.

### <a name="parameters"></a>Parametreler

- **geçerli** Geçerli pencere öğesi işaretçisi
- **widget_return** Pencere öğesi işaretçisi döndürme işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) işaretçisi döndü
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Retrieve previous sibling widget */

GX_WIDGET *get_previous(GX_WIDGET *current)
{
      GX_WIDGET *sibling;
      UINT status;

      status = gx_widget_previous_sibling_get(current, &sibling);
      if (status == GX_SUCCESS)
      {
          return sibling;
      }
      return GX_NULL;
}
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_first_child_get
- gx_widget_last_child_get
- gx_widget_next_sibling_get
- gx_widget_parent_get
- gx_widget_top_visible_child_find

## <a name="gx_widget_resize"></a>gx_widget_resize
### <a name="resize-widget"></a>Pencere öğesini yeniden boyutlandır

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_resize(
    GX_WIDGET *widget, 
    GX_RECTANGLE *new_size);
```
### <a name="description"></a>Açıklama

Bu hizmet pencere öğesini yeniden boyutlandırır. Pencere öğesi görünür durumdaysa otomatik olarak geçersiz kılınır ve yeniden çizim için sıraya alınır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **new_size** Yeni pencere öğesi boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi yeniden boyutlandırma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RECTANGLE new_size;

gx_utility_rectangle_define(&new_size, 0, 0, 100, 100);

/* Resize widget “my_widget”. */
status = gx_widget_resize(&my_widget, &new_size);

/* If status is GX_SUCCESS the widget “my_widget” has been resized. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_shift"></a>gx_widget_shift
### <a name="shift-widget"></a>Kaydırma pencere öğesi

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_shift(
    GX_WIDGET *widget, 
    GX_VALUE x_shift,
    GX_VALUE y_shift, 
    GX_BOOL mark_dirty);
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesini kaymalar ve isteğe bağlı olarak onu kirli olarak işaretler.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **x_shift** X ekseninde kaydırma için piksel sayısı
- **y_shift** Y ekseninde kaydırma yapılacak piksel sayısı
- **mark_dirty** Kirli olduğunu göstermek için GX_TRUE, aksi takdirde GX_FALSE

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi kaydırma GX_CALLER_ERROR (0x11) bu işlevin geçersiz çağıranı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Shift widget “my_widget”. */
status = gx_widget_shift(&my_widget, 10, 20, GX_FALSE);

/* If status is GX_SUCCESS the widget “my_widget” has been shifted. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_show"></a>gx_widget_show
### <a name="show-widget"></a>Pencere öğesini göster

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_show(GX_WIDGET *widget);
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesini gösterir. Pencere öğesi yalnızca bir üst öğeye iliştirilmişse görünür hale gelir ve üst pencere öğesi de görünür olur.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi Show
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Show widget “my_widget”. */
status = gx_widget_show(&my_widget);

/* If status is GX_SUCCESS the widget “my_widget” has been shown. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_status_add"></a>gx_widget_status_add
### <a name="add-widget-status"></a>Pencere öğesi durumu Ekle

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_status_add(
    GX_WIDGET *widget, 
    ULONG status)
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencere öğesine durum bayraklarının herhangi bir birleşimini ekler.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **durum** Eklenecek durum

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi durumu ekleme
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Add status to widget “my_widget”. */
status = gx_widget_status_add(&my_widget, status_to_add);

/* If status is GX_SUCCESS the widget “my_widget” status was. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_status_get"></a>gx_widget_status_get
### <a name="get-widget-status"></a>Pencere öğesi durumunu al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_status_get(
    GX_WIDGET *widget,
    ULONG *return_status)
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesinin durum bayraklarını alır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **return_status** Döndürülen durum işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi durumu Al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
ULONT get_status;

/* Retrieve status flag from widget “my_widget”. */ status =
gx_widget_status_get(&my_widget, &get_status);

/* If status is GX_SUCCESS the status from widget “my_widget” is
saved to “get_status”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_status_remove"></a>gx_widget_status_remove
### <a name="remove-widget-status"></a>Pencere öğesi durumunu kaldır

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_status_remove(
    GX_WIDGET *widget, 
    ULONG status)
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğeleri iç durum değişkeninden belirtilen durum bayraklarını kaldırır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **durum** Kaldırılacak durum

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi durumu kaldırma
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Remove status of widget “my_widget”. */
status = gx_widget_status_remove(&my_widget, status_to_remove);

/* If status is GX_SUCCESS, the status flags are removed from the
widget “my_widget”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_status_test"></a>gx_widget_status_test
### <a name="test-widget-status"></a>Test pencere öğesi durumu

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_status_test(
    GX_WIDGET *widget, 
    ULONG status,
    GX_BOOL *return_test);
```
### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencere öğesinin durum bayraklarını sınar ve sonucu "return_test" ile işaret edilen bellekte depolar.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **durum** Sınanacak durum
- **return_status** Testin sonucu için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi durum testi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_BOOL test_result;

/* Test status of widget “my_widget”. */
status = gx_widget_status_test(&my_widget, status_to_test,
                              &test_result);

/* If status is GX_SUCCESS the widget “my_widget” status was tested
and the result in “test_result”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set

## <a name="gx_widget_string_get"></a>gx_widget_string_get
### <a name="retrieve-string-associated-with-a-visible-widget-and-string-id-deprecated"></a>Görünür bir pencere öğesi ve dize KIMLIĞIYLE ilişkili dizeyi al (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_string_get(
    GX_WIDGET *widget,
    GX_RESOURCE_ID string_id,
    GX_CONST GX_CHAR **string);
```

### <a name="description"></a>Açıklama

Bu hizmet gx_widget_string_get_ext () kullanımı için kullanım dışıdır.

Bu hizmet, belirtilen dize KIMLIĞI değeri için dize tablosu girişini döndürür. Bu hizmet gx_display_string_get benzerdir, çünkü etkin ekran, arayan tarafından geçirilmesi yerine otomatik olarak belirlenir. Bu hizmet yalnızca görünen pencere öğeleri için kullanılabilir, yani bu pencere öğesiyle ilişkili görüntüleme bilinmektedir.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **string_id** Kaynak üstbilgisinden dize KIMLIĞI değeri
- **dize** Dizeyi döndüren değişkenin adresi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi durum testi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_CONST GX_CHAR *string;

/* Test status of widget “my_widget”. */
status = gx_widget_string_get(&my_widget, GX_STRING_ID_SHUTDOWN,
      &string);

/* If status is GX_SUCCESS the string has been retrieved */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_string_get
- gx_display_active_langauge_set

## <a name="gx_widget_string_get_ext"></a>gx_widget_string_get_ext
### <a name="retrieve-string-associated-with-a-visible-widget-and-string-id"></a>Görünür bir pencere öğesi ve dize KIMLIĞIYLE ilişkili dizeyi al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_string_get(
    GX_WIDGET *widget,
    GX_RESOURCE_ID string_id,
    GX_CONST GX_STRING *string);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen dize KIMLIĞI değeri için dize tablosu girişini döndürür. Bu hizmet gx_display_string_get benzerdir, çünkü etkin ekran, arayan tarafından geçirilmesi yerine otomatik olarak belirlenir. Bu hizmet yalnızca görünen pencere öğeleri için kullanılabilir, yani bu pencere öğesiyle ilişkili görüntüleme bilinmektedir.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **string_id** Kaynak üstbilgisinden dize KIMLIĞI değeri
- **dize** Dizeyi döndüren değişkenin adresi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi durum testi
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_STRING string;

/* Test status of widget “my_widget”. */

status = gx_widget_string_get_ext(&my_widget,
                          GX_STRING_ID_SHUTDOWN, &string);

/* If status is GX_SUCCESS the string has been retrieved */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_display_string_get
- gx_display_active_langauge_set

## <a name="gx_widget_style_add"></a>gx_widget_style_add
### <a name="add-widget-style"></a>Pencere öğesi stili Ekle

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_style_add(
    GX_WIDGET *widget, 
    ULONG style)
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesine bir stil ekler. Ayrıca, aşağıdaki eylemler alınır.

Eklenen stil GX_STYLE_TRANSPARENT, durum GX_STATUS_TRANSPARENT eklenir.

Eklenen stil GX_STYLE_ENABLED, durum GX_STATUS_SELECTABLE eklenir.

Pencere öğesi görünür durumdaysa otomatik olarak geçersiz kılınır ve yeniden çizim için sıraya alınır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **Stil** Eklenecek yeni stil. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi stili ekleme
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Add style to widget “my_widget”. */
status = gx_widget_style_add(&my_widget, GX_STYLE_BORDER_RAISED);

/* If status is GX_SUCCESS, the style was successfully applied to the widget “my_widget”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_style_get"></a>gx_widget_style_get
### <a name="get-widget-style"></a>Pencere öğesi stili al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_style_get(
    GX_WIDGET *widget, 
    ULONG *return_style)
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesinden stil bayrağını alır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **return_style** Döndürülmekte olan stilin işaretçisi.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarıyla pencere öğesi stili alındı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları


### <a name="example"></a>Örnek

```C
/* Retrieve style from widget into “style”. */
status = gx_widget_style_get(&my_widget, &style);

/* If status is GX_SUCCESS the style flag from widget is saved in “style”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_remove
- gx_widget_style_add
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_style_remove"></a>gx_widget_style_remove
### <a name="remove-widget-style"></a>Pencere öğesi stilini kaldır

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_style_remove(
    GX_WIDGET *widget, 
    ULONG style)
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesinin bir stilini kaldırır. Ayrıca, aşağıdaki eylemler alınır.

Kaldırılan stil GX_STYLE_TRANSPARENT, durum GX_STATUS_TRANSPARENT kaldırılır.

Kaldırılan stil GX_STYLE_ENABLED, durum GX_STATUS_SELECTABLE kaldırılır.

Pencere öğesi görünür durumdaysa otomatik olarak geçersiz kılınır ve yeniden çizim için sıraya alınır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **Stil** Kaldırılacak stil. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi stili kaldır
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Remove style from widget “my_widget”. */
status = gx_widget_style_remove(&my_widget,
                                GX_STYLE_BORDER_RAISED);

/* If status is GX_SUCCESS the GX_STYLE_BORDER_RAISED style was removed from the widget “my_widget”.*/
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_style_set"></a>gx_widget_style_set
### <a name="set-widget-style"></a>Pencere öğesi stilini ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_style_set(
    GX_WIDGET *widget, 
    ULONG style)
```

### <a name="description"></a>Açıklama

Bu hizmet pencere öğesine bir stil ayarlar.

Küme stili GX_STYLE_TRANSPARENT içeriyorsa, durum GX_STATUS_TRANSPARENT eklenir, aksi takdirde durum kaldırılır.

Küme stili GX_STYLE_ENABLED içeriyorsa, durum GX_STATUS_SELECTABLE eklenir, aksi takdirde durum kaldırılır.

Pencere öğesi görünür durumdaysa otomatik olarak geçersiz kılınır ve yeniden çizim için sıraya alınır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **Stil** Ayarlanacak stil. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi stil kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set style GX_STYLE_TRANSPARENT to the widget “my_widget”. */
status = gx_widget_style_set(&my_widget, GX_STYLE_TRANSPARENT);

/* If status is GX_SUCCESS the widget “my_widget” style is set to GX_STYLE_TRANSPARENT. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_set
- gx_widget_width_get

## <a name="gx_widget_text_blend"></a>gx_widget_text_blend
### <a name="blend-text-assigned-to-widget-deprecated"></a>Pencere öğesine atanan metin Blend (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_text_blend(
    GX_WIDGET *widget, 
    UINT *tColor,
    UINT font_id, 
    GX_CHAR *string,
    INT x_offset, 
    INT y_offset, 
    UCHAR alpha)
```

### <a name="description"></a>Açıklama

Bu hizmet gx_widget_text_blend_ext () kullanımı için kullanım dışıdır.

Bu hizmet, geçerli fırça ve metin hizalamasını kullanarak belirtilen metni bir pencere öğesi üzerinde karıştırır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **TColor** Metin rengi
- **font_id** Yazı tipi kimliği
- **dize** Çizim dizesi
- **x_offset** Çizim konumu ayarlama
- **y_offset** Çizim konumu ayarlama
- **Alfa** Değer karıştırma 0-255

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi genişliği al
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Blend “my_string” over “my_widget” given alpha value 120. */
status = gx_widget_text_blend(&my_widget, my_text_color, my_font_id,
                              &my_string, xoffset, yoffset, 120);

/* If status is GX_SUCCESS “my_string” has been blend to “my_widget”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_text_blend_ext

## <a name="gx_widget_text_blend_ext"></a>gx_widget_text_blend_ext
### <a name="blend-text-assigned-to-widget"></a>Pencere öğesine atanan metni karıştır

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_text_blend(
    GX_WIDGET *widget, 
    UINT *tColor,
    UINT font_id, 
    GX_CONST GX_STRING *string,
    INT x_offset, 
    INT y_offset, 
    UCHAR alpha)
```

### <a name="description"></a>Açıklama

Bu hizmet gx_widget_text_blend_ext () kullanımı için kullanım dışıdır.

Bu hizmet, geçerli fırça ve metin hizalamasını ve belirtilen renk, yazı tipi ve x, y sapmasını kullanarak belirtilen pencere öğesi üzerinde bir dize oluşturur.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **TColor** Metin rengi
- **font_id** Yazı tipi kimliği
- **dize** Çizim dizesi
- **x_offset** Çizim konumu ayarlama
- **y_offset** Çizim konumu ayarlama
- **Alfa** Değer karıştırma 0-255

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi genişliği al
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_STRING_LENGTH** (0x34) geçersiz dize uzunluğu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
gx_string render_string;
render_string.gx_string_ptr = “Hello”;
render_string.gx_string_length =
    strlen(render_string.gx_string_ptr);

/* Blend “my_string” over “my_widget” given alpha value 120. */
status = gx_widget_text_blend_ext(&my_widget,
        my_text_color,
        my_font_id,
        &render_string, xoffset, yoffset, 120);

/* If status is GX_SUCCESS “my_string” has been blend to “my_widget”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_text_draw_ext

## <a name="gx_widget_text_draw"></a>gx_widget_text_draw
### <a name="draw-text-assigned-to-widget-deprecated"></a>Pencere öğesine atanan metin çiz (kullanım dışı)

### <a name="prototype"></a>Prototype

```C
VOID gx_widget_text_draw(
    GX_WIDGET *widget, 
    UINT *tColor,
    UINT font_id, 
    GX_CHAR *string,
    INT x_offset, 
    INT y_offset)
```

### <a name="description"></a>Açıklama

Bu hizmet gx_widget_text_draw_ext () kullanımı için kullanım dışıdır.

Bu hizmet, geçerli fırça ve metin hizalamasını kullanarak belirtilen metni bir pencere öğesi üzerine çizer.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **TColor** Metin rengi
- **font_id** Yazı tipi kimliği
- **dize** Çizim dizesi
- **x_offset** Çizim konumu ayarlama
- **y_offset** Çizim konumu ayarlama

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom widget draw function. */

VOID my_custom_widget_draw(GX_WIDGET *widget)
{
    /* Add your own background raw here. */

    /* Call widget text draw. */
    gx_widget_text_draw(widget, my_text_color, my_font_id
                        &my_string, xoffset, yoffset);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_text_blend
- gx_widget_text_id_draw

## <a name="gx_widget_text_draw_ext"></a>gx_widget_text_draw_ext
### <a name="draw-text-assigned-to-widget"></a>Pencere öğesine atanan metin çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_widget_text_draw(
    GX_WIDGET *widget,
    UINT *tColor,
    UINT font_id, 
    GX_CONST GX_STRING *string,
    INT x_offset,
    INT y_offset)
```

### <a name="description"></a>Açıklama

Bu hizmet, geçerli fırça ve metin hizalamasını kullanarak belirtilen metni bir pencere öğesi üzerine çizer.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **TColor** Metin rengi
- **font_id** Yazı tipi kimliği
- **text_id** Metin kimliği
- **x_offset** Çizim konumu ayarlama
- **y_offset** Çizim konumu ayarlama

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
gx_string render_string;
render_string.gx_string_ptr = “Hello”;
render_string.gx_string_length =
    strlen(render_string.gx_string_ptr);

/* Write a custom widget draw function. */
VOID my_custom_widget_draw(GX_WIDGET *widget)
{
    /* Add your own background draw here. */

    /* Call widget text draw. */
    gx_widget_text_draw_ext(widget, my_text_color, my_font_id
                        &render_string, xoffset, yoffset);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_text_blend
- gx_widget_text_id_draw

## <a name="gx_widget_text_id_draw"></a>gx_widget_text_id_draw
### <a name="draw-text-assigned-to-widget"></a>Pencere öğesine atanan metin çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_widget_text_id_draw(
    GX_WIDGET *widget, 
    UINT *tColor,
    UINT font_id, 
    UINT text_id,
    INT x_offset, 
    INT y_offse)
```

### <a name="description"></a>Açıklama

Bu hizmet, metin kimliği verilen bir pencere öğesinin üzerine metin çizer.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **TColor** Metin rengi
- **font_id** Yazı tipi kimliği
- **text_id** Metin kimliği
- **x_offset** Çizim konumu ayarlama
- **y_offset** Çizim konumu ayarlama

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom widget draw function. */

VOID my_custom_widget_draw(GX_WIDGET *widget)
{
    /* Add your own background raw here. */

    /* Call widget text id draw. */
    gx_widget_text_id_draw(widget, my_text_color, my_font_id
                            &my_string_id, xoffset, yoffset);
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_text_blend
- gx_widget_text_draw

## <a name="gx_widget_top_visible_child_find"></a>gx_widget_top_visible_child_find
### <a name="return-pointer-to-visible-child-that-is-top-of-z-order"></a>İşaretçiyi Z düzeninin en üstünde bulunan, görünür alt öğeye döndür

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_top_visible_child_find(
    GX_WIDGET *current,
    GX_WIDGET **widget_return);
```

### <a name="description"></a>Açıklama

GUX, üst ve alt pencere öğelerinin yapılandırılmış bir listesini tutar.
Bu hizmet, geçerli pencere öğesinin en üstteki görünür alt öğesine bir işaretçi döndürür.

### <a name="parameters"></a>Parametreler

- **geçerli** Geçerli pencere öğesi işaretçisi
- **widget_return** Pencere öğesi işaretçisi döndürme işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) işaretçisi döndü
- **GX_PTR_ERROR** (0x07) geçersiz pencere öğesi işaretçisi
- **GX_INVALID_WIDGET** (0x12) geçersiz pencere öğesi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Retrieve topmost visible widget on the display */

GX_WIDGET *get_top_window(GX_WINDOW_ROOT *root)
{
    GX_WIDGET *top_window;
    UINT status;

    status = gx_widget_top_visible_child_find(root, &top_window);
    if (status == GX_SUCCESS)
    {
        return top_window;
    }
    return GX_NULL;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_first_child_get,
- gx_widget_last_child_get,
- gx_widget_next_sibling_get,
- gx_widget_parent_get,
- gx_widget_previous_sibling_get

## <a name="gx_widget_type_find"></a>gx_widget_type_find
### <a name="search-for-a-widget-of-the-requested-type"></a>İstenen türde pencere öğesi ara

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_type_find(
    GX_WIDGET *parent, 
    USHORT widget_id,
    GX_WIDGET **return_widget)
```

### <a name="description"></a>Açıklama

Bu hizmet, istenen türdeki bir pencere öğesini arar.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **return_width** Pencere öğesi genişliği için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi genişliği al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_WIDGET *retrieved_widget;

/* Find horizontal scrollbar under “parent_widget”. */
status = gx_widget_type_find(&parent_widget,
                GX_TYPE_HORIZONTAL_SCROLL_BAR, &retrieved_widget);

/* If status is GX_SUCCESS, the horizontal scrollbar widget is retrieved. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set

## <a name="gx_widget_width_get"></a>gx_widget_width_get
### <a name="get-widget-width"></a>Pencere öğesi genişliğini al

### <a name="prototype"></a>Prototype

```C
UINT gx_widget_width_get(
    GX_WIDGET *widget,
    GX_VALUE *return_width)
```

### <a name="description"></a>Açıklama

Bu hizmet, pencere öğesinin genişliğini alır.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi işaretçisi
- **return_width** Pencere öğesi genişliği için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere öğesi genişliği al
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_VALUE my_widget_width;

/* Get width of widget “my_widget”. */
status = gx_widget_width_get(&my_widget, &my_widget_width);

/* If status is GX_SUCCESS the width of widget “my_widget” is in “my_widget_width”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_widget_attach
- gx_widget_back_move
- gx_widget_background_set
- gx_widget_border_draw
- gx_widget_border_style_set
- gx_widget_border_width_get
- gx_widget_canvas_get
- gx_widget_child_detect
- gx_widget_children_draw
- gx_widget_client_get
- gx_widget_created
- gx_widget_created_test
- gx_widget_delete
- gx_widget_detach
- gx_widget_draw
- gx_widget_draw_set
- gx_widget_event_generate
- gx_widget_event_process
- gx_widget_event_process_set
- gx_widget_event_to_parent
- gx_widget_find
- gx_widget_front_move
- gx_widget_height_get
- gx_widget_hide
- gx_widget_resize
- gx_widget_shift
- gx_widget_show
- gx_widget_status_add
- gx_widget_status_get
- gx_widget_status_remove
- gx_widget_status_test
- gx_widget_style_add
- gx_widget_style_get
- gx_widget_style_remove
- gx_widget_style_set

## <a name="gx_window_client_height_get"></a>gx_window_client_height_get
### <a name="get-window-client-height"></a>Pencere istemci yüksekliğini al

### <a name="prototype"></a>Prototype

```C
UINT gx_window_client_height_get(
    GX_WINDOW *window,
    GX_VALUE *return_height);
```

### <a name="description"></a>Açıklama

Bu hizmet, pencerenin istemci yüksekliğini alır.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere işaretçisi
- **return_height** İstemci yüksekliğinin hedefi işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere istemci yüksekliği al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RECTANGLE my_client_height;

/* Get client height of “my_window”. */
status = gx_window_client_height_get(&my_window,
                                     &my_client_height);

/* If status is GX_SUCCESS the window “my_window” client height is contained in “my_client_height”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- x_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_client_scroll"></a>gx_window_client_scroll
### <a name="scroll-window-clients"></a>Pencere istemcilerini kaydır

### <a name="prototype"></a>Prototype

```C
UINT gx_window_client_scroll(
    GX_WINDOW *window, 
    GX_VALUE x_scroll,
    GX_VALUE y_scroll);
```

### <a name="description"></a>Açıklama

Bu hizmet, Windows istemcilerini belirtilen tutara göre kaydırır.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere işaretçisi
- **x_scroll** X ekseninde kaydırılan miktar
- **y_scroll** Y ekseninde kaydırılan miktar

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere istemcisi kaydırma
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_VALUE** (0X22) kaydırma değerleri geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Scroll clients of “my_window”. */
status = gx_window_client_scroll(&my_window, 10, 0);

/* If status is GX_SUCCESS the clients of window “my_window” have been scrolled. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_client_width_get"></a>gx_window_client_width_get
### <a name="get-window-client-width"></a>Pencere istemci genişliğini al

### <a name="prototype"></a>Prototype

```C
UINT gx_window_client_width_get(
    GX_WINDOW *window,
    GX_VALUE *return_width);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencerenin istemci genişliğini alır.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere işaretçisi
- **return_height** İstemci genişliği için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere istemci genişliği al
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_VALUE my_client_widthl

/* Get client width of “my_window”. */
status = gx_window_client_width_get(&my_window, &my_client_width);

/* If status is GX_SUCCESS “my_client_width” contains the client width of window “my_window”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_close"></a>gx_window_close
### <a name="close-modal-window"></a>Kalıcı pencereyi kapat

### <a name="prototype"></a>Prototype

```C
UINT gx_window_close(GX_WINDOW *window);
```

### <a name="description"></a>Açıklama

Bu hizmet, kalıcı bir pencerenin üst öğesinden ayrılmaya ve kalıcı yürütme döngüsünden geri dönmesini zorlar.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) pencereyi başarıyla kapattı
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Close window “my_window”. */
status = gx_window_close(&my_window);

/* If status is GX_SUCCESS window “my_window” has been closed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_create"></a>gx_window_create
### <a name="create-window"></a>Pencere oluştur

### <a name="prototype"></a>Prototype

```C
UINT gx_window_create(
    GX_WINDOW *window, 
    GX_CONST GX_CHAR *name,
    GX_WIDGET *parent, 
    ULONG style,
    USHORT window_id, 
    GX_CONST GX_RECTANGLE *size);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pencere oluşturur.

GX_WINDOW GX_WIDGET türetilir ve tüm gx_widget API hizmetlerini destekler.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere denetim bloğu işaretçisi
- **ad** Pencerenin mantıksal adı
- **üst öğe** Üst pencere öğesi işaretçisi
- **Stil** Pencere stili. **Ek D** , tüm pencere öğelerinin yanı sıra pencere öğesine özgü stillerin önceden tanımlanmış genel stillerini içerir.
- **window_id** Pencerenin uygulama tanımlı KIMLIĞI
- **Boyut** Pencerenin boyutu

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere oluştur
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_WINDOW my_window;

/* Create window “my_window”. */
status = gx_window_create(&my_window, "my window",
                          &my_parent_window, GX_STYLE_BORDER_RAISED,
                          MY_WINDOW_ID, &size);

/* If status is GX_SUCCESS window “my_window” has been created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_draw"></a>gx_window_draw
### <a name="draw-window"></a>Pencereyi çiz

### <a name="prototype"></a>Prototype

```C
VOID gx_window_draw(GX_WINDOW *window);
```

### <a name="description"></a>Açıklama

Bu hizmet bir pencere çizer. Bu hizmet, genellikle tuval yenilemesi sırasında dahili olarak çağrılır, ancak özel pencere çizim işlevlerinden de çağrılabilir.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **Hiçbiri**

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Write a custom window draw function. */

VOID my_custom_window_draw(GX_WINDOW *window)
{
    /* Call default window draw. */
    gx_window_draw(window);

    /* Add your own drawing here. */
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_event_process"></a>gx_window_event_process
### <a name="process-window-event"></a>İşlem penceresi olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_window_event_process(
    GX_WINDOW *window, 
    GX_EVENT *event);
```

### <a name="description"></a>Açıklama

Bu hizmet bu pencere için bir olay işler.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere denetim bloğu işaretçisi
- **olay** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere olay işleme
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic window event processing as part of custom event processing function. */

UINT custom_window_event_process(GX_WINDOW *window,
                                 GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
        case xyz:
            /* Insert custom event handling here */
            break;
        default:
            /* Pass all other events to the default window
            event processing */
            status = gx_window_event_process(window, event);
            break;
        }
        return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_execute"></a>gx_window_execute
### <a name="modally-execute-a-window"></a>Bir pencereyi önemli bir şekilde yürütür

### <a name="prototype"></a>Prototype

```C
UINT gx_window_execute(
    GX_WINDOW *window,
    ULONG *return_ptr)
```

### <a name="description"></a>Açıklama

Bu hizmet, bir pencereyi önemli ölçüde yürütür. Pencere istemci alanının dışında herhangi bir kullanıcı girişi (Pen olayları, vb.) yok sayılır. Bu işlevin sürekli engelleyici bir yürütme döngüsü girdiğini ve model yürütme sonlanana kadar çağırana dönmediğini unutmayın.

Alınan herhangi bir olay için olay işleme sıfır olmayan bir durum değeri döndürdüğünde veya gx_window_close API işlevi çağrıldığında kalıcı yürütme sonlandırılır. Sıfır olmayan olay işleme dönüş kodu, bu API 'ye geçirilen return_ptr aracılığıyla çağırana döndürülür

### <a name="parameters"></a>Parametreler

- **pencere** Pencere denetim bloğu işaretçisi
- **return_ptr** Kalıcı yürütme çıkış durumunun kaydedileceği konum. GX_NULL olabilir.

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı yürütme
- **GX_SYSTEM_EVENT_RECEIVE_ERROR (0x05)** Olay kuyruğundan alma olayı başarısız oldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Execute a modal window. */
status = gx_window_execute(&my_window, &return_code);

/* If status is GX_SUCCESS the window was executed, and return_code holds the execution return code. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_root_create"></a>gx_window_root_create
### <a name="create-a-root-window"></a>Kök penceresi oluşturma

### <a name="prototype"></a>Prototype

```C
UINT gx_window_root_create(
    GX_WINDOW_ROOT *root_window,
    GX_CONST GX_CHAR *name,
    GX_CANVAS *canvas, 
    ULONG style,
    USHORT id,
    GX_CONST GX_RECTANGLE *size)
```

### <a name="description"></a>Açıklama

Bu hizmet bir kök penceresi oluşturur.

### <a name="parameters"></a>Parametreler

- **root_window** Kök pencere denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) kök pencere başarıyla oluşturuldu
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_SIZE** (0x19) geçersiz pencere öğesi denetimi blok boyutu
- **GX_ALREADY_CREATED** (0x13) pencere öğesi zaten oluşturuldu

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_ROOT_WINDOW root_window;
GX_CANVAS canvas;

/* Create canvas here. */

/* Create a root window */
status = gx_window_root_create(&root_window, “root”, &canvas,
GX_STYLE_BORDER_NONE, GX_NULL, &size);

/* If status is GX_SUCCESS, the “root_window” is successfully created. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find

## <a name="gx_window_root_delete"></a>gx_window_root_delete
### <a name="destroy-a-root-window"></a>Kök pencereyi yok etme

### <a name="prototype"></a>Prototype

```C
UINT gx_window_root_delete(GX_WINDOW_ROOT *root_window)
```

### <a name="description"></a>Açıklama

Bu hizmet bir kök pencereyi siler.

### <a name="parameters"></a>Parametreler

- **root_window** Kök pencere denetim bloğu işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) kök pencere başarıyla silindi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_SYSTEM_MEMORY_ERROR** (0x30) bellek boş işlevi tanımlı değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Delete a root window */
status = gx_window_root_delete(&root_window);

/* If status is GX_SUCCESS the “root_window” is destroyed. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_root_event_process"></a>gx_window_root_event_process
### <a name="process-event-for-the-root-window"></a>Kök pencere için işlem olayı

### <a name="prototype"></a>Prototype

```C
UINT gx_window_root_create(
    GX_WINDOW_ROOT *root_window,
    GX_EVENT *event)
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen kök pencereyle ilgili olayları işler.

### <a name="parameters"></a>Parametreler

- **root_window** Kök pencere denetim bloğu işaretçisi
- **olay** İşlenecek olaya yönelik işaretçi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) kök pencere olayı başarıyla işlendi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi

### <a name="allowed-from"></a>İzin verilen

İş Parçacıkları

### <a name="example"></a>Örnek

```C
/* Call generic root window event processing as part of custom event processing function. */

UINT custom_root_window_event_process(GX_ROOT_WINDOW *root,
                                      GX_EVENT *event)
{
    UINT status = GX_SUCCESS;

    switch(event->gx_event_type)
    {
    case xyz:
        /* Insert custom event handling here */
        break;
    default:
        /* Pass all other events to the default root window
            event processing */
        status = gx_window_root_event_process(root, event);
        break;
    }
    return status;
}
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_root_find"></a>gx_window_root_find
### <a name="find-root-window"></a>Kök penceresini bul

### <a name="prototype"></a>Prototype

```C
UINT gx_window_root_find(
    GX_WIDGET *widget,
    GX_WINDOW_ROOT **return_root_window);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencere öğesi için kök pencereyi bulur.

### <a name="parameters"></a>Parametreler

- **pencere öğesi** Pencere öğesi denetim bloğu işaretçisi
- **return_root_window** Bulunan kök penceresi için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı kök pencere bulma
- **GX_FAILURE** (0x00) kök penceresi yok
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Find root window associated with window “my_window”. */
status = gx_window_root_find(&my_window, &root_window);

/* If status is GX_SUCCESS the “root_window” contains the root window for window “my_window”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_scroll_info_get"></a>gx_window_scroll_info_get
### <a name="get-window-scroll-info"></a>Pencere kaydırma bilgisini al

### <a name="prototype"></a>Prototype

```C
UINT gx_window_scroll_info_get(
    GX_WINDOW *window, 
    ULONG style,
    GX_SCROLL_INFO *return_scroll_info);
```

### <a name="description"></a>Açıklama

Bu hizmet pencere kaydırma bilgilerini alır.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere işaretçisi
- **Stil** GX_SCROLLBAR_HORIZONTAL veya GX_SCROLLBAR_VERTICAL
- **return_scroll_info** Kaydırma bilgisi için hedef işaretçisi. Ana pencere, üst pencere kaydırma çubuğunu, görüntülenebilir alanı ve kaydırma artışını ve sınırlarını bilgilendirmek için bu yapıyı başlatır. Varsayılan uygulama, Windows istemci alanını görüntülenebilir alan olarak kullanır ve piksellere göre kayar, ancak özelleştirilmiş pencere uygulama, kaydırma parametrelerini kullanabilir. **Ek ı** GX_SCROLL_INFO yapısının tanımını içerir

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere kaydır bilgi al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_TYPE** (0x1B) geçersiz tür

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_SCROLL_INFO scroll_info;

/* Get scroll information for window “my_window”. */
status = gx_window_scroll_info_get(&my_window,
                    GX_SCROLLBAR_HORIZONTAL, &scroll_info);

/* If status is GX_SUCCESS the “scroll_info” contains the scroll information for window “my_window”. */
```
### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scrollbar_find
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_scrollbar_find"></a>gx_window_scrollbar_find
### <a name="find-window-scrollbar"></a>Pencere kaydırma çubuğunu bul

### <a name="prototype"></a>Prototype

```C
UINT gx_window_scrollbar_find(
    GX_WINDOW *window, 
    USHORT type,
    GX_SCROLLBAR **return_scrollbar);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencere için kaydırma çubuğunu bulur.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere işaretçisi
- **tür** GX_TYPE_VERTICAL_SCROLL veya GX_TYPE_HORIZONTAL_SCROLL
- **return_scrollbar** Kaydırma çubuğu için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere kaydırma çubuğu bul
- **GX_NOT_FOUND** (0x09) kaydırma çubuğu bulunamadı
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil
- **GX_INVALID_TYPE** (0x1B) geçersiz tür

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Find horizontal scrollbar for window “my_window”. */
status = gx_window_scrollbar_find(&my_window,
                 GX_SCROLLBAR_HORIZONTAL, &my_scrollbar);

/* If status is GX_SUCCESS the “my_scrollbar” contains the horizontal scrollbar for window “my_window”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_wallpaper_get
- gx_window_wallpaper_set

## <a name="gx_window_wallpaper_get"></a>gx_window_wallpaper_get
### <a name="get-window-wallpaper"></a>Pencere duvar kağıdını al

### <a name="prototype"></a>Prototype

```C
UINT gx_window_wallpaper_get(
    GX_WINDOW *window,
    GX_RESOURCE_ID *return_wallpaper_id);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencere için duvar kağıdını alır.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere işaretçisi
- **return_wallpaper_id** Duvar kağıdının kaynak KIMLIĞI için hedef işaretçisi

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere duvar kağıdı al
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
GX_RESOURCE_ID my_window_wallpaper;

/* Get wallpaper for window “my_window”. */
status = gx_window_wallpaper_get(&my_window, &my_window_wallpaper);

/* If status is GX_SUCCESS the “my_window_wallpaper” contains the wallpaper resource ID for window “my_window”. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
- gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_set

## <a name="gx_window_wallpaper_set"></a>gx_window_wallpaper_set
### <a name="set-window-wallpaper"></a>Pencere duvar kağıdını ayarla

### <a name="prototype"></a>Prototype

```C
UINT gx_window_wallpaper_set(
    GX_WINDOW *window,
    GX_RESOURCE_ID wallpaper_id,
    GX_BOOL tile);
```

### <a name="description"></a>Açıklama

Bu hizmet, belirtilen pencere için duvar kağıdını ayarlar.

### <a name="parameters"></a>Parametreler

- **pencere** Pencere işaretçisi
- **wallpaper_id** Kullanılacak duvar kağıdının kaynak KIMLIĞI
- **kutucuk** Duvar kağıdı GX_TRUE ise döşeli, aksi halde duvar kağıdı döşeli değildir

### <a name="return-values"></a>Dönüş Değerleri

- **GX_SUCCESS** (0x00) başarılı pencere duvar kağıdı kümesi
- **GX_CALLER_ERROR** (0x11) bu Işlev için geçersiz çağıran
- **GX_PTR_ERROR** (0x07) geçersiz işaretçi
- **GX_INVALID_WIDGET** (0x12) pencere öğesi geçerli değil

### <a name="allowed-from"></a>İzin verilen

Başlatma ve iş parçacıkları

### <a name="example"></a>Örnek

```C
/* Set wallpaper for window “my_window”. */
status = gx_window_wallpaper_set(&my_window,
                                 MY_WALLPAPER_RESOURCE_ID,
                                 GX_TRUE);

/* If status is GX_SUCCESS the wallpaper for window “my_window” is set. */
```

### <a name="see-also"></a>Ayrıca Bkz.

- gx_window_canvas_set
- gx_window_client_height_get
- gx_window_client_scroll
- gx_window_client_width_get
- gx_window_create
- gx_window_draw
- gx_window_event_process
- gx_window_root_create
- gx_window_root_delete
- gx_window_root_event_process
- gx_window_root_find
-  gx_window_scroll_info_get
- gx_window_scrollbar_find
- gx_window_wallpaper_get