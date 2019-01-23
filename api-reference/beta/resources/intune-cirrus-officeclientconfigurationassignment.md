---
title: Тип ресурса officeClientConfigurationAssignment
description: Назначение конфигурации клиента Office.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be86dd036619174ae176c2b24487cc18f515c847
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423967"
---
# <a name="officeclientconfigurationassignment-resource-type"></a>Тип ресурса officeClientConfigurationAssignment

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение конфигурации клиента Office.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список officeClientConfigurationAssignments](../api/intune-cirrus-officeclientconfigurationassignment-list.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции|Свойства списка и связей объектов [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|
|[Получение officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Чтение свойства и связи объекта [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|
|[Создание officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-create.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Создание нового объекта [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|
|[Удаление officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-delete.md)|Нет|Удаляет [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).|
|[Обновление officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-update.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Обновление свойства объекта [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор OfficeConfigurationAssignment.|
|target|[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|Назначение целевой, определенные администратором.|

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



