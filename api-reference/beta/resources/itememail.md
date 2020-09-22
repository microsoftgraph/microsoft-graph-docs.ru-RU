---
title: Тип ресурса Итемемаил
description: Тип ресурса Итемемаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2dbf1f3f2c90cf7562d034e32f8fa03d1590ee42
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021485"
---
# <a name="itememail-resource-type"></a>Тип ресурса Итемемаил

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения об адресах электронной почты, связанных с пользователем.

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список сообщений электронной почты](../api/profile-list-emails.md)|Коллекция [итемемаил](../resources/itememail.md)|Получение ресурсов Итемемаил из свойства навигации по электронной почте.|
|[Создание Итемемаил](../api/profile-post-emails.md)|[итемемаил](../resources/itememail.md)|Создание нового объекта Итемемаил.|
|[Получение Итемемаил](../api/itememail-get.md)|[итемемаил](../resources/itememail.md)|Чтение свойств и связей объекта [итемемаил](../resources/itememail.md) .|
|[Обновление Итемемаил](../api/itememail-update.md)|[итемемаил](../resources/itememail.md)|Обновление свойств объекта [итемемаил](../resources/itememail.md) .|
|[Удаление Итемемаил](../api/itememail-delete.md)|Нет|Удаляет объект [итемемаил](../resources/itememail.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|address|String|Сам адрес электронной почты.|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|displayName|String|Имя или метка, с которыми пользователь связан с определенным адресом электронной почты.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|type|емаилтипе|Тип адреса электронной почты. Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemEmail",
  "id": "0f30bf5d-bf5d-0f30-5dbf-300f5dbf300f",
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
  "address": "String",
  "displayName": "String",
  "type": "String"
}
```


