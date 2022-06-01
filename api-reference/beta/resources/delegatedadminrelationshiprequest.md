---
title: Тип ресурса delegatedAdminRelationshipRequest
description: Представляет запрос, относящийся к отношениям делегированного администратора между партнером и клиентом.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 5aaaabed54e6f5a4f0ba21cbdf64fb7d9deb0e8f
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821185"
---
# <a name="delegatedadminrelationshiprequest-resource-type"></a>Тип ресурса delegatedAdminRelationshipRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос, относящийся к отношениям делегированного администратора между партнером и клиентом. Это позволяет администратору партнера Майкрософт выполнять действия в отношении таких отношений, как блокировка связи для утверждения или прерывание связи.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание delegatedAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Создайте новый **объект delegatedAdminRelationshipRequest** .|
|[Перечисление delegatedAdminRelationshipRequests](../api/delegatedadminrelationship-list-requests.md)|[Коллекция delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Получение списка объектов **delegatedAdminRelationshipRequest** и их свойств.|
|[Получение delegatedAdminRelationshipRequest](../api/delegatedadminrelationshiprequest-get.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Чтение свойств и связей объекта **delegatedAdminRelationshipRequest** .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|delegatedAdminRelationshipRequestAction|Действие, выполняемые с делегированным отношением администратора.|
|createdDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и время создания запроса связи в формате UTC. Только для чтения. |
|id|Строка|Уникальный идентификатор запроса связи. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения этого запроса связи в формате ISO 8601 и время в формате UTC. Только для чтения.|
|status|delegatedAdminRelationshipRequestStatus|Состояние запроса. Только для чтения. Допустимые значения: `created`, `pending`, `succeeded`, `failed`, `unknownFutureValue`.|

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

