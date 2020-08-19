---
title: Тип ресурса Итемпатент
description: Тип ресурса Итемпатент
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4b8a5c72117e20a73fb3c3b6b8a2af308219b69d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809764"
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
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|description|String|Дескприптион патента или для хранения. |
|displayName|String|Название патента или его для архивации. |
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|Ожидается        |Логический     |Указывает, что патент находится в состоянии ожидания.        |
|иссуеддате       |Дата        |Дата предоставления патента.   |
|иссуингаусорити |String      |Центр сертификации, который предоставил патент.     |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|число           |String      |Номер патента.                      |
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|webUrl           |String      |URL-адрес, ссылающийся на патент или в систему архивации. |


## <a name="relationships"></a>Отношения
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
