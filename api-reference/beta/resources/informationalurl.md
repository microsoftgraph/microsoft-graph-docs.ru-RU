---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 23c1baa55a8cc50b77f429898614f54e02b7813c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016499"
---
# <a name="informationalurl-resource-type"></a>Тип ресурса informationalUrl

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Основные сведения о профиле приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|logoUrl|String|URL-адрес сети CDN для логотипа приложения и только для чтения.|
|маркетингурл|String| Ссылка на маркетинговую страницу приложения. Пример: https://www.contoso.com/app/marketing |
|привацистатементурл|String| Ссылка на заявление о конфиденциальности приложения. Пример: https://www.contoso.com/app/privacy |
|supportUrl|String| Ссылка на страницу поддержки приложения. Пример: https://www.contoso.com/app/support |
|термсофсервицеурл|String| Ссылка на условия заявления приложения. Пример: https://www.contoso.com/app/termsofservice |

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
  "logoUrl": "String",
  "marketingUrl": "String",
  "privacyStatementUrl": "String",
  "supportUrl": "String",
  "termsOfServiceUrl": "String"
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


