---
title: Belirli pencere öğesi türlerini düzenlemeyle ilgili notlar
description: Belirli karmaşık pencere öğesi türleri için Düzenle yöntemlerini açıklayan ayrıntılı açıklamalar.
author: jdeere5220
ms.author: kemaxwel
ms.date: 9/30/2020
ms.service: rtos
ms.topic: article
ms.openlocfilehash: 3194a1b8c8965bf821631a8c34ac5e9961f8c8ff
ms.sourcegitcommit: e3d42e1f2920ec9cb002634b542bc20754f9544e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104827125"
---
# <a name="chapter-8-notes-on-editing-specific-widget-types"></a><span data-ttu-id="ac50f-103">Bölüm 8: belirli pencere öğesi türlerini düzenlemeyle ilgili notlar</span><span class="sxs-lookup"><span data-stu-id="ac50f-103">Chapter 8: Notes on Editing Specific Widget Types</span></span>

<span data-ttu-id="ac50f-104">GUX Studio, kullanıcının uygulama kullanıcı arabirimi ekranlarını oluşturacak olan Gux pencere öğelerini kolayca oluşturmasını ve değiştirmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="ac50f-104">GUIX Studio allows the user to easily create and modify GUIX widgets that will compose the application UI screens.</span></span> <span data-ttu-id="ac50f-105">Bu düzenlemenin çoğu sezgisel ve açıktır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-105">Most of these editing methods are intuitive and obvious.</span></span> <span data-ttu-id="ac50f-106">Örneğin, bir pencere öğesini yeniden boyutlandırmak için fare ile pencere öğesini seçebilir ve pencere öğesi kenarlıklarını sürükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ac50f-106">For example, to resize a widget you can select the widget with the mouse and drag the widget borders.</span></span> <span data-ttu-id="ac50f-107">Ayrıca, seçilen pencere öğesinin sol/üst/genişlik/yükseklik özellik alanlarına doğrudan yazabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ac50f-107">You can also directly type into the left/top/width/height property fields of the selected widget.</span></span>

<span data-ttu-id="ac50f-108">Bazı pencere öğesi türleri daha gelişmiş bir Düzenle işlemi gerektirir, çünkü bu pencere öğeleri kendi özellik desteğiyle bir bit daha karmaşıktır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-108">Certain widget types require a more advanced editing process, because these widgets are themselves a bit more sophisticated in their feature support.</span></span>

<span data-ttu-id="ac50f-109">Bu bölümde, bu daha karmaşık pencere öğesi türleri için daha gelişmiş Düzenle özelliklerine ilişkin notlar sağlanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-109">This chapter provides notes on the more advanced editing features for these more complex widget types.</span></span> <span data-ttu-id="ac50f-110">Bu notlar, Guix kitaplığı 'nda sunulan pencere öğesi türleriyle birlikte Gux Studio 'nun özellikleri ile ileriye yönelik özellikler olarak genişletilir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-110">These notes will expand as the features of GUIX Studio advance along with the widget types provided within the GUIX library.</span></span>

## <a name="rich-text-view"></a><span data-ttu-id="ac50f-111">Zengin metin görünümü</span><span class="sxs-lookup"><span data-stu-id="ac50f-111">Rich Text View</span></span>

<span data-ttu-id="ac50f-112">Bu pencere öğesi, satır içi metin biçimlendirme kodlarını destekleyen zengin metinleri göstermek için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-112">This widget is used to display rich text that supports inline text formatting codes.</span></span> <span data-ttu-id="ac50f-113">Bu biçimlendirme kodları kalın, italik ve diğer birkaç tane içerir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-113">These formatting codes include bold, italic, and several others.</span></span> <span data-ttu-id="ac50f-114">Başlamak için *proje görünümü* veya *hedef görünümü* ' nden seçilen üst öğeye sağ tıklayın ve zengin metin görünümü pencere öğesi eklemek Için menü **Ekle/metin/zengin metin görünümü** ' nü seçin.</span><span class="sxs-lookup"><span data-stu-id="ac50f-114">To begin, right-click on the selected parent from the *Project View* or *Target View* and select menu **Insert/Text/Rich Text View** to insert a rich text view widget.</span></span>

