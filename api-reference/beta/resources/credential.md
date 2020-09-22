---
title: Тип ресурса Credential
description: Указывает одну учетную запись, используемую для входа в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a281e39850ea18ee3bcbe0d83c5df3b41d0ccd31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016690"
---
# <a name="credential-resource-type"></a>Тип ресурса Credential

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает одну учетную запись, используемую для входа в приложение. Например, username это один учетный набор учетных данных, пароль — это еще одна учетная запись.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|fieldId|String|Имя поля для этих учетных данных. Например, имя пользователя или пароль или phoneNumber. Это определяется приложением. Должно отличаться от того, что указано в поле HTML в объекте Синглесигнонсеттингс/Password.|
|type|String|Тип для этих учетных данных. Допустимые значения: username, Password или other.|
|value|String|Значение для этих учетных данных. Например, мисуперхидденпассворд. Примечание. значение для паролей доступно только для записи, его значение не может быть прочитано обратно.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credential",
  "baseType": null
}-->

```json
{
  "fieldId": "param_username",
  "value": "myusername",
  "type": "username"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


