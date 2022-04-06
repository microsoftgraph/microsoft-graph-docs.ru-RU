---
title: тип ресурса delegatedAdminRelationship
description: Представляет сведения о делегированных административных привилегиях, которые партнер Майкрософт имеет в клиенте клиента.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f0bb9038773c965e54ce0695ff443b931df02cfd
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589803"
---
# <a name="delegatedadminrelationship-resource-type"></a>тип ресурса delegatedAdminRelationship

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет делегированную связь администратора между партнером и клиентом.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание делегированияAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|Создание нового **объекта делегированияAdminRelationship** .|
|[Список делегированAdminRelationships](../api/tenantrelationship-list-delegatedadminrelationships.md)|[delegatedAdminRelationship collection](delegatedadminrelationship.md)|Получите список объектов **делегированияAdminRelationship** и их свойств.|
|[ДелегированиеAdminRelationship](../api/delegatedadminrelationship-get.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|Ознакомьтесь с свойствами и отношениями объекта **делегированияAdminRelationship** .|
|[Обновление делегированияAdminRelationship](../api/delegatedadminrelationship-update.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|Обновление свойств объекта **делегированияAdminRelationship** .|
|[Удаление делегированияAdminRelationship](../api/delegatedadminrelationship-delete.md)|Нет|Удаление **объекта делегированияAdminRelationship** .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Сведения о доступе, содержащие идентификаторы административных ролей, запрашиваемого администратором-партнером в клиенте клиента.|
|activatedDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и времени UTC, когда отношения стали активными. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и времени UTC, когда была создана связь. Только для чтения.|
|клиент|[delegatedAdminRelationshipCustomerParticipant](../resources/delegatedadminrelationshipcustomerparticipant.md)|Имя отображения и уникальный идентификатор клиента отношения. Это настраивается партнером на момент создания отношений или системой после утверждения отношения клиентом. Клиент не может изменить его.|
|displayName|Строка|Отображает имя отношения, используемого для простоты идентификации. Должна быть уникальной для *всех* делегированных отношений администратора партнера. Это устанавливается партнером только в том случае, `created` если связь находится в состоянии и не может быть изменена клиентом.|
|duration|Длительность|Продолжительность отношений в формате ISO 8601. Должно быть значением между инклюзивным `P1D` `P2Y` . Это устанавливается партнером только в том случае, `created` если связь находится в состоянии и не может быть изменена клиентом.|
|endDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и времени UTC  `terminated`, когда состояние отношений изменяется либо .`expired` Вычисляется как `endDateTime = activatedDateTime + duration`. Только для чтения.|
|id|String|Уникальный идентификатор отношения. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и времени UTC, когда связь была изменена в последний раз. Только для чтения.|
|status|delegatedAdminRelationshipStatus|Состояние отношений. Только для чтения. Возможные значения: `activating`, , `approvalPending``active`, , `approved`, `created`, `expired`, `terminationRequested``expiring``terminated``terminating``unknownFutureValue`. Поддерживает `$orderBy`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|accessAssignments|[delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) collection|Назначения доступа, связанные с делегированием отношений администратора.|
|operations|[delegatedAdminRelationshipOperation](../resources/delegatedadminrelationshipoperation.md) collection|Длительные операции, связанные с делегированной связью администратора.|
|запросы|[delegatedAdminRelationshipRequest collection](../resources/delegatedadminrelationshiprequest.md)|Запросы, связанные с делегированием отношения администратора.|

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

