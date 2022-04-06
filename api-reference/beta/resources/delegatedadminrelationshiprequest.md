---
title: delegatedAdminRelationshipRequest resource type
description: Представляет запрос, определенный для делегирования отношений администратора между партнером и клиентом.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7381f4acf3ec04f4bdf4ef8f3a8bdf3744efa81d
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589797"
---
# <a name="delegatedadminrelationshiprequest-resource-type"></a>delegatedAdminRelationshipRequest resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос, определенный для делегирования отношений администратора между партнером и клиентом. Это позволяет администратору партнеров Майкрософт принимать меры по таким отношениям, как блокировка отношений для утверждения или прекращения отношений.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание делегированияAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Создание нового **объекта делегированияAdminRelationshipRequest** .|
|[Список делегированAdminRelationshipRequests](../api/delegatedadminrelationship-list-requests.md)|[delegatedAdminRelationshipRequest collection](delegatedadminrelationshiprequest.md)|Получите список объектов **делегированияAdminRelationshipRequest** и их свойств.|
|[Получить делегированиеAdminRelationshipRequest](../api/delegatedadminrelationshiprequest-get.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Ознакомьтесь с свойствами и отношениями объекта **delegatedAdminRelationshipRequest** .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|delegatedAdminRelationshipRequestAction|Действие, выполняемые в делегированной связи администратора.|
|createdDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и времени UTC, когда был создан запрос на связь. Только для чтения. |
|id|Строка|Уникальный идентификатор запроса на связь. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и время UTC, когда этот запрос отношения был изменен в последний раз. Только для чтения.|
|status|delegatedAdminRelationshipRequestStatus|Состояние запроса. Только для чтения. Допустимые значения: `created`, `pending`, `complete`, `failed`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipRequest",
  "id": "String (identifier)",
  "action": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

