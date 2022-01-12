---
title: тип ресурса accessPackageResource
description: Ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом ролей, которые можно использовать в одном или более пакетах доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 01c37923f3ca63b7dd7ccf6803bb2bc696ef4546
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792143"
---
# <a name="accesspackageresource-resource-type"></a>тип ресурса accessPackageResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-overview.md)ресурс пакета доступа является ссылкой на ресурс, связанный с каталогом пакетов доступа. Роли для ресурса пакета доступа можно использовать в одном или более пакетах доступа.  Чтобы попросить связать ресурс с каталогом пакетов доступа или удалить его из каталога, создайте [accessPackageResourceRequest](accesspackageresourcerequest.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Ресурсы accessPackageCatalog списка](../api/accesspackagecatalog-list-accesspackageresources.md) | [коллекция accessPackageResource](accesspackageresource.md) | Извлечение списка объектов accessPackageResource в каталоге. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Содержит сведения об среде для ресурса. Это можно установить с помощью `@odata.bind` аннотации или *originId среды.*|
|attributes|[коллекция accessPackageResourceAttribute](../resources/accesspackageresourceattribute.md)| Содержит сведения о атрибутах для ресурса.
|addedBy|String|Только для чтения.|
|addedOn|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
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
  "attributes": [
    {
      "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
    }
   ],
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