<span data-ttu-id="ac50f-115">Tüm pencere öğesi türleri tarafından desteklenen standart özellik kümesine ek olarak, zengin metin görünümü pencere öğesi türü ek özellikleri destekler.</span><span class="sxs-lookup"><span data-stu-id="ac50f-115">In addition to the standard set of properties supported by all widget types, the Rich Text View widget type supports additional properties.</span></span>

### <a name="additional-properties"></a><span data-ttu-id="ac50f-116">Ek özellikler</span><span class="sxs-lookup"><span data-stu-id="ac50f-116">Additional Properties</span></span>

| <span data-ttu-id="ac50f-117">Özellik</span><span class="sxs-lookup"><span data-stu-id="ac50f-117">Property</span></span> | <span data-ttu-id="ac50f-118">Anlamı</span><span class="sxs-lookup"><span data-stu-id="ac50f-118">Meaning</span></span> |
|----------|---------|
| <span data-ttu-id="ac50f-119">Metin Hizala</span><span class="sxs-lookup"><span data-stu-id="ac50f-119">Text Align</span></span> | <span data-ttu-id="ac50f-120">Varsayılan metin hizalaması</span><span class="sxs-lookup"><span data-stu-id="ac50f-120">Default text alignment</span></span> |
| <span data-ttu-id="ac50f-121">Normal yazı tipi</span><span class="sxs-lookup"><span data-stu-id="ac50f-121">Normal Font</span></span>| <span data-ttu-id="ac50f-122">Varsayılan metin yazı tipi</span><span class="sxs-lookup"><span data-stu-id="ac50f-122">Default text font</span></span> |
| <span data-ttu-id="ac50f-123">Kalın yazı tipi</span><span class="sxs-lookup"><span data-stu-id="ac50f-123">Bold Font</span></span>  | <span data-ttu-id="ac50f-124">Kalın olarak etiketlenen metnin metin yazı tipi</span><span class="sxs-lookup"><span data-stu-id="ac50f-124">Text font for text tagged as bold</span></span> |
| <span data-ttu-id="ac50f-125">İtalik yazı tipi</span><span class="sxs-lookup"><span data-stu-id="ac50f-125">Italic Font</span></span>| <span data-ttu-id="ac50f-126">İtalik olarak etiketlenen metnin metin yazı tipi</span><span class="sxs-lookup"><span data-stu-id="ac50f-126">Text font for text tagged as italic</span></span>|
| <span data-ttu-id="ac50f-127">Kalın Italik yazı tipi</span><span class="sxs-lookup"><span data-stu-id="ac50f-127">Bold Italic Font</span></span>| <span data-ttu-id="ac50f-128">Kalın ve italik olarak etiketlenen metnin metin yazı tipi</span><span class="sxs-lookup"><span data-stu-id="ac50f-128">Text font for text tagged as bold and italic</span></span> |
| <span data-ttu-id="ac50f-129">Özel metin kopyalama</span><span class="sxs-lookup"><span data-stu-id="ac50f-129">Private Text Copy</span></span> | <span data-ttu-id="ac50f-130">Pencere öğesi atanmış metinlerin kendisine ait özel kopyasını tutmadıysanız, denetlenmesi gerekir</span><span class="sxs-lookup"><span data-stu-id="ac50f-130">Should be checked if the widget is to keep its own private copy of any text assigned</span></span> |
| <span data-ttu-id="ac50f-131">Boşluk</span><span class="sxs-lookup"><span data-stu-id="ac50f-131">Whitespace</span></span> | <span data-ttu-id="ac50f-132">Pencere öğesi ile görüntülenmiş metin arasındaki kenar boşluğunun piksel cinsinden genişliği.</span><span class="sxs-lookup"><span data-stu-id="ac50f-132">Width of margin between the widget and the displayed text, in pixels.</span></span> |
| <span data-ttu-id="ac50f-133">Satır alanı</span><span class="sxs-lookup"><span data-stu-id="ac50f-133">Line Space</span></span> | <span data-ttu-id="ac50f-134">Metnin iki satırı arasındaki boşluk (piksel cinsinden).</span><span class="sxs-lookup"><span data-stu-id="ac50f-134">Space between two lines of the text, in pixels.</span></span> |
|||

