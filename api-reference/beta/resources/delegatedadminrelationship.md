---
title: Тип ресурса delegatedAdminRelationship
description: Представляет сведения о делегированных административных привилегиях, которые партнер Майкрософт имеет в клиенте клиента.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 753212cabaf62f8bbfc5e119f3322b797d6559f8
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820632"
---
# <a name="delegatedadminrelationship-resource-type"></a>Тип ресурса delegatedAdminRelationship

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет делегированное отношение администратора между партнером и клиентом.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание delegatedAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|Создайте новый **объект delegatedAdminRelationship** .|
|[Перечисление объектов delegatedAdminRelationship](../api/tenantrelationship-list-delegatedadminrelationships.md)|[Коллекция delegatedAdminRelationship](delegatedadminrelationship.md)|Получение списка объектов **delegatedAdminRelationship** и их свойств.|
|[Получение delegatedAdminRelationship](../api/delegatedadminrelationship-get.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|Чтение свойств и связей объекта **delegatedAdminRelationship** .|
|[Обновление delegatedAdminRelationship](../api/delegatedadminrelationship-update.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|Обновление свойств объекта **delegatedAdminRelationship** .|
|[Удаление delegatedAdminRelationship](../api/delegatedadminrelationship-delete.md)|Нет|Удаление объекта **delegatedAdminRelationship** .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Сведения о доступе, содержащие идентификаторы административных ролей, запрашиваемых администратором партнера в клиенте клиента.|
|activatedDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и времени в формате UTC, когда связь стала активной. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и время создания связи в формате UTC. Только для чтения.|
|Клиентов|[delegatedAdminRelationshipCustomerParticipant](../resources/delegatedadminrelationshipcustomerparticipant.md)|Отображаемое имя и уникальный идентификатор клиента связи. Он настраивается либо партнером во время создания отношения, либо системой после того, как клиент утвердит связь. Не может быть изменен клиентом.|
|displayName|Строка|Отображаемое имя связи, используемой для упрощения идентификации. Должен быть уникальным для *всех делегированных* отношений администратора партнера. Этот параметр задается партнером только в том случае `created` , если связь находится в состоянии и не может быть изменена клиентом.|
|duration|Длительность|Длительность связи в формате ISO 8601. Должно быть значением между инклюзивным `P1D` `P2Y` . Этот параметр задается партнером только в том случае `created` , если связь находится в состоянии и не может быть изменена клиентом.|
|endDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и времени в формате UTC,  когда состояние связи изменяется на любой `terminated` `expired`или . Вычисляется как `endDateTime = activatedDateTime + duration`. Только для чтения.|
|id|Строка|Уникальный идентификатор связи. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и время последнего изменения связи в формате UTC. Только для чтения.|
|status|delegatedAdminRelationshipStatus|Состояние связи. Только для чтения. Возможные значения: `activating`, , `active`, `approvalPending`, `approved`, `created`, `expiring``expired`, `terminated`, . `unknownFutureValue``terminating``terminationRequested` Поддерживает `$orderBy`.|

### <a name="delegatedadminrelationshipstatus-values"></a>Значения delegatedAdminRelationshipStatus 
| Member | Описание |
| --- | --- |
| создано | Партнер создал новую связь. В этом состоянии связь может быть изменена. |
| approvalPending | Партнер завершил связь с помощью действия `lockForApproval` делегированного [объекта DelegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md) . |
| Утвержденных | Клиент утверждает связь с помощью действия `approve` объекта [delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md) . |
| Активация | Система начинает подготовку связи. |
| Активных | Система завершает подготовку связи. |
| Истекает | Срок действия связи истек. |
| Истек | Система завершает отмену подготовки связи. |
| terminationRequested | Партнер или клиент запрашивает `terminate` прекращение связи с помощью действия делегированного объекта [delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md) . |
| Прекращения | Система начинает отмену подготовки связи. |
| Прекращено | Система завершила отмену подготовки связи. |
| unknownFutureValue | Значение sentinel для развиваемого перечисления. Не следует использовать. |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|accessAssignments|[Коллекция delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md)|Назначения доступа, связанные с делегированным отношением администратора.|
|operations|[Коллекция delegatedAdminRelationshipOperation](../resources/delegatedadminrelationshipoperation.md)|Длительные операции, связанные с делегированным отношением администратора.|
|Запросы|[Коллекция delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md)|Запросы, связанные с делегированным отношением администратора.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminRelationship",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
  "id": "String (identifier)",
  "displayName": "String",
  "duration": "String",
  "customer": {
    "@odata.type": "microsoft.graph.delegatedAdminRelationshipCustomerParticipant"
  },
  "accessDetails": {
    "@odata.type": "microsoft.graph.delegatedAdminAccessDetails"
  },
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "activatedDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

