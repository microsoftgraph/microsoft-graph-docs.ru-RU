---
title: тип ресурсов accessPackageSubject
description: В управлении правами Azure AD субъект назначения пакета доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5092494b1c5f496a1ee3abf76800dbb8a05f49ff
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651184"
---
# <a name="accesspackagesubject-resource-type"></a>тип ресурсов accessPackageSubject

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-overview.md)субъект пакета доступа — это пользователь, руководитель службы или другая сущность, которую можно настроить для запроса или присвоения пакета доступа.  Он может представлять запросителя из связанной организации, который еще не находится в клиенте.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Отображение имени субъекта.|
|email|String|Адрес электронной почты субъекта.|
|id|String| Только для чтения.|
|objectId|String|Идентификатор объекта субъекта. `null` если субъект еще не является пользователем в клиенте.|
|principalName|String|Основное имя, если известно, субъекта.|
|type|Строка|Тип ресурса субъекта.|
|connectedOrganizationId|Строка|Идентификатор связанной организации субъекта.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|connectedOrganization|[connectedOrganization](connectedorganization.md)| Подключенная организация субъекта. Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON

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

