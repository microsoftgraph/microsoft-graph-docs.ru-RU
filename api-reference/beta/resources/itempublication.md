---
title: тип ресурса itemPublication
description: тип ресурса itemPublication
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5cdc4a741205be696e584100d1ce6900052a951354481cc0dceffb7d1e19464b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248291"
---
# <a name="itempublication-resource-type"></a>тип ресурса itemPublication

Пространство имен: microsoft.graph

Представляет публикацию или статью, связанную с профилем [пользователя.](../resources/profile.md)

Наследует от [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Публикации списка](../api/profile-list-publications.md)|[коллекция itemPublication](../resources/itempublication.md)|Получите ресурсы itemPublication из свойства навигации публикаций.|
|[Создание itemPublication](../api/profile-post-publications.md)|[itemPublication](../resources/itempublication.md)|Создайте новый объект itemPublication.|
|[Get itemPublication](../api/itempublication-get.md)|[itemPublication](../resources/itempublication.md)|Ознакомьтесь с свойствами и отношениями [объекта itemPublication.](../resources/itempublication.md)|
|[Обновление itemPublication](../api/itempublication-update.md)|[itemPublication](../resources/itempublication.md)|Обновление свойств объекта [itemPublication.](../resources/itempublication.md)|
|[Удаление itemPublication](../api/itempublication-delete.md)|Нет|Удаляет объект [itemPublication.](../resources/itempublication.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|String|Аудитории, которые могут видеть значения, содержащиеся в объекте. Унаследовано от [itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создав объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|description    |Строка      |Описание публикации.                   |
|displayName    |String      |Название публикации.                         |
|id|Строка|Идентификатор, используемый для индивидуального обращения к объекту. Унаследованный от [сущности](../resources/entity.md)|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или модифицируют приложение. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которые в последний раз изменили объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|publishedDate  |Дата        |Дата публикации.      |
|publisher      |String      |Публикация или издатель для публикации.     |
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникли, если синхронизированы с другой службы. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|thumbnailUrl   |Строка      |URL-адрес, ссылающийся на эскиз публикации.   |
|webUrl         |String      |URL-адрес, ссылающийся на публикацию.                  |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPublication",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPublication",
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
  "publishedDate": "Date",
  "publisher": "String",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


