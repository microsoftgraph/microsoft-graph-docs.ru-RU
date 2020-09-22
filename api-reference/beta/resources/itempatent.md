---
title: Тип ресурса Итемпатент
description: Тип ресурса Итемпатент
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7e6732a53f841902422348f90dada22174813b39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089292"
---
# <a name="itempatent-resource-type"></a>Тип ресурса Итемпатент
 
Пространство имен: microsoft.graph

Представляет предоставленный или архивированный патент, который был добавлен в [профиль](../resources/profile.md)пользователя.

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список патентов](../api/profile-list-patents.md)|Коллекция [итемпатент](../resources/itempatent.md)|Получите ресурсы Итемпатент в свойстве навигации для патентов.|
|[Создание Итемпатент](../api/profile-post-patents.md)|[итемпатент](../resources/itempatent.md)|Создание нового объекта Итемпатент.|
|[Получение Итемпатент](../api/itempatent-get.md)|[итемпатент](../resources/itempatent.md)|Чтение свойств и связей объекта [итемпатент](../resources/itempatent.md) .|
|[Обновление Итемпатент](../api/itempatent-update.md)|[итемпатент](../resources/itempatent.md)|Обновление свойств объекта [итемпатент](../resources/itempatent.md) .|
|[Удаление Итемпатент](../api/itempatent-delete.md)|Нет|Удаляет объект [итемпатент](../resources/itempatent.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|Строка|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|description|Строка|Дескприптион патента или для хранения. |
|displayName|Строка|Название патента или его для архивации. |
|id|Строка|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|Ожидается        |Boolean     |Указывает, что патент находится в состоянии ожидания.        |
|иссуеддате       |Дата        |Дата предоставления патента.   |
|иссуингаусорити |Строка      |Центр сертификации, который предоставил патент.     |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|число           |Строка      |Номер патента.                      |
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|webUrl           |String      |URL-адрес, ссылающийся на патент или в систему архивации. |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPatent",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPatent",
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
  "isPending": "Boolean",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "number": "String",
  "webUrl": "String"
}
```


