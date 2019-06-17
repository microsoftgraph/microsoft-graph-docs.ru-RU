---
title: Тип ресурса Граупполициконфигуратионассигнмент
description: Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0ec4346174bdaafbc37c0721462ba8fd612abcc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975947"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a>Тип ресурса Граупполициконфигуратионассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициконфигуратионассигнментс](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Список свойств и связей объектов [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|
|[Получение Граупполициконфигуратионассигнмент](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[Граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Чтение свойств и связей объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|
|[Создание Граупполициконфигуратионассигнмент](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[Граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Создание нового объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|
|[Удаление Граупполициконфигуратионассигнмент](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|Нет|Удаляет объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).|
|[Обновление Граупполициконфигуратионассигнмент](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[Граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Обновление свойств объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Тип групп, нацеленных на конфигурацию групповой политики.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





