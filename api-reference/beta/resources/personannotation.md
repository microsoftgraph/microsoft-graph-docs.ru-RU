---
title: Тип ресурса Персонаннотатион
description: Тип ресурса Персонаннотатион
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 403df171498bcde62d113ce2a2f2a27cf3987285
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997972"
---
# <a name="personannotation-resource-type"></a>Тип ресурса Персонаннотатион

Пространство имен: microsoft.graph

Предоставляет сведения в примечаниях, которые пользователь связал с собственными службами в различных службах и совместно используется совместно с другими пользователями.

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список заметок](../api/profile-list-notes.md)|Коллекция [персонаннотатион](../resources/personannotation.md)|Получение ресурсов Персонаннотатион из свойства навигации Notes.|
|[Создание Персонаннотатион](../api/profile-post-notes.md)|[персонаннотатион](../resources/personannotation.md)|Создание нового объекта Персонаннотатион.|
|[Получение Персонаннотатион](../api/personannotation-get.md)|[персонаннотатион](../resources/personannotation.md)|Чтение свойств и связей объекта [персонаннотатион](../resources/personannotation.md) .|
|[Обновление Персонаннотатион](../api/personannotation-update.md)|[персонаннотатион](../resources/personannotation.md)|Обновление свойств объекта [персонаннотатион](../resources/personannotation.md) .|
|[Удаление Персонаннотатион](../api/personannotation-delete.md)|Нет|Удаляет объект [персонаннотатион](../resources/personannotation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|описаны|[itemBody](../resources/itembody.md)|Содержит подробные сведения о самом заметке.|
|displayName|String|Содержит понятное имя для заметки.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAnnotation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnnotation",
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
  "detail": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "displayName": "String"
}
```


