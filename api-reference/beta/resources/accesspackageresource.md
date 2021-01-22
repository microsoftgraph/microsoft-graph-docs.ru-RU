---
title: Тип ресурса accessPackageResource
description: Ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом, роли которого можно использовать в одном или более пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e34b850b19836eeb19cc63232c7af822512bfee4
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934830"
---
# <a name="accesspackageresource-resource-type"></a>Тип ресурса accessPackageResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-root.md)ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом пакетов доступа, роли для которого можно использовать в одном или более пакетах доступа.  Чтобы запросить связывание ресурса с каталогом пакетов доступа или удалить ресурс из каталога, создайте [accessPackageResourceRequest.](accesspackageresourcerequest.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список ресурсов accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Коллекция accessPackageResource](accesspackageresource.md) | Получить список объектов accessPackageResource в каталоге. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|addedBy|String|Только для чтения.|
|addedOn|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|description|String|Описание ресурса.|
|displayName|String|Отображаемого имени ресурса, например имя приложения, имя группы или имя сайта.|
|id|String| Только для чтения.|
|isPendingOnboarding|Boolean|Имеет true, если ресурс еще не доступен для назначения.|
|originId|String|Уникальный идентификатор ресурса в системе источника. В случае группы Azure AD это идентификатор группы. |
|originSystem|String|Тип ресурса в системе источника, например `SharePointOnline` , или `AadApplication` `AadGroup` .|
|resourceType|String|Тип ресурса, например, подключенное к Azure AD приложение `Application` или сайт `SharePoint Online Site` SharePoint Online.|
|url|String|Уникальный локатор ресурса, например URL-адрес для регистрации пользователя в приложении.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
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


