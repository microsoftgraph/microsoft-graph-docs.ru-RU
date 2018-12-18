---
title: Тип ресурса managedEBookAssignment
description: Содержит свойства, используемые при назначении электронной книги группе.
author: tfitzmac
ms.openlocfilehash: d5b9d7a3d4574c2098dbe694eb208894c4262514
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362764"
---
# <a name="managedebookassignment-resource-type"></a>Тип ресурса managedEBookAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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