### <a name="the-rich-text-formatting-codes"></a><span data-ttu-id="ac50f-135">Zengin metin biçimlendirme kodları</span><span class="sxs-lookup"><span data-stu-id="ac50f-135">The Rich Text formatting codes</span></span>

<span data-ttu-id="ac50f-136">Metin biçimlendirme için aşağıdaki biçim kodları desteklenir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-136">The following format codes are supported for text formatting.</span></span>

|<span data-ttu-id="ac50f-137">Etiket</span><span class="sxs-lookup"><span data-stu-id="ac50f-137">Tag</span></span>|<span data-ttu-id="ac50f-138">Anlamı</span><span class="sxs-lookup"><span data-stu-id="ac50f-138">Meaning</span></span>|
|---|---|
|\<b>\</b> | <span data-ttu-id="ac50f-139">Metin yazı tipini Kullanıcı tarafından belirtilen kalın yazı tipi KIMLIĞIYLE işle</span><span class="sxs-lookup"><span data-stu-id="ac50f-139">Render text font with user specified bold font ID</span></span>|
|\<i>\</i> | <span data-ttu-id="ac50f-140">Metin yazı tipini Kullanıcı tarafından belirtilen italik yazı tipi KIMLIĞIYLE işle</span><span class="sxs-lookup"><span data-stu-id="ac50f-140">Render text font with user specified italic font ID</span></span>|
|\<u>\</u> | <span data-ttu-id="ac50f-141">Altı çizili metni işle</span><span class="sxs-lookup"><span data-stu-id="ac50f-141">Render underlined text</span></span>|
|\<f GX_FONT_ID>\</f> | <span data-ttu-id="ac50f-142">Belirtilen yazı tipi KIMLIĞINI kullanarak metni işle.</span><span class="sxs-lookup"><span data-stu-id="ac50f-142">Render text using the specified font ID.</span></span> |
|\<c GX_COLOR_ID>\</c> | <span data-ttu-id="ac50f-143">Belirtilen renk KIMLIĞINI kullanarak metni işle</span><span class="sxs-lookup"><span data-stu-id="ac50f-143">Render text using the specified color ID</span></span>|
|\<hc GX_COLOR_ID>\</hc> | <span data-ttu-id="ac50f-144">Belirtilen arka plan rengi KIMLIĞINI kullanarak metin işle</span><span class="sxs-lookup"><span data-stu-id="ac50f-144">Render text using the specified background color ID</span></span>|
|\<align left/right/center>\</align> | <span data-ttu-id="ac50f-145">Metin hizalaması ata</span><span class="sxs-lookup"><span data-stu-id="ac50f-145">Assign text alignment</span></span>|
|||

<span data-ttu-id="ac50f-146">GUX Studio içinden zengin metin dizesini düzenlemenin iki yolu vardır:</span><span class="sxs-lookup"><span data-stu-id="ac50f-146">There are two ways to edit the rich text string from within GUIX Studio:</span></span>

- <span data-ttu-id="ac50f-147">Önerilen ve en basit düzenleme yöntemi olan zengin metin Düzenle iletişim kutusunu kullanın.</span><span class="sxs-lookup"><span data-stu-id="ac50f-147">Use the Edit Rich Text dialog, which is the recommended and simplest editing method.</span></span>
- <span data-ttu-id="ac50f-148">Yukarıdaki tabloda gösterilen biçimlendirme etiketlerini el ile eklemenize olanak tanıyan dize tablosu Düzenleyicisi iletişim kutusunu kullanın.</span><span class="sxs-lookup"><span data-stu-id="ac50f-148">Use the String Table Editor dialog, which allows you to manually insert the formatting tags shown in the preceding table.</span></span>

