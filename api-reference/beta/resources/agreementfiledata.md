---
title: Тип ресурса agreementFileData
description: Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.
ms.openlocfilehash: 557725e14f4954f8b2c10112e1013beb71dda0be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078732"
---
# <a name="agreementfiledata-resource-type"></a>Тип ресурса agreementFileData

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.

## <a name="properties"></a>Свойства
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|data|Двоичный|Данные, представляющие условия использования PDF-документа. Только для чтения.|

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
