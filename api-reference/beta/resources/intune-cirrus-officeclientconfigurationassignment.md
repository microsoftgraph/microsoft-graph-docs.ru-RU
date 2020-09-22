---
title: Тип ресурса Оффицеклиентконфигуратионассигнмент
description: Назначение конфигурации клиента Office.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c7a6e9f1ef14977a7d5694d90649d96e5d27a2fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021688"
---
# <a name="officeclientconfigurationassignment-resource-type"></a>Тип ресурса Оффицеклиентконфигуратионассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение конфигурации клиента Office.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Оффицеклиентконфигуратионассигнментс](../api/intune-cirrus-officeclientconfigurationassignment-list.md)|Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Список свойств и связей объектов [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|
|[Получение Оффицеклиентконфигуратионассигнмент](../api/intune-cirrus-officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Чтение свойств и связей объекта [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|
|[Создание Оффицеклиентконфигуратионассигнмент](../api/intune-cirrus-officeclientconfigurationassignment-create.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Создание нового объекта [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|
|[Удаление Оффицеклиентконфигуратионассигнмент](../api/intune-cirrus-officeclientconfigurationassignment-delete.md)|Нет|Удаляет объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md).|
|[Обновление Оффицеклиентконфигуратионассигнмент](../api/intune-cirrus-officeclientconfigurationassignment-update.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Обновление свойств объекта [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта Оффицеконфигуратионассигнмент.|
|target|[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|Целевое назначение, заданное администратором.|

## <a name="relationships"></a>Отношения
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```