<span data-ttu-id="ac50f-149">*Hedef görünümde* zengin metin görünümü pencere öğesi seçildikten sonra, Şekil 8,1 ' de gösterilen zengin metin düzenleme iletişim kutusunu çağırmak Için *Özellikler görünümündeki* **zengin metin Düzenle** düğmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="ac50f-149">After selecting a Rich Text View widget in the *Target View*, select the **Edit Rich Text** button in the *Properties View* to invoke the  rich text edit dialog, shown in Figure 8.1.</span></span>

![GUX Studio zengin metin düzenleme iletişim kutusunun ekran görüntüsü.](./media/guix-studio/edit_rich_text_dialog.png)

<span data-ttu-id="ac50f-151">**Şekil 8,1**</span><span class="sxs-lookup"><span data-stu-id="ac50f-151">**Figure 8.1**</span></span>

<span data-ttu-id="ac50f-152">Sol bölme zengin metin düzenleme alanıdır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-152">The left pane is the rich text edit field.</span></span> <span data-ttu-id="ac50f-153">Araç çubuğu simgelerini, ihtiyacınız olan etiketleri eklemeye yardımcı olması için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ac50f-153">You can use the toolbar icons to help insert tags you require.</span></span> <span data-ttu-id="ac50f-154">Düzenleme alanında herhangi bir metin bloğunu seçin ve ardından gerekli stilleri ve renkleri seçili metin bloğuna uygulamak için araç çubuğu düğmelerini seçin.</span><span class="sxs-lookup"><span data-stu-id="ac50f-154">Select any block of text in the edit field, and then select the toolbar buttons to apply the required styles and colors to the selected text block.</span></span> <span data-ttu-id="ac50f-155">Zengin metin Düzenle iletişim kutusu, biçimlendirme kodlarını test dizesine eklemenin kolay bir yoludur.</span><span class="sxs-lookup"><span data-stu-id="ac50f-155">The Edit Rich Text dialog is an easy way to insert the formatting codes into the test string.</span></span> <span data-ttu-id="ac50f-156">Ayrıca, bu etiketleri el ile ekleyebilir veya gerekirse çalışma zamanında oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ac50f-156">You can also insert these tags manually or even generate them at runtime if needed.</span></span>

<span data-ttu-id="ac50f-157">Sağ bölme, metnin hedef görünümde nasıl işleneceğini göstermek için pencere öğesi önizlemesidir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-157">The Right pane is the widget preview to show how the text is rendered in the target view.</span></span> <span data-ttu-id="ac50f-158">Pencere öğesi önizlemenin arka plan rengi düzeltildi, bu işlem, hedef görünümdeki pencere öğesinin atanan arka plan rengiyle eşleşmeyebilir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-158">The background color of the widget preview is fixed, which may not match the widget's assigned background color in the target view.</span></span>

<span data-ttu-id="ac50f-159">Kaynak KIMLIĞI adları, belirli yazı tipine veya renk kaynaklarına başvurmak için zengin metin halinde kullanılır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-159">Resource ID names are used in rich text to reference specific font or color resources.</span></span> <span data-ttu-id="ac50f-160">Bir fontun veya rengin kaynak adı, zengin metin dizesi tarafından başvurulduktan sonra değiştirilirse, GUıDX Studio zengin metin dizesini kaynak adı değişikliklerini yansıtacak şekilde otomatik olarak güncelleştirir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-160">If the resource name of a font or color is changed after it has been referenced by the rich text string, GUIX Studio will automatically update the rich text string to reflect the resource name changes.</span></span> <span data-ttu-id="ac50f-161">Diğer taraftan, bir zengin metin pencere öğesi tarafından başvurulan bir yazı tipini veya renk kaynağını silerseniz, silinen kaynak KIMLIĞI adlarını kaldırmak veya değiştirmek için etkilenen zengin metni el ile düzenlemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-161">On the other hand if you delete a font or color resource that is referenced by a rich text widget, you must edit the affected rich text manually to remove or change the resource ID names that have been deleted.</span></span>

<span data-ttu-id="ac50f-162">Bu iletişim kutusunda Kaydet düğmesini seçtiğinizde, tanımladığınız zengin metin dizesi proje dizesi tablosuna eklenir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-162">When you select the Save button in this dialog, the rich text string you have defined is added to the project string table.</span></span>

