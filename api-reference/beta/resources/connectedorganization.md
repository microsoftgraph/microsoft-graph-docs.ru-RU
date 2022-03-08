---
title: тип ресурса connectedOrganization
description: В управлении правами Azure AD подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6e782def17541cbfe48923d788e8cbf774c1a473
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334102"
---
# <a name="connectedorganization-resource-type"></a>тип ресурса connectedOrganization

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-overview.md) подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Списки подключенныхОрганизацией](../api/entitlementmanagement-list-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) collection | Извлечение списка объектов connectedOrganization. |
|[Создание connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | Создание нового объекта connectedOrganization. |
|[ПодключениеОрганизация](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Чтение свойств и связей объекта connectedOrganization. |
|[Обновление connectedOrganization](../api/connectedorganization-update.md) | | Обновление подключеннойорганизации. |
|[Удаление connectedOrganization](../api/connectedorganization-delete.md) |Нет | Удаление подключеннойорганизации. |
|[Список internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Извлечение списка внутренних спонсоров connectedOrganization. |
|[Список externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Извлечение списка внешних спонсоров connectedOrganization. |
|[Добавление internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Нет | Добавьте пользователя или группу во внутренние спонсоры connectedOrganization. |
|[Добавление externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Нет | Добавьте пользователя или группу к внешним спонсорам connectedOrganization. |
|[Удаление internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Нет | Удалите пользователя или группу из внутренних спонсоров connectedOrganization. |
|[Удаление externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Нет | Удалите пользователя или группу из внешних спонсоров connectedOrganization. |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|String|UPN пользователя, создавшего этот ресурс. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|description|Строка|Описание связанной организации.|
|displayName|String|Отображает имя подключенной организации. Поддерживает `$filter` (`eq`).|
|id|String| Только для чтения.|
|modifiedBy|Строка|UPN пользователя, который в последний раз изменил этот ресурс. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|state|connectedOrganizationState|Состояние связанной организации определяет `AllConfiguredConnectedOrganizationSubjects` , применимы ли политики назначения с типом области запроса. Возможные значения: `configured`, `proposed`.|
|identitySources|[коллекция identitySource](identitySource.md)| Источники удостоверений в этой связанной организации, один из [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation](externaldomainfederation.md). Только для чтения. Допускается значение null. Поддерживает и `$select` `$filter`().`eq` Чтобы фильтровать полученные типы, необходимо объявить ресурс с использованием полного литья OData, `$filter=identitySources/any(is:is/microsoft.graph.azureActiveDirectoryTenant/tenantId eq 'bcfdfff4-cbc3-43f2-9000-ba7b7515054f')`например .|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|internalSponsors| Коллекция [directoryObject](directoryobject.md)| Допускается значение null.|
|externalSponsors| Коллекция [directoryObject](directoryobject.md)| Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "String (identifier)",
      "displayName": "String"
    }
  ],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


