---
title: тип ресурса personAward
description: тип ресурса personAward
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4af72499276b6eb4e90333243462e94f0cfa02b92aa014cbcdc59e1a111d1afa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251052"
---
# <a name="personaward-resource-type"></a>тип ресурса personAward

Пространство имен: microsoft.graph

Представляет награду, связанную с профилем [пользователя.](../resources/profile.md)

Наследует от [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Награды списка](../api/profile-list-awards.md)|[коллекция personAward](../resources/personaward.md)|Получите ресурсы personAward из свойства навигации наград.|
|[Создание personAward](../api/profile-post-awards.md)|[personAward](../resources/personaward.md)|Создайте новый объект personAward.|
|[Get personAward](../api/personaward-get.md)|[personAward](../resources/personaward.md)|Ознакомьтесь с свойствами и отношениями [объекта personAward.](../resources/personaward.md)|
|[Обновление personAward](../api/personaward-update.md)|[personAward](../resources/personaward.md)|Обновление свойств объекта [personAward.](../resources/personaward.md)|
|[Удаление personAward](../api/personaward-delete.md)|Нет|Удаляет [объект personAward.](../resources/personaward.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|Строка|Аудитории, которые могут видеть значения, содержащиеся в объекте. Унаследовано от [itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создав объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|description|Строка|Descpription of the award or honor. |
|displayName|String|Имя награды или чести. |
|id|Строка|Идентификатор, используемый для индивидуального обращения к объекту. Унаследованный от [сущности](../resources/entity.md)|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или модифицируют приложение. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|issuedDate|Дата|Дата, в которую была предоставлена награда или честь. |
|issuingAuthority|Строка|Орган, который предоставил награду или честь.  |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которые в последний раз изменили объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникли, если синхронизированы с другой службы. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|thumbnailUrl|Строка|URL-адрес, ссылающийся на эскиз награды или чести.  |
|webUrl|String|URL-адрес, ссылающийся на награду или честь. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAward",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAward",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "description": "String",
  "displayName": "String",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