## <a name="string-scroll-wheel"></a><span data-ttu-id="ac50f-163">Dize kaydırma tekerleği</span><span class="sxs-lookup"><span data-stu-id="ac50f-163">String Scroll Wheel</span></span>

<span data-ttu-id="ac50f-164">Bir dize kaydırma tekerleği pencere öğesi dizeler dizisinin görüntülenmesini destekler.</span><span class="sxs-lookup"><span data-stu-id="ac50f-164">A string scroll wheel widget supports the display of an array of strings.</span></span> <span data-ttu-id="ac50f-165">Bu dizeler dinamik olarak atanabilir veya uygulamanın birden çok dili desteklemesi durumunda, atanan dizelerin etkin dize tablosundan çekbir şekilde atanabilmesini sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-165">These strings may be dynamically assigned, or, in the case that the application supports multiple languages, the assigned strings can be pulled from the active string table.</span></span>

<span data-ttu-id="ac50f-166">Dize kaydırma tekerleği pencere öğesi bir dizi dizeyi destekler.</span><span class="sxs-lookup"><span data-stu-id="ac50f-166">The string scroll wheel widget supports an array of strings.</span></span> <span data-ttu-id="ac50f-167">Şekil 8,2 ' de gösterilen dize kaydırma tekerleği düzenleme iletişim kutusu, kullanıcının bu dize dizisini atamasına izin vermek için verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-167">The String Scroll Wheel Edit dialog, shown in Figure 8.2, is provided to allow the user to assign this array of strings.</span></span>

![GUX Studio dize kaydırma tekerleği düzenleme iletişim kutusunun ekran görüntüsü.](./media/guix-studio/string_scroll_wheel_edit.png)

<span data-ttu-id="ac50f-169">**Şekil 8,2**</span><span class="sxs-lookup"><span data-stu-id="ac50f-169">**Figure 8.2**</span></span>

<span data-ttu-id="ac50f-170">Bu iletişim kutusunu çağırmak için *hedef görünüm* veya *proje görünümü* içinde bir dize kaydırma tekerleği pencere öğesi seçin.</span><span class="sxs-lookup"><span data-stu-id="ac50f-170">To invoke this dialog, select a string scroll wheel widget within the *Target View* or the *Project View*.</span></span> <span data-ttu-id="ac50f-171">Bu pencere öğesi türü seçildikten sonra, *Özellikler Görünümü* **dizeleri Düzenle** düğmesi içerecektir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-171">Once this widget type is selected, the *Properties View* will include an **Edit Strings** button.</span></span> <span data-ttu-id="ac50f-172">Dize kaydırma tekerleği düzenleme iletişim kutusunu çağırmak için bu düğmeyi seçin.</span><span class="sxs-lookup"><span data-stu-id="ac50f-172">Select this button to invoke the String Scroll Wheel Edit dialog.</span></span>

<span data-ttu-id="ac50f-173">Her metin dizini için bir dize atamak üzere, açılan listeden bir dize KIMLIĞI seçebilir veya sağdaki metin alanına yeni bir dize değeri yazabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ac50f-173">To assign a string for each text index, you can either select a string ID from the drop-down list, or you can type a new string value in the Text field on the right.</span></span> <span data-ttu-id="ac50f-174">Yaptığınız değişikliklerle işiniz bittiğinde, tüm yeni veya değiştirilmiş dizeler etkin dize tablosuna kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-174">When you are done with your changes, any new or modified strings are saved to the active string table.</span></span>

## <a name="sprite"></a><span data-ttu-id="ac50f-175">Öğesini</span><span class="sxs-lookup"><span data-stu-id="ac50f-175">Sprite</span></span>

