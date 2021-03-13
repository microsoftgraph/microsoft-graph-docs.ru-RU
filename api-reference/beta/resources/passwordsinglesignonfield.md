---
title: тип ресурса passwordSingleSignOnField
description: Поля для захвата учетных данных для SSO пароля
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e0db6198d61715603acee54e7351c9fd5f2fed88
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761551"
---
# <a name="passwordsinglesignonfield-resource-type"></a>тип ресурса passwordSingleSignOnField

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит поля для захвата для заполнения учетных данных использования для одного входа на основе пароля.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|customizedLabel|String|Переопределение заголовка или метки для настройки.|
|defaultLabel|String|Метка, которая будет использоваться, если не будет предоставлена настройкаLabel. Только для чтения.|
|fieldId|String|Идентификатор, используемый для удостоверения типа поля. Это внутренний id и возможные значения `param_1` , `param_2` , `param_userName` `param_password` .|
|type|String|   Тип учетных данных. Значения могут быть `text` , `password` .|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnField",
  "baseType": null
}-->

```json
{
  "customizedLabel": "String",
  "defaultLabel": "String",
  "fieldId": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

