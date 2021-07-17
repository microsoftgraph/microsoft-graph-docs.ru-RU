---
title: тип ресурса accessPackageResource
description: Ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом ролей, которые можно использовать в одном или более пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 14bbbe23fca77f8fef06a2cb546cd0b1fdcc1949
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467115"
---
# <a name="accesspackageresource-resource-type"></a>тип ресурса accessPackageResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-root.md)ресурс пакета доступа является ссылкой на ресурс, связанный с каталогом пакетов доступа. Роли для ресурса пакета доступа можно использовать в одном или более пакетах доступа.  Чтобы попросить связать ресурс с каталогом пакетов доступа или удалить его из каталога, создайте [accessPackageResourceRequest](accesspackageresourcerequest.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Ресурсы accessPackageCatalog списка](../api/accesspackagecatalog-list-accesspackageresources.md) | [коллекция accessPackageResource](accesspackageresource.md) | Извлечение списка объектов accessPackageResource в каталоге. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Содержит сведения об среде для ресурса. Это можно установить с помощью `@odata.bind` аннотации или *originId среды.*|
|addedBy|String|Только для чтения.|
|addedOn|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|description|String|Описание ресурса.|
|displayName|String|Отображает имя ресурса, например имя приложения, имя группы или имя сайта.|
|id|String| Только для чтения.|
|isPendingOnboarding|Логический|True, если ресурс еще не доступен для назначения.|
|OriginId|String|Уникальный идентификатор ресурса в системе происхождения. В случае группы Azure AD это идентификатор группы. |
|originSystem|String|Тип ресурса в системе происхождения, например `SharePointOnline` , `AadApplication` или `AadGroup` .|
|resourceType|String|Тип ресурса, например, подключенное приложение `Application` Azure AD или веб-SharePoint `SharePoint Online Site` Online.|
|url|String|Уникальный локатор ресурсов для ресурса, например URL-адрес для подписания пользователя в приложение.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](accesspackageresourceenvironment.md)| Допускается значение null. Поддерживает `$expand`.|
|accessPackageResourceRoles|[коллекция accessPackageResourceRole](accesspackageresourcerole.md)| Только для чтения. Допускается значение null. Поддерживает `$expand`.|
|accessPackageResourceScopes|[коллекция accessPackageResourceScope](accesspackageresourcescope.md)| Только для чтения. Допускается значение null. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "keyProperty": "id"
}-->

```json
{
  "addedBy": "String",
  "addedOn": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isPendingOnboarding": true,
  "originId": "String",
  "originSystem": "String",
  "resourceType": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
