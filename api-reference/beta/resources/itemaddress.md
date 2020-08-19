---
title: Тип ресурса Итемаддресс
description: Тип ресурса Итемаддресс
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ea99085ca04ea85b78a2fee1b80525ef934856a7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809766"
---
# <a name="itemaddress-resource-type"></a>Тип ресурса Итемаддресс

Пространство имен: microsoft.graph

Представляет физический адрес и сведения о расположении, в котором находится адрес.

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список адресов](../api/profile-list-addresses.md)|Коллекция [итемаддресс](../resources/itemaddress.md)|Получение ресурсов Итемаддресс из свойства навигации Addresses.|
|[Создание Итемаддресс](../api/profile-post-addresses.md)|[итемаддресс](../resources/itemaddress.md)|Создание нового объекта Итемаддресс.|
|[Получение Итемаддресс](../api/itemaddress-get.md)|[итемаддресс](../resources/itemaddress.md)|Чтение свойств и связей объекта [итемаддресс](../resources/itemaddress.md) .|
|[Обновление Итемаддресс](../api/itemaddress-update.md)|[итемаддресс](../resources/itemaddress.md)|Обновление свойств объекта [итемаддресс](../resources/itemaddress.md) .|
|[Удаление Итемаддресс](../api/itemaddress-delete.md)|Нет|Удаляет объект [итемаддресс](../resources/itemaddress.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|описаны|[physicalAddress](../resources/physicaladdress.md)|Сведения о самом адресе.|
|displayName|String|Понятное имя, назначенное пользователю для этого адреса. |
|geoCoordinates|[geoCoordinates](../resources/geocoordinates.md)|Геокоординаты адреса.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemAddress",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemAddress",
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
  "displayName": "String",
  "detail": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.geoCoordinates"
  }
}
```
