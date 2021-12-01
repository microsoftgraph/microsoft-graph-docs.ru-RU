---
title: тип ресурса connectedOrganization
description: В управлении правами Azure AD подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 42ec49fd292f0e7c59002a57f7f4ccaff47c292d
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242883"
---
# <a name="connectedorganization-resource-type"></a>тип ресурса connectedOrganization

Пространство имен: microsoft.graph


В [управлении правами Azure AD](entitlementmanagement-root.md)подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Списки подключенныхОрганизацией](../api/entitlementmanagement-list-connectedorganizations.md)|[connectedOrganization](connectedorganization.md) collection|Извлечение списка объектов connectedOrganization. |
|[Создание connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md)|[connectedOrganization](connectedorganization.md)|Создание нового объекта connectedOrganization. |
|[ПодключениеОрганизация](../api/connectedorganization-get.md)|[connectedOrganization](connectedorganization.md)|Чтение свойств и связей объекта connectedOrganization. |
|[Обновление connectedOrganization](../api/connectedorganization-update.md)|[connectedOrganization](connectedorganization.md) collection|Обновление подключеннойорганизации. |
|[Удаление connectedOrganization](../api/connectedorganization-delete.md)|Нет|Удаление подключеннойорганизации. |
|[Список externalSponsors](../api/connectedorganization-list-externalsponsors.md)|Коллекция [directoryObject](directoryobject.md)|Извлечение списка внешних спонсоров connectedOrganization. |
|[Добавление externalSponsors](../api/connectedorganization-post-externalsponsors.md)|Нет|Добавьте пользователя или группу к внешним спонсорам connectedOrganization. |
|[Список internalSponsors](../api/connectedorganization-list-internalsponsors.md)|Коллекция [directoryObject](directoryobject.md)|Извлечение списка внутренних спонсоров connectedOrganization. |
|[Добавление internalSponsors](../api/connectedorganization-post-internalsponsors.md)|Нет|Добавьте пользователя или группу во внутренние спонсоры connectedOrganization. |
|[Удаление internalSponsors](../api/connectedorganization-delete-internalsponsors.md)|Нет|Удалите пользователя или группу из внутренних спонсоров connectedOrganization. |
|[Удаление externalSponsors](../api/connectedorganization-delete-externalsponsors.md)|Нет|Удалите пользователя или группу из внешних спонсоров connectedOrganization. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|description|Строка|Описание связанной организации.|
|displayName|Строка|Отображает имя подключенной организации.|
|id|String|Только для чтения.|
|identitySources|[коллекция identitySource](../resources/identitysource.md)|Источники удостоверений в этой связанной организации, один из [azureActiveDirectoryTenant,](azureactivedirectorytenant.md) [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation.](externaldomainfederation.md) Допускается значение null.|
|modifiedDateTime|DateTimeOffset|*Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|state|connectedOrganizationState|Состояние связанной организации определяет, применимы ли политики назначения с типом области `AllConfiguredConnectedOrganizationSubjects` запроса.  Допустимые значения: `configured`, `proposed`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|externalSponsors|Коллекция [directoryObject](directoryobject.md)|Допускается значение null.|
|internalSponsors|Коллекция [directoryObject](directoryobject.md)|Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectedOrganization",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant"
    }
  ],
  "state": "String"
}
```


