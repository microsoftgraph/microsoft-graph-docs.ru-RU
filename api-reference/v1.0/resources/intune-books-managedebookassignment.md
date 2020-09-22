---
title: Тип ресурса managedEBookAssignment
description: Содержит свойства, используемые при назначении электронной книги группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a201472e394a08cf351e7eedc58489f305dda3a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088645"
---
# <a name="managedebookassignment-resource-type"></a>Тип ресурса managedEBookAssignment

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения электронной книги.|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|Цель установки электронной книги. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Связи
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









