---
title: Тип ресурса Персонанниверсари
description: Тип ресурса Персонанниверсари
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9c6f979ae1bb0378b22b91494866f724c4fe6628
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997979"
---
# <a name="personanniversary-resource-type"></a>Тип ресурса Персонанниверсари

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о значимых датах, связанных с пользователем в [профиле](profile.md)пользователя.

Наследуется от [итемфацет](itemFacet.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список юбилеев](../api/profile-list-anniversaries.md)|Коллекция [персонанниверсари](../resources/personanniversary.md)|Получение ресурсов Персонанниверсари из свойства навигации юбилеев.|
|[Создание Персонанниверсари](../api/profile-post-anniversaries.md)|[персонанниверсари](../resources/personanniversary.md)|Создание нового объекта Персонанниверсари.|
|[Получение Персонанниверсари](../api/personanniversary-get.md)|[персонанниверсари](../resources/personanniversary.md)|Чтение свойств и связей объекта [персонанниверсари](../resources/personanniversary.md) .|
|[Обновление Персонанниверсари](../api/personanniversary-update.md)|[персонанниверсари](../resources/personanniversary.md)|Обновление свойств объекта [персонанниверсари](../resources/personanniversary.md) .|
|[Удаление Персонанниверсари](../api/personanniversary-delete.md)|Нет|Удаляет объект [персонанниверсари](../resources/personanniversary.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|date|Date|Содержит дату, связанную с типом юбилея.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|type|анниверсаритипе|Тип юбилея даты. Возможные значения: `birthday`, `wedding`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnniversary",
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
  "type": "String",
  "date": "Date"
}
```


