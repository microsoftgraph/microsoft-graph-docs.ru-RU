---
title: Тип ресурса учетных данных
description: Указывает один учетный документ, используемый для входа в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0521f766a7a0da482cf67628c3816935ee9270b8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761683"
---
# <a name="credential-resource-type"></a>Тип ресурса учетных данных

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает один учетный документ, используемый для входа в приложение. Например, имя пользователя — это один учетный данные, пароль — другой учетный данные.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|fieldId|String|Имя поля для этого учетного данных. например, имя пользователя, пароль или phoneNumber. Это определяется приложением. Должно совпадать с тем, что находится в html-поле на объекте singleSignOnSettings/password.|
|type|String|Тип для этого учетного данных. Допустимые значения: имя пользователя, пароль или другие.|
|value|String|Значение для этого учетного данных. например, mysuperhiddenpassword. Обратите внимание, что значение для паролей является только для записи, значение никогда не может быть прочитано обратно.|

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


