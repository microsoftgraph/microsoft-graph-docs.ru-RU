---
title: Тип ресурса managedEBookAssignment
description: Содержит свойства, используемые при назначении электронной книги группе.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38c4ce911b913ec810746827ba14bc30a8564650
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086962"
---
# <a name="managedebookassignment-resource-type"></a>Тип ресурса managedEBookAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|id|String|Ключ объекта.|
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
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "installIntent": "String"
}
```



