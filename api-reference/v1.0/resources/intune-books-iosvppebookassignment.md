---
title: Тип ресурса iosVppEBookAssignment
description: Содержит свойства, используемые при назначении электронной книги в формате VPP для iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54686cd1fa860a37d5d1c6e48a664bf5b16612c84cf680365f65e56491903e55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54175233"
---
# <a name="iosvppebookassignment-resource-type"></a>Тип ресурса iosVppEBookAssignment

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые при назначении электронной книги в формате VPP для iOS группе.


Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-list.md)|Коллекция [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Список свойств и связей объектов [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|
|[Получение объекта iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-get.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Чтение свойств и связей объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|
|[Создание объекта iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-create.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|
|[Удаление объекта iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-delete.md)|Нет|Удаляет объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|
|[Обновление объекта iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-update.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Обновление свойств объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения электронной книги. Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|Цель установки электронной книги. Унаследованный от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md). Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```