<span data-ttu-id="ac50f-176">Bir sprite pencere öğesi, bir animasyon efekti sağlamak üzere bir görüntü dizisini göstermek için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-176">A sprite widget is used to display a sequence of images to provide an animation effect.</span></span> <span data-ttu-id="ac50f-177">Bir sprite pencere öğesi, çerçevedeki her bir görüntüye uygulanan bir resim kimlikleri ve benzersiz parametreler dizisi olan bir çerçeve listesi gerektirir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-177">A sprite widget requires a frame list, which is an array of image IDs and unique parameters applied to each image in the frame.</span></span> <span data-ttu-id="ac50f-178">Hareketli pencere öğesi için bu çerçeve listesini oluşturmak için Şekil 8,3 ' de gösterilen Sprite çerçevelerini Düzenle iletişim kutusu sağlanır:</span><span class="sxs-lookup"><span data-stu-id="ac50f-178">To build this frame list for the sprite widget the Edit Sprite Frames dialog, shown in figure 8.3, is provided:</span></span>

![GUX Studio Sprite çerçeveleri düzenleme iletişim kutusunun ekran görüntüsü.](./media/guix-studio/edit_sprite_frames.png)

<span data-ttu-id="ac50f-180">**Şekil 8,3**</span><span class="sxs-lookup"><span data-stu-id="ac50f-180">**Figure 8.3**</span></span>

<span data-ttu-id="ac50f-181">Bu iletişim kutusunu çağırmak için *hedef görünüm* veya *proje görünümü* içinde bir sprite pencere öğesi seçin.</span><span class="sxs-lookup"><span data-stu-id="ac50f-181">To invoke this dialog, select a sprite widget within the *Target View* or the *Project View*.</span></span> <span data-ttu-id="ac50f-182">Bu pencere öğesi türü seçildikten sonra, *Özellikler Görünümü* bir **Framelist düğmesini Düzenle** düğmesi içerecektir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-182">Once this widget type is selected, the *Properties View* will include an **Edit Framelist** button.</span></span> <span data-ttu-id="ac50f-183">Dize kaydırma tekerleği düzenleme iletişim kutusunu çağırmak için bu düğmeyi seçin.</span><span class="sxs-lookup"><span data-stu-id="ac50f-183">Select this button to invoke the String Scroll Wheel Edit dialog.</span></span>

<span data-ttu-id="ac50f-184">*Toplam Sprite çerçevesi sayısı* alanı, Sprite pencere öğesi tarafından görüntülenecek toplam çerçeve sayısını girmenize olanak sağlayan bir giriş alanıdır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-184">The *Total number of Sprite Frames* field is an input field allowing you to enter the integer total number of frames to be displayed by the sprite widget.</span></span> <span data-ttu-id="ac50f-185">Görüntüler çerçeve listesi içinde yeniden kullanılabilir, yani her görüntü benzersiz olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-185">Images can be reused within the frame list, meaning not every image must be unique.</span></span>

<span data-ttu-id="ac50f-186">Sprite çerçeve KIMLIĞI alanı, 1 ' den toplam çerçeve sayısıyla değişen bir çerçeve dizini seçim değeridir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-186">The Sprite Frame ID field is a frame index selection value that ranges from 1 to Total number of Frames.</span></span> <span data-ttu-id="ac50f-187">Bir sprite çerçevesinin yanına ilerlemek için bu değeri artırın ve azaltır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-187">Increment and Decrement this value to move from one sprite frame to the next.</span></span>

<span data-ttu-id="ac50f-188">Her Sprite çerçevesinin çeşitli parametreleri vardır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-188">Each sprite frame has several parameters.</span></span> <span data-ttu-id="ac50f-189">Birincisi, arka plan Işlemidir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-189">The first is the Background Operation.</span></span> <span data-ttu-id="ac50f-190">Bu alan popüler GIF animasyon biçiminin yeteneklerini taklit eder.</span><span class="sxs-lookup"><span data-stu-id="ac50f-190">This field mimics the capabilities of the popular GIF animation format.</span></span> <span data-ttu-id="ac50f-191">Buradaki seçimler şunları içerir:</span><span class="sxs-lookup"><span data-stu-id="ac50f-191">The choices here include:</span></span>

