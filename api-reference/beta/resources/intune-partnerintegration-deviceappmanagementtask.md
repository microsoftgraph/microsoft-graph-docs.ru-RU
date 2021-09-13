---
title: тип ресурса deviceAppManagementTask
description: Задача управления приложениями для устройств.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aaa21f40405bcbe2524854537f3e78a93e8dfb0c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101081"
---
# <a name="deviceappmanagementtask-resource-type"></a>тип ресурса deviceAppManagementTask

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Задача управления приложениями для устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List deviceAppManagementTasks](../api/intune-partnerintegration-deviceappmanagementtask-list.md)|[коллекция deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Список свойств и связей [объектов deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|[Get deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-get.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Чтение свойств и связей [объекта deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|[Создание deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-create.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Создание нового [объекта deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|[Удаление устройстваAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-delete.md)|Нет|Удаляет [устройствоAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).|
|[Обновление устройстваAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-update.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Обновление свойств объекта [deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|[действие updateStatus](../api/intune-partnerintegration-deviceappmanagementtask-updatestatus.md)|Нет|Установите состояние задачи и приложите примечание.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности.|
|displayName|String|Имя.|
|description|String|Описание.|
|createdDateTime|DateTimeOffset|Дата создания.|
|dueDateTime|DateTimeOffset|Срок действия.|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|Категория. Возможные значения: `unknown`, `advancedThreatProtection`.|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|Приоритет. Возможные значения: `none`, `high`, `low`.|
|creator|String|Адрес электронной почты создателя.|
|creatorNotes|String|Заметки от создателя.|
|assignedTo|String|Имя или электронная почта администратора этой задачи назначены.|
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



