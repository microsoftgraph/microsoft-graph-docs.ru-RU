---
title: Тип ресурса managedEBookAssignment
description: Содержит свойства, используемые при назначении электронной книги группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e2ba3dae32e24864a63dc650ac1fc50ae1bdaea9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028800"
---
# <a name="managedebookassignment-resource-type"></a>Тип ресурса managedEBookAssignment

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые при назначении электронной книги группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedEBookAssignment](../api/intune-books-managedebookassignment-list.md)|Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Список свойств и связей объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|[Получение объекта managedEBookAssignment](../api/intune-books-managedebookassignment-get.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Чтение свойств и связей объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|[Создание объекта managedEBookAssignment](../api/intune-books-managedebookassignment-create.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Создание объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|[Удаление объекта managedEBookAssignment](../api/intune-books-managedebookassignment-delete.md)|Нет|Удаляет объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|[Обновление объекта managedEBookAssignment](../api/intune-books-managedebookassignment-update.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Обновление свойств объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения электронной книги.|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|Цель установки электронной книги. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```



