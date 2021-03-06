---
title: GUX Studio komut satırı
description: GUX Studio, Studio tarafından oluşturulan çıkış dosyalarını güncelleştirmek için gereken derleme işlem hatları için yararlı olan komut satırı çağrısı sağlar.
author: jdeere5220
ms.author: kemaxwel
ms.date: 9/30/2020
ms.service: rtos
ms.topic: article
ms.openlocfilehash: bd88054d974aabea30b50c6f4e10b4c5df9994db03ab84a4a5d8f9394b4d6ed8
ms.sourcegitcommit: 93d716cf7e3d735b18246d659ec9ec7f82c336de
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/07/2021
ms.locfileid: "116785405"
---
# <a name="chapter-9-guix-studio-command-line"></a>Bölüm 9: Gux Studio komut satırı

GUX Studio, Studio tarafından oluşturulan çıkış dosyalarının güncelleştirilmesi için gereken derleme işlem hatları için yararlı olan komut satırı çağrısını destekler.

## <a name="command-line-usage"></a>Command-Line kullanımı

**Kullanım:** guix_studio \[ seçenek \] \[ bağımsız değişkeni\]

*. GXP* projesini açın.

Studio projesini açın ve istenen çıktı dosyalarını oluşturun.


**Örnekler:**

`guix_studio demo.gxp`  
"Demo. GXP" projesini aç


`guix_studio.exe –p demo.gxp`  
"Demo. GXP" projesini aç


`guix_studio.exe –n –p demo.gxp`  
Demo. GXP projesinin tüm çıkış dosyalarını oluşturur.

`guix_studio.exe –n –r –p demo.gxp`  
Demo. GXP projesinin kaynak dosyalarını oluşturma


## <a name="command-line-options"></a>Command-Line seçenekleri

```C
***-n --nogui***  
```

"Noguı" seçeneği. GUX Studio 'Yu Pencereleme Kullanıcı arabirimi arabirimini başlatmadan çalıştırmayı söyleyin.

```C
***-o pathname***  
***--log***  
```

Günlük seçeneği, bir günlük dosyası belirtin.

```C
***-b***  
***--binary***  
```

İkili kaynak seçeneği. C dosyası yerine bir ikili kaynak dosyası üretir.

```C
***-d display1, display2***  
***--display***  
```

Adları görüntüle seçeneği. Bu seçenek kullanılırsa, oluşturulan herhangi bir kaynak veya belirtim dosyasına yalnızca belirtilen görünen adlar dahil edilir. Bu seçenek kullanılmazsa, tüm ekranlar dahil edilir.

```C
***-t theme1, theme2***  
***--theme***  
```

Tema adı (ler) seçeneği. Bu seçenek kullanılırsa, oluşturulan herhangi bir kaynak veya belirtim dosyasına yalnızca belirtilen Tema adları eklenir. Bu seçenek kullanılmazsa, tüm temalar dahil edilir.

```C
***-l langage1, language2***  
***--language***  
```

Dil adı (ler) seçeneği. Bu seçenek kullanılırsa, belirtilen dil adları oluşturulan kaynak veya belirtim dosyalarına dahil edilir. Aksi takdirde tüm dil adları dahil edilir.

```C
***-r [filename]***  
***--resource***  
```

Kaynak seçeneği, Studio 'Nun önceden belirlenen görüntüler, Temalar ve diller için bir kaynak dosyası üretmesi gerektiğini belirtir.

```C
***-s [filename]***  
***--specification***  
```

Belirtim seçeneği, Studio 'nun belirtilen görüntü, tema ve dil için bir belirtim dosyası üretmesi gerektiğini belirtir.

```C
***-p project_pathname***  
***--project***  
```

Project pathname seçeneği, yüklenecek örnek projeyi belirtin.

```C
***-i [pathname]***  
***--import***  
```

Dizeyi XLIFF veya CSV biçim dosyasından içeri aktarın.

***--big_endian***  
Büyük endian biçiminde kaynak verileri oluşturun.
