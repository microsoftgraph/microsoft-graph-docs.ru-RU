---
title: Тип ресурса Персонреспонсибилити
description: Тип ресурса Персонреспонсибилити
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a8124a379bd6195a71ad3377edf19e49d85edf9c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809760"
---
# <a name="personresponsibility-resource-type"></a>Тип ресурса Персонреспонсибилити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет подробные сведения о обязанностях, связанных с самим пользователем в различных службах.

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список обязанностей](../api/profile-list-responsibilities.md)|Коллекция [персонреспонсибилити](../resources/personresponsibility.md)|Получение ресурсов Персонреспонсибилити из свойства навигации "обязанности".|
|[Создание Персонреспонсибилити](../api/profile-post-responsibilities.md)|[персонреспонсибилити](../resources/personresponsibility.md)|Создание нового объекта Персонреспонсибилити.|
|[Получение Персонреспонсибилити](../api/personresponsibility-get.md)|[персонреспонсибилити](../resources/personresponsibility.md)|Чтение свойств и связей объекта [персонреспонсибилити](../resources/personresponsibility.md) .|
|[Обновление Персонреспонсибилити](../api/personresponsibility-update.md)|[персонреспонсибилити](../resources/personresponsibility.md)|Обновление свойств объекта [персонреспонсибилити](../resources/personresponsibility.md) .|
|[Удаление Персонреспонсибилити](../api/personresponsibility-delete.md)|Нет|Удаляет объект [персонреспонсибилити](../resources/personresponsibility.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|коллаборатионтагс|Коллекция String|Содержит теги сценариев, с которыми пользователь связан с интересом. Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|description|String|Описание ответственности.|
|displayName|String|Содержит понятное имя для ответственности. |
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|webUrl|String|Содержит ссылку на веб-страницу или ресурс, отвечающие за ответственность.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personResponsibility",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personResponsibility",
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
  "webUrl": "String",
  "collaborationTags": [
    "String"
  ]
}
```
