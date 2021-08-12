---
title: тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: e0c60cdde2d636321f3777b4b41bdf11bfe1da69d3303169f4fce1a3a71b3acc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178391"
---
# <a name="informationalurl-resource-type"></a>тип ресурса informationalUrl

Пространство имен: microsoft.graph

Основные сведения о профиле приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|logoUrl|String|CDN URL-адрес логотипа приложения только для чтения.|
|marketingUrl|String| Ссылка на страницу маркетинга приложения. Пример: https://www.contoso.com/app/marketing |
|privacyStatementUrl|String| Ссылка на заявление о конфиденциальности приложения. Пример: https://www.contoso.com/app/privacy |
|supportUrl|String| Ссылка на страницу поддержки приложения. Пример: https://www.contoso.com/app/support |
|termsOfServiceUrl|String| Ссылка на условия службы приложения. Пример: https://www.contoso.com/app/termsofservice |

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

