---
title: Перечисление fileHashType
description: Перечисление для типов файлов хэш-функции.
localization_priority: Normal
ms.openlocfilehash: 082fdd9cdad6c3ec1ea4e07020983ac0bac7ed65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518382"
---
# <a name="filehashtype-enum"></a>Перечисление fileHashType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Перечисление для типов файлов хэш-функции.

## <a name="members"></a>Элементы

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|(0)|Неизвестный тип.|
|SHA1|$1|Тип хэш SHA1.|
|SHA256|–2| Тип SHA256 хэш-функции.|
|MD5|–3| Тип хэш MD5.|
|authenticodeHash256|4| Тип AuthenticodeHash256 хэш-функции.|
|lsHash|$-5| Тип LsHash хэш-функции.|
|ctph|6| Тип CTPH хэш-функции.|
|peSha1|7| Тип PESHA1 хэш-функции.|
|peSha256|: = 8| Тип PESHA256 хэш-функции.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/filehashtypeenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
