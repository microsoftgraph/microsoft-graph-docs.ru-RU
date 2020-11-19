---
title: Тип ресурса Девицеаппманажементтаск
description: Задача управления приложениями для устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51e8c7e057dc660e348dec17e8fa4e4704c7c202
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222522"
---
# <a name="deviceappmanagementtask-resource-type"></a>Тип ресурса Девицеаппманажементтаск

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Задача управления приложениями для устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеаппманажементтаскс](../api/intune-partnerintegration-deviceappmanagementtask-list.md)|Коллекция [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Список свойств и связей объектов [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[Получение Девицеаппманажементтаск](../api/intune-partnerintegration-deviceappmanagementtask-get.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Чтение свойств и связей объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[Создание Девицеаппманажементтаск](../api/intune-partnerintegration-deviceappmanagementtask-create.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Создание нового объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[Удаление Девицеаппманажементтаск](../api/intune-partnerintegration-deviceappmanagementtask-delete.md)|Нет|Удаляет объект [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md).|
|[Обновление Девицеаппманажементтаск](../api/intune-partnerintegration-deviceappmanagementtask-update.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Обновление свойств объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[действие updateStatus](../api/intune-partnerintegration-deviceappmanagementtask-updatestatus.md)|Нет|Задайте состояние задачи и вложите заметку.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Имя.|
|description|String|Описание.|
|createdDateTime|DateTimeOffset|Дата создания.|
|dueDateTime|DateTimeOffset|Дата выполнения.|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|Категория. Возможные значения: `unknown`, `advancedThreatProtection`.|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|Приоритет. Возможные значения: `none`, `high`, `low`.|
|creator|String|Адрес электронной почты создателя.|
|креаторнотес|String|Заметки автора.|
|assignedTo|String|Имя или электронная почта администратора, которому назначена эта задача.|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|Состояние. Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagementTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String"
}
```




