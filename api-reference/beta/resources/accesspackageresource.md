---
title: Тип ресурса accessPackageResource
description: Ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом, роли которого можно использовать в одном или более пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 31499fda1d2d12f1e9868da6cf9e09fde38298cd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137475"
---
# <a name="accesspackageresource-resource-type"></a>Тип ресурса accessPackageResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [azure AD Entitlement Management](entitlementmanagement-root.md)ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом пакетов доступа. Роли для ресурса пакета доступа можно использовать в одном или более пакетах доступа.  Чтобы запросить связывание ресурса с каталогом пакетов доступа или удалить ресурс из каталога, создайте [accessPackageResourceRequest.](accesspackageresourcerequest.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список ресурсов accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Коллекция accessPackageResource](accesspackageresource.md) | Получить список объектов accessPackageResource в каталоге. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Содержит сведения о среде для ресурса. Это можно настроить с помощью `@odata.bind` аннотации или источника *среды.*|
|addedBy|String|Только для чтения.|
|addedOn|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|description|Строка|Описание ресурса.|
|displayName|Строка|Отображаемого имени ресурса, например имя приложения, имя группы или имя сайта.|
|id|String| Только для чтения.|
|isPendingOnboarding|Boolean|Имеет true, если ресурс еще не доступен для назначения.|
|originId|Строка|Уникальный идентификатор ресурса в системе источника. В случае группы Azure AD это идентификатор группы. |
|originSystem|Строка|Тип ресурса в системе источника, например `SharePointOnline` , или `AadApplication` `AadGroup` .|
|resourceType|Строка|Тип ресурса, например, подключенное к Azure AD приложение `Application` или сайт `SharePoint Online Site` SharePoint Online.|
|url|String|Уникальный локатор ресурса, например URL-адрес для регистрации пользователя в приложении.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](accesspackageresourceenvironment.md)| Допускается значение null.|
|accessPackageResourceRoles|[Коллекция accessPackageResourceRole](accesspackageresourcerole.md)| Только для чтения. Допускается значение null.|
|accessPackageResourceScopes|[Коллекция accessPackageResourceScope](accesspackageresourcescope.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "baseType": "",
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
