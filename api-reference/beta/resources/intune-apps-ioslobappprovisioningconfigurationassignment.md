---
title: Тип ресурса Иослобапппровисионингконфигуратионассигнмент
description: Класс, содержащий свойства, которые используются для назначения групп при подготовке и настройке бизнес-приложения для iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 647c4aa8ee9c6a0d83d7168cf9e78cd610e1eee3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003887"
---
# <a name="ioslobappprovisioningconfigurationassignment-resource-type"></a>Тип ресурса Иослобапппровисионингконфигуратионассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, которые используются для назначения групп при подготовке и настройке бизнес-приложения для iOS.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иослобапппровисионингконфигуратионассигнментс](../api/intune-apps-ioslobappprovisioningconfigurationassignment-list.md)|Коллекция [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Список свойств и связей объектов [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|
|[Получение Иослобапппровисионингконфигуратионассигнмент](../api/intune-apps-ioslobappprovisioningconfigurationassignment-get.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Чтение свойств и связей объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|
|[Создание Иослобапппровисионингконфигуратионассигнмент](../api/intune-apps-ioslobappprovisioningconfigurationassignment-create.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Создание нового объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|
|[Удаление Иослобапппровисионингконфигуратионассигнмент](../api/intune-apps-ioslobappprovisioningconfigurationassignment-delete.md)|Нет|Удаляет объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).|
|[Обновление Иослобапппровисионингконфигуратионассигнмент](../api/intune-apps-ioslobappprovisioningconfigurationassignment-update.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Обновление свойств объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевое назначение группы, определенное администратором.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```






