---
title: Тип ресурса accessPackageSubject
description: В управлении правами Azure AD субъект назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3f5bbd3147b27193d8a8e8a3e4bea3914719124c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161784"
---
# <a name="accesspackagesubject-resource-type"></a>Тип ресурса accessPackageSubject

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-root.md)субъектом пакета доступа является пользователь, субъект-служба или другая сущность, которую можно настроить для запроса или получения пакета доступа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Отображаемого имени темы.|
|email|String|Адрес электронной почты темы.|
|id|String| Только для чтения.|
|objectId|String|ИД объекта темы.|
|principalName|String|Имя субъекта( если известно) темы.|
|type|String|Тип ресурса темы.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "Administrator",
  "email": "admin@contoso.com",
  "id": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
  "objectId": "cc754ed5-f598-45c0-aaf0-fc2f2eb1838f",
  "principalName": "admin@domain.contoso.com",
  "type": "User"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageSubject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


