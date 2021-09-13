---
title: тип ресурса itemPatent
description: тип ресурса itemPatent
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a6e53816f9e239de0f1c928763d1e329cc8cb63f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063624"
---
# <a name="itempatent-resource-type"></a>тип ресурса itemPatent
 
Пространство имен: microsoft.graph

Представляет предоставленный или подаренный патент, который был добавлен в профиль [пользователя.](../resources/profile.md)

Наследует от [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Патенты списка](../api/profile-list-patents.md)|[коллекция itemPatent](../resources/itempatent.md)|Получите ресурсы itemPatent из свойства навигации патентов.|
|[Создание itemPatent](../api/profile-post-patents.md)|[itemPatent](../resources/itempatent.md)|Создание нового объекта itemPatent.|
|[Получить itemPatent](../api/itempatent-get.md)|[itemPatent](../resources/itempatent.md)|Ознакомьтесь с свойствами и отношениями объекта [itemPatent.](../resources/itempatent.md)|
|[Обновление itemPatent](../api/itempatent-update.md)|[itemPatent](../resources/itempatent.md)|Обновление свойств объекта [itemPatent.](../resources/itempatent.md)|
|[Удаление itemPatent](../api/itempatent-delete.md)|Нет|Удаляет объект [itemPatent.](../resources/itempatent.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|String|Аудитории, которые могут видеть значения, содержащиеся в объекте. Унаследовано от [itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создав объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|description|Строка|Descpription патента или подачи. |
|displayName|String|Название патента или подачи. |
|id|Строка|Идентификатор, используемый для индивидуального обращения к объекту. Унаследованный от [сущности](../resources/entity.md)|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или модифицируют приложение. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|isPending        |Boolean     |Указывает, что патент находится в стадии ожидания.        |
|issuedDate       |Дата        |Дата предоставления патента.   |
|issuingAuthority |String      |Орган, выдав патент.     |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которые в последний раз изменили объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|число           |Строка      |Номер патента.                      |
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникли, если синхронизированы с другой службы. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|webUrl           |String      |URL-адрес, ссылающийся на патент или подачу. |


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


