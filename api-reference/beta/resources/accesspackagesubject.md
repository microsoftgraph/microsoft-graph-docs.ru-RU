---
title: Тип ресурса Акцесспаккажесубжект
description: В службе управления обслуживанием Azure AD тема назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0b37d91ad5669a0a87cef91893babf392f2f309b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939406"
---
# <a name="accesspackagesubject-resource-type"></a>Тип ресурса Акцесспаккажесубжект

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)субъектом пакета Access является пользователь, участник службы или другой объект, который можно настроить для запроса или назначения пакета доступа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Отображаемое имя субъекта.|
|email|String|Адрес электронной почты субъекта.|
|id|String| Только для чтения.|
|objectId|Строка|Идентификатор объекта subject.|
|principalName|Строка|Имя участника (если оно известно) субъекта.|
|type|String|Тип ресурса субъекта.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "baseType": "",
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
