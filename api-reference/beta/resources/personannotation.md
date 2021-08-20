---
title: тип ресурса personAnnotation
description: тип ресурса personAnnotation
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 49e7945b1ba07d7daedbd197b826148921f2f0227dd71b5780413a3b67b6c6be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197851"
---
# <a name="personannotation-resource-type"></a>тип ресурса personAnnotation

Пространство имен: microsoft.graph

Предоставляет сведения в заметках, которые пользователь связал с собой в различных службах и поделился с другими.

Наследует от [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Заметки списка](../api/profile-list-notes.md)|[коллекция personAnnotation](../resources/personannotation.md)|Получите ресурсы personAnnotation из свойства навигации примечаний.|
|[Создание personAnnotation](../api/profile-post-notes.md)|[personAnnotation](../resources/personannotation.md)|Создание нового объекта personAnnotation.|
|[Get personAnnotation](../api/personannotation-get.md)|[personAnnotation](../resources/personannotation.md)|Ознакомьтесь с свойствами и отношениями [объекта personAnnotation.](../resources/personannotation.md)|
|[Обновление personAnnotation](../api/personannotation-update.md)|[personAnnotation](../resources/personannotation.md)|Обновление свойств объекта [personAnnotation.](../resources/personannotation.md)|
|[Удаление personAnnotation](../api/personannotation-delete.md)|Нет|Удаляет объект [personAnnotation.](../resources/personannotation.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|Строка|Аудитории, которые могут видеть значения, содержащиеся в объекте. Унаследовано от [itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создав объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|подробные|[itemBody](../resources/itembody.md)|Содержит сведения о самой заметке.|
|displayName|Строка|Содержит удобное имя для заметки.|
|id|String|Идентификатор, используемый для индивидуального обращения к объекту. Унаследованный от [сущности](../resources/entity.md)|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или модифицируют приложение. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которые в последний раз изменили объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникли, если синхронизированы с другой службы. Унаследовано от [itemFacet](../resources/itemfacet.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAnnotation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnnotation",
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
  "detail": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "displayName": "String"
}
```


