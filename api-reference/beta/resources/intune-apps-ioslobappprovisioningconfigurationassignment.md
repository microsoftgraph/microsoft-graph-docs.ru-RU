---
title: Тип ресурса iosLobAppProvisioningConfigurationAssignment
description: Класс, содержащий свойства, используемые для назначения группы для iOS, бизнес-приложения подготовки и настройки.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7b88526c5cef42d4bd0637fed718f620741fbc7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395134"
---
# <a name="ioslobappprovisioningconfigurationassignment-resource-type"></a>Тип ресурса iosLobAppProvisioningConfigurationAssignment

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для назначения группы для iOS, бизнес-приложения подготовки и настройки.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosLobAppProvisioningConfigurationAssignments](../api/intune-apps-ioslobappprovisioningconfigurationassignment-list.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) коллекции|Свойства списка и связей объектов [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|
|[Получение iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-get.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Чтение свойства и связи объекта [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|
|[Создание iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-create.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Создание нового объекта [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|
|[Удаление iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-delete.md)|Нет|Удаляет [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).|
|[Обновление iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-update.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Обновление свойства объекта [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевое назначение группы, определенное администратором.|

## <a name="relationships"></a>Отношения
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




