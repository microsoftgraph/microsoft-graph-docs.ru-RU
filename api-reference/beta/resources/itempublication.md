---
title: Тип ресурса Итемпубликатион
description: Тип ресурса Итемпубликатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 59b30c08e78db52af9e10c6aac2550dc02c11e62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084004"
---
# <a name="itempublication-resource-type"></a>Тип ресурса Итемпубликатион

Пространство имен: microsoft.graph

Представляет публикацию или статью, сопоставленные с [профилем](../resources/profile.md)пользователя.

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список публикаций](../api/profile-list-publications.md)|Коллекция [итемпубликатион](../resources/itempublication.md)|Получение ресурсов Итемпубликатион из свойства навигации публикации.|
|[Создание Итемпубликатион](../api/profile-post-publications.md)|[итемпубликатион](../resources/itempublication.md)|Создание нового объекта Итемпубликатион.|
|[Получение Итемпубликатион](../api/itempublication-get.md)|[итемпубликатион](../resources/itempublication.md)|Чтение свойств и связей объекта [итемпубликатион](../resources/itempublication.md) .|
|[Обновление Итемпубликатион](../api/itempublication-update.md)|[итемпубликатион](../resources/itempublication.md)|Обновление свойств объекта [итемпубликатион](../resources/itempublication.md) .|
|[Удаление Итемпубликатион](../api/itempublication-delete.md)|Нет|Удаляет объект [итемпубликатион](../resources/itempublication.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|Строка|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|description    |Строка      |Описание публикации.                   |
|displayName    |Строка      |Название публикации.                         |
|id|Строка|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|публишеддате  |Дата        |Дата публикации публикации.      |
|publisher      |String      |Публикация или издатель для публикации.     |
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
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


