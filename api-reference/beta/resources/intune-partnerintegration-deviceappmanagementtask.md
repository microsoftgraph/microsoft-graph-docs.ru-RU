---
title: Тип ресурса Девицеаппманажементтаск
description: Задача управления приложениями для устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2767ec1fee73f7bc9cdc774d53f5d985cdfd2439
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001890"
---
# <a name="deviceappmanagementtask-resource-type"></a>Тип ресурса Девицеаппманажементтаск

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Задача управления приложениями для устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеаппманажементтаскс](../api/intune-partnerintegration-deviceappmanagementtask-list.md)|Коллекция [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Список свойств и связей объектов [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[Получение Девицеаппманажементтаск](../api/intune-partnerintegration-deviceappmanagementtask-get.md)|[Девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Чтение свойств и связей объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[Создание Девицеаппманажементтаск](../api/intune-partnerintegration-deviceappmanagementtask-create.md)|[Девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Создание нового объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[Удаление Девицеаппманажементтаск](../api/intune-partnerintegration-deviceappmanagementtask-delete.md)|Нет|Удаляет объект [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md).|
|[Обновление Девицеаппманажементтаск](../api/intune-partnerintegration-deviceappmanagementtask-update.md)|[Девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Обновление свойств объекта [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[действие updateStatus](../api/intune-partnerintegration-deviceappmanagementtask-updatestatus.md)|Нет|Задайте состояние задачи и вложите заметку.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|Строка|Имя.|
|description|String|Описание.|
|createdDateTime|DateTimeOffset|Дата создания.|
|dueDateTime|DateTimeOffset|Дата выполнения.|
|category|[Девицеаппманажементтасккатегори](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|Категория. Возможные значения: `unknown`, `advancedThreatProtection`.|
|priority|[Девицеаппманажементтаскприорити](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|Приоритет. Возможные значения: `none`, `high`, `low`.|
|модуль|String|Адрес электронной почты создателя.|
|Креаторнотес|String|Заметки автора.|
|assignedTo|String|Имя или электронная почта администратора, которому назначена эта задача.|
|status|[Девицеаппманажементтаскстатус](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|Состояние. Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.|

## <a name="relationships"></a>Отношения
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





