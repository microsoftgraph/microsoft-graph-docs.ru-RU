---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9e2eaad003f4669623a4db4af1b364e05198515d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006257"
---
# <a name="informationalurl-resource-type"></a>Тип ресурса informationalUrl

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Основные сведения о профиле приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|проведения|String| Ссылка на маркетинговую страницу приложения. Пример: https://www.contoso.com/app/marketing |
|уведомление|String| Ссылка на заявление о конфиденциальности приложения. Пример: https://www.contoso.com/app/privacy |
|поддержки|String| Ссылка на страницу поддержки приложения. Пример: https://www.contoso.com/app/support |
|Термсофсервице|String| Ссылка на условия заявления приложения. Пример: https://www.contoso.com/app/termsofservice |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
