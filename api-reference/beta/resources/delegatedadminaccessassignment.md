---
title: Тип ресурса delegatedAdminAccessAssignment
description: Представляет назначение административных ролей контейнеру доступа партнера Майкрософт.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: a9d831325d211233062d93ce1ccda1128d9dfb4b
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704340"
---
# <a name="delegatedadminaccessassignment-resource-type"></a>Тип ресурса delegatedAdminAccessAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначение административных ролей партнеру Майкрософт с помощью делегированного администрирования. Административные роли назначаются партнеру Майкрософт через контейнер доступа (например, группу безопасности). Когда он активен, члены контейнера доступа получают доступ к ролям, указанным в сведениях о доступе.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание delegatedAdminAccessAssignment](../api/delegatedadminrelationship-post-accessassignments.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Создайте новый **объект delegatedAdminAccessAssignment** .|
|[Перечисление delegatedAdminAccessAssignments](../api/delegatedadminrelationship-list-accessassignments.md)|[Коллекция delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Получение списка объектов **delegatedAdminAccessAssignment** и их свойств.|
|[Получение delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-get.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Чтение свойств и связей объекта **delegatedAdminAccessAssignment** .|
|[Обновление delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-update.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Обновление свойств объекта **delegatedAdminAccessAssignment** .|
|[Удаление delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md)|Нет|Удаление объекта **delegatedAdminAccessAssignment** .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessContainer|[delegatedAdminAccessContainer](../resources/delegatedadminaccesscontainer.md)|Контейнер доступа, через который членам назначается доступ. Например, группа безопасности.|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Сведения о доступе, содержащие идентификаторы административных ролей, назначенных партнеру в клиенте клиента.|
|createdDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и времени в формате UTC, когда было создано назначение доступа. Только для чтения.|
|id|String|Уникальный идентификатор назначения доступа. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время в ISO 8601 и времени в формате UTC, когда это назначение доступа было изменено в последний раз. Только для чтения.|
|status|delegatedAdminAccessAssignmentStatus|Состояние назначения доступа. Только для чтения. Допустимые значения: `pending`, `active`, `deleting`, `deleted`, `error`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminAccessAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminAccessAssignment",
  "id": "String (identifier)",
  "status": "String",
  "accessContainer": {
    "@odata.type": "microsoft.graph.delegatedAdminAccessContainer"
  },
  "accessDetails": {
    "@odata.type": "microsoft.graph.delegatedAdminAccessDetails"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

