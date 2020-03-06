---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ebf2a79931936e8f45f93cba46b1fefdbf0163b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532881"
---
# <a name="informationalurl-resource-type"></a>Тип ресурса informationalUrl

Пространство имен: microsoft.graph

Основные сведения о профиле приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|logoUrl|Строка|URL-адрес сети CDN для логотипа приложения и только для чтения.|
|маркетингурл|Строка| Ссылка на маркетинговую страницу приложения. Пример: https://www.contoso.com/app/marketing |
|привацистатементурл|Строка| Ссылка на заявление о конфиденциальности приложения. Пример: https://www.contoso.com/app/privacy |
|supportUrl|Строка| Ссылка на страницу поддержки приложения. Пример: https://www.contoso.com/app/support |
|термсофсервицеурл|Строка| Ссылка на условия заявления приложения. Пример: https://www.contoso.com/app/termsofservice |

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
