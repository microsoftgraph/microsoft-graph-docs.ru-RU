---
title: Тип ресурса iosVppEBookAssignment
description: Содержит свойства, используемые при назначении электронной книги в формате VPP для iOS группе.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 49ddbf75f4e073f636857c4ba9c9fa7910c847f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399593"
---
# <a name="iosvppebookassignment-resource-type"></a>Тип ресурса iosVppEBookAssignment

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|Цель установки электронной книги. Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md). Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

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




