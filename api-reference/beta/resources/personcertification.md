---
title: тип ресурса personCertification
description: тип ресурса personCertification
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 893856a5a8322cc82023572ebc2539a5ee91a112c5cc5455c9fd5ebea6bd2e89
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206041"
---
# <a name="personcertification-resource-type"></a>тип ресурса personCertification

Пространство имен: microsoft.graph

Представляет сертификацию или обозначение, связанное с профилем [пользователя.](../resources/profile.md)

Наследует от [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Сертификации списков](../api/profile-list-certifications.md)|[коллекция personCertification](../resources/personcertification.md)|Получите ресурсы personCertification из свойства навигации сертификации.|
|[Создание personCertification](../api/profile-post-certifications.md)|[personCertification](../resources/personcertification.md)|Создайте новый объект personCertification.|
|[Get personCertification](../api/personCertification-get.md)|[personCertification](../resources/personcertification.md)|Ознакомьтесь с свойствами и отношениями [объекта personCertification.](../resources/personcertification.md)|
|[Обновление personCertification](../api/personCertification-update.md)|[personCertification](../resources/personcertification.md)|Обновление свойств объекта [personCertification.](../resources/personcertification.md)|
|[Удаление personCertification](../api/personCertification-delete.md)|Нет|Удаляет объект [personCertification.](../resources/personcertification.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|String|Аудитории, которые могут видеть значения, содержащиеся в объекте. Унаследовано от [itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|certificationId  |String      |Справочный идентификатор для сертификации. |
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создав объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|description      |Строка      |Описание сертификации.                   |
|displayName      |String      |Название сертификата.                         |
|endDate          |Date        |Дата истечения срока сертификации.            |
|id|Строка|Идентификатор, используемый для индивидуального обращения к объекту. Унаследованный от [сущности](../resources/entity.md)|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или модифицируют приложение. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|issuedDate       |Дата        |Дата выдачи сертификата.         |
|issuingAuthority |Строка      |Орган, который предоставил сертификацию.          |
|issuingCompany   |Строка      |Компания, которая предоставила сертификацию.          |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которые в последний раз изменили объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникли, если синхронизированы с другой службы. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|startDate        |Date        |Дата, когда сертификация стала допустимой.       |
|thumbnailUrl     |String      |URL-адрес, ссылающийся на эскиз сертификата.   |
|webUrl           |String      |URL-адрес, ссылающийся на сертификацию.                  |

## <a name="relationships"></a>Связи
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


