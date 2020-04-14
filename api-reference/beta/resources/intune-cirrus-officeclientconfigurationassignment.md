---
title: Тип ресурса Оффицеклиентконфигуратионассигнмент
description: Назначение конфигурации клиента Office.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 360988d80af473819f4bf25ac72d6f0d817eadbc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43362745"
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

## <a name="relationships"></a>Связи
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



