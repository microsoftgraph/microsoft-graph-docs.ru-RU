---
title: Тип ресурса Персонцертификатион
description: Тип ресурса Персонцертификатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ef4ebe3bc870bafd0edf6a5315589c8f823286df
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46813149"
---
# <a name="personcertification-resource-type"></a>Тип ресурса Персонцертификатион

Пространство имен: microsoft.graph

Представляет сертификат или обозначение, сопоставленные с [профилем](../resources/profile.md)пользователя.

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список сертификатов](../api/profile-list-certifications.md)|Коллекция [персонцертификатион](../resources/personcertification.md)|Получите ресурсы Персонцертификатион в свойстве навигации сертификации.|
|[Создание Персонцертификатион](../api/profile-post-certifications.md)|[персонцертификатион](../resources/personcertification.md)|Создание нового объекта Персонцертификатион.|
|[Получение Персонцертификатион](../api/personCertification-get.md)|[персонцертификатион](../resources/personcertification.md)|Чтение свойств и связей объекта [персонцертификатион](../resources/personcertification.md) .|
|[Обновление Персонцертификатион](../api/personCertification-update.md)|[персонцертификатион](../resources/personcertification.md)|Обновление свойств объекта [персонцертификатион](../resources/personcertification.md) .|
|[Удаление Персонцертификатион](../api/personCertification-delete.md)|Нет|Удаляет объект [персонцертификатион](../resources/personcertification.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|цертификатионид  |String      |Справочный идентификатор для сертификации. |
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|description      |String      |Описание сертификата.                   |
|displayName      |String      |Название сертификата.                         |
|endDate          |Date        |Дата истечения срока действия сертификата.            |
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|иссуеддате       |Дата        |Дата выдачи сертификата.         |
|иссуингаусорити |String      |Центр сертификации, который предоставил сертификат.          |
|иссуингкомпани   |String      |Компания, которой назначена эта сертификация.          |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|startDate        |Date        |Дата, когда сертификация стала действительна.       |
|thumbnailUrl     |String      |URL-адрес, ссылающийся на эскиз сертификата.   |
|webUrl           |String      |URL-адрес, ссылающийся на сертификат.                  |

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personCertification",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personCertification",
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
  "certificationId": "String",
  "description": "String",
  "displayName": "String",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "issuingCompany": "String",
  "startDate": "Date",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```
