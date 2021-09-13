---
title: тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: c0f2fa7a71c4512336ada081bd65cd731b3d3165
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129889"
---
# <a name="informationalurl-resource-type"></a>тип ресурса informationalUrl

Пространство имен: microsoft.graph

Основные сведения о профиле приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|logoUrl|Строка|CDN URL-адрес логотипа приложения только для чтения.|
|marketingUrl|Строка| Ссылка на страницу маркетинга приложения. Пример: https://www.contoso.com/app/marketing |
|privacyStatementUrl|Строка| Ссылка на заявление о конфиденциальности приложения. Пример: https://www.contoso.com/app/privacy |
|supportUrl|Строка| Ссылка на страницу поддержки приложения. Пример: https://www.contoso.com/app/support |
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

