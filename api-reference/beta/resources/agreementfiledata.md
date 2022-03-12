---
title: тип ресурса agreementFileData
description: Представляет blob из Azure Active Directory (Azure AD) терминов файла соглашения об использовании.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 3fa6c94497ae42b102f03bee6142ec38677eda93
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451314"
---
# <a name="agreementfiledata-resource-type"></a>тип ресурса agreementFileData

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет blob из Azure Active Directory (Azure AD) терминов файла соглашения об использовании.

## <a name="properties"></a>Свойства
| Свойство       | Тип | Описание |
|:-------------|:------------|:------------|
|data|Binary|Данные, которые представляют условия использования документа PDF. Только для чтения. <br/><br/>**Примечание:** Вы можете использовать метод .NET [Convert.ToBase64String](/dotnet/api/system.convert.tobase64string) для преобразования файла в двоичные данные для загрузки с помощью API [Create agreements](../api/termsofusecontainer-post-agreements.md) . Пример синтаксиса с использованием этого метода в PowerShell .`[convert]::ToBase64String((Get-Content -path "your_file_path" -Encoding byte))` |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