- <span data-ttu-id="ac50f-192">Işlem yok, bu, geçerli çerçeve görüntüsünün önceki çerçeve görüntüsünün üzerine çizildiği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-192">No Operation, which means the current frame image is drawn over the previous frame image.</span></span>
- <span data-ttu-id="ac50f-193">Ilk piksel eşlemesini geri yükle, yani 1 piksel eşlemesinin geçerli piksel eşlemesinden önce çizildiği ve</span><span class="sxs-lookup"><span data-stu-id="ac50f-193">Restore First Pixel-map, which means the index 1 pixel-map is drawn before the current pixel-map and</span></span>
- <span data-ttu-id="ac50f-194">Düz renk dolgusu, bu, Sprite arka planının, geçerli çerçevenin çizilmeden önce Sprite arka plan rengiyle doldurulduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-194">Solid Color Fill, which means the sprite background is filled with the sprite background color before the current frame is drawn.</span></span>

<span data-ttu-id="ac50f-195">Pixel-Map KIMLIĞI alanı, daha önce proje kaynaklarına eklenmiş herhangi bir piksel eşlemesini seçmenizi sağlar.</span><span class="sxs-lookup"><span data-stu-id="ac50f-195">The Pixel-map ID field allows you to select any pixel-map previously added to the project resources.</span></span> <span data-ttu-id="ac50f-196">Aynı piksel eşleme KIMLIĞI birden çok çerçeve için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-196">The same pixel-map ID can be used for multiple frames.</span></span> <span data-ttu-id="ac50f-197">Örneğin, Sprite animasyonunuz, farklı Sprite görüntülerini kullanmanın yanı sıra görüntünün hareketini (x ve y boşluğu alanlarını kullanarak) kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-197">For example your sprite animation might utilize movement of the image (using the x and y offset fields) instead of or in addition to using different sprite images.</span></span>

<span data-ttu-id="ac50f-198">Alfa değeri alanı piksel eşleme çiziminin tamamına uygulanır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-198">The Alpha value field is applied to the entire pixel-map drawing.</span></span> <span data-ttu-id="ac50f-199">Bu alanın yalnızca 8 BPP renk derinliği ve üzeri sürümlerde çalıştığı bir etkisi vardır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-199">This field only has an effect when running at 8 bpp color depth and higher.</span></span> <span data-ttu-id="ac50f-200">Alfa değeri 0 tamamen saydamdır ve alfa değeri 255 donuk olur.</span><span class="sxs-lookup"><span data-stu-id="ac50f-200">Alpha value 0 is fully transparent, and alpha value 255 is opaque.</span></span>

<span data-ttu-id="ac50f-201">Geçerli piksel eşlemesinin x-kayması ve Frame y-kayması alanları kullanılarak çizileceği hareketli kare içinde bir konum belirtebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ac50f-201">You can specify an offset within the sprite frame at which the current pixel-map will be drawn using the Frame x-offset and Frame y-offset fields.</span></span> <span data-ttu-id="ac50f-202">Diğer bir deyişle, çizilen her görüntünün, Sprite pencere öğesinin tam boyutu olması gerekmez.</span><span class="sxs-lookup"><span data-stu-id="ac50f-202">In other words, each image drawn does not have to be the full size of the sprite widget.</span></span>

<span data-ttu-id="ac50f-203">Gecikme süresi, sonraki Sprite çerçevesine geçmeden önce gecikme süresini belirtir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-203">The Delay period specifies the time to delay before moving to the next sprite frame.</span></span> <span data-ttu-id="ac50f-204">Bu değer, varsayılan Gux/ThreadX Zamanlayıcı yapılandırması için her tick 50 MS 'yi temsil eden Tick 'dır.</span><span class="sxs-lookup"><span data-stu-id="ac50f-204">This value is in ticks, which for the default GUIX/ThreadX timer configuration each tick represents 50 ms.</span></span>

<span data-ttu-id="ac50f-205">Değişiklikleri Sprite çerçevelerini Düzenle iletişim kutusunda kaydettiğinizde, GUıDX Studio, çıkış belirtimleri dosya oluşturmanın bir parçası olarak tüm Çerçeve listesi dizisini üretebilir.</span><span class="sxs-lookup"><span data-stu-id="ac50f-205">When you save your changes in the Edit Sprite Frames dialog, GUIX Studio is able to generate the complete frame list array as part of the output specifications file generation.</span></span>