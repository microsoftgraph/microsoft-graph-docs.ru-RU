---
title: Тип ресурса Едукатионалактивити
description: Тип ресурса Едукатионалактивити
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5f920b2afbb319af923212563aac6e8ea163c9de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055682"
---
# <a name="educationalactivity-resource-type"></a>Тип ресурса Едукатионалактивити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные, которые пользователь предоставил, относящихся к выпуску, выпускнику, выпуску или другим учебным действиям.

Наследует свойства метаданных от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Едукатионалактивитиес](../api/profile-list-educationalactivities.md)|Коллекция [едукатионалактивити](../resources/educationalactivity.md)|Получение ресурсов Едукатионалактивити из свойства навигации Едукатионалактивитиес.|
|[Создание Едукатионалактивити ](../api/profile-post-educationalactivities.md)|[едукатионалактивити](../resources/educationalactivity.md)|Создание нового объекта Едукатионалактивити.|
|[Получение Едукатионалактивити](../api/educationalactivity-get.md)|[едукатионалактивити](../resources/educationalactivity.md)|Чтение свойств и связей объекта [едукатионалактивити](../resources/educationalactivity.md) .|
|[Обновление Едукатионалактивити](../api/educationalactivity-update.md)|[едукатионалактивити](../resources/educationalactivity.md)|Обновление свойств объекта [едукатионалактивити](../resources/educationalactivity.md) .|
|[Удаление Едукатионалактивити](../api/educationalactivity-delete.md)|Нет|Удаляет объект [едукатионалактивити](../resources/educationalactivity.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|комплетионмонсеар|Дата|Месяц и год, когда пользователь выполнит или выполнил действие. |
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|ендмонсеар|Дата|Месяц и год, когда пользователь завершил действие учебного заведения.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|Организация|[институтиондата](../resources/institutiondata.md)|Содержит подробные сведения о учебном заведения. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|Программа|[едукатионалактивитидетаил](../resources/educationalactivitydetail.md)|Содержит расширенные сведения о программе или курсе.|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|стартмонсеар|Дата|Месяц и год, когда пользователь присвоено указанному действию.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationalActivity",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationalActivity",
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
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "@odata.type": "microsoft.graph.institutionData"
  },
  "program": {
    "@odata.type": "microsoft.graph.educationalActivityDetail"
  },
  "startMonthYear": "Date"
}
```

