---
title: тип ресурса userExperienceAnalyticsNotAutopilotReadyDevice
description: Устройство аналитики пользовательского интерфейса не готово для автопилота Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e85b13e540547111e2aea513f7fe595f7ece7404
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58804276"
---
# <a name="userexperienceanalyticsnotautopilotreadydevice-resource-type"></a>тип ресурса userExperienceAnalyticsNotAutopilotReadyDevice

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Устройство аналитики пользовательского интерфейса не готово для автопилота Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsNotAutopilotReadyDevices](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-list.md)|[коллекция userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|Список свойств и связей [объектов userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|
|[Get userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-get.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|Чтение свойств и связей [объекта userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|
|[Создание userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-create.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|Создание нового [объекта userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|
|[Удаление userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md).|
|[Обновление userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-update.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|Обновление свойств объекта [userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор устройства intune аналитики пользовательского интерфейса.|
|deviceName|String|Имя устройства intune.|
|serialNumber|String|Серийный номер устройства intune.|
|manufacturer|String|Производитель устройства intune.|
|model|String|Модель устройства intune.|
|managedBy|Строка|Устройство intune управляется.|
|autoPilotRegistered|Логический|Автопилотрегистер устройства intune.|
|autoPilotProfileAssigned|Логический|Автопилот Устройства intuneProfileAssigned.|
|azureAdRegistered|Логический|Устройство intune azureAdRegistered.|
|azureAdJoinType|Строка|Azure Ad ad для устройства intune присоединяется кType.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "id": "String (identifier)",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "managedBy": "String",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdJoinType": "String"
}
```



