---
title: Тип ресурса connectedOrganization
description: В Azure AD управления правами подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e31f0bb97022863f3c575fcd0321297b3f68db64
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694906"
---
# <a name="connectedorganization-resource-type"></a>Тип ресурса connectedOrganization

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD управления правами](entitlementmanagement-overview.md) подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов connectedOrganization](../api/entitlementmanagement-list-connectedorganizations.md) | [коллекция connectedOrganization](connectedorganization.md) | Получение списка объектов connectedOrganization. |
|[Создание connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | Создайте объект connectedOrganization. |
|[Получение connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Чтение свойств и связей объекта connectedOrganization. |
|[Обновление connectedOrganization](../api/connectedorganization-update.md) | | Обновление connectedOrganization. |
|[Удаление connectedOrganization](../api/connectedorganization-delete.md) |Нет | Удаление connectedOrganization. |
|[Перечисление объектов internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка внутренних спонсоров connectedOrganization. |
|[Перечисление объектов externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка внешних спонсоров connectedOrganization. |
|[Добавление internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Нет | Добавьте пользователя или группу во внутренних спонсоров connectedOrganization. |
|[Добавление externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Нет | Добавьте пользователя или группу во внешних спонсоров connectedOrganization. |
|[Удаление internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Нет | Удалите пользователя или группу из внутренних спонсоров connectedOrganization. |
|[Удаление externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Нет | Удаление пользователя или группы из внешних спонсоров connectedOrganization. |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|String|Имя участника-пользователя, создавшего этот ресурс. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|description|Строка|Описание подключенной организации.|
|displayName|String|Отображаемое имя подключенной организации. Поддерживает `$filter` (`eq`).|
|id|String| Только для чтения.|
|modifiedBy|Строка|Имя участника-пользователя, который последним изменил этот ресурс. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|state|connectedOrganizationState|Состояние подключенной организации `AllConfiguredConnectedOrganizationSubjects` определяет, применимы ли политики назначения с типом области запроса. Возможные значения: `configured`, `proposed`.|
|identitySources|[Коллекция identitySource](identitySource.md)| Источники удостоверений в этой подключенной организации, один из [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [crossCloudAzureActiveDirectoryTenant](crosscloudazureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation](externaldomainfederation.md). Только для чтения. Допускается значение null. Поддерживает и `$select` `$filter`(`eq`). Чтобы выполнить фильтрацию по производным типам, необходимо объявить ресурс, используя полное приведение OData, `$filter=identitySources/any(is:is/microsoft.graph.azureActiveDirectoryTenant/tenantId eq 'bcfdfff4-cbc3-43f2-9000-ba7b7515054f')`например.|

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


