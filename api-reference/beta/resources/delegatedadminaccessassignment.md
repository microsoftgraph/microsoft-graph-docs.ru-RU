---
title: тип ресурса delegatedAdminAccessAssignment
description: Представляет назначение административных ролей контейнеру доступа партнера Майкрософт.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: eec8597ffa629b919a7f9b7a9f9d22fbdcde2217
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589863"
---
# <a name="delegatedadminaccessassignment-resource-type"></a>тип ресурса delegatedAdminAccessAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначение административных ролей партнеру Майкрософт с помощью делегирования администрирования. Административные роли назначены партнеру Майкрософт через контейнер доступа (например, группу безопасности). Когда он активен, члены контейнера доступа получают доступ к ролям, указанным в сведениях о доступе.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание делегированияAdminAccessAssignment](../api/delegatedadminrelationship-post-accessassignments.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Создание нового **объекта делегированияAdminAccessAssignment** .|
|[Список делегированAdminAccessAssignments](../api/delegatedadminrelationship-list-accessassignments.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md) collection|Получите список объектов **делегированияAdminAccessAssignment** и их свойств.|
|[ДелегированиеAdminAccessAssignment](../api/delegatedadminaccessassignment-get.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Ознакомьтесь с свойствами и отношениями объекта **делегированияAdminAccessAssignment** .|
|[Обновление делегированияAdminAccessAssignment](../api/delegatedadminaccessassignment-update.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Обновление свойств объекта **делегированияAdminAccessAssignment** .|
|[Удаление делегированияAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md)|Нет|Удаление **объекта делегированияAdminAccessAssignment** .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessContainer|[delegatedAdminAccessContainer](../resources/delegatedadminaccesscontainer.md)|Контейнер доступа, через который участникам назначен доступ. Например, группа безопасности.|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Сведения о доступе, содержащие идентификаторы административных ролей, которые партнеру назначены в клиенте клиента.|
|createdDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и времени UTC, когда было создано назначение доступа. Только для чтения.|
|id|Строка|Уникальный идентификатор назначения доступа. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время в ISO 8601 и времени UTC, когда это назначение доступа было изменено в последний раз. Только для чтения.|
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

