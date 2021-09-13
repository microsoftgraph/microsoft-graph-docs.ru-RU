---
title: тип ресурса userExperienceAnalyticsDeviceStartupProcessPerformance
description: Производительность процесса запуска устройства для аналитики пользовательского интерфейса.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6f8ade092e5927792386140b53caa1ea769f3f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125724"
---
# <a name="userexperienceanalyticsdevicestartupprocessperformance-resource-type"></a>тип ресурса userExperienceAnalyticsDeviceStartupProcessPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Производительность процесса запуска устройства для аналитики пользовательского интерфейса.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список пользователейExperienceAnalyticsDeviceStartupProcessPerformances](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-list.md)|[коллекция userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|
|[Get userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-get.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|
|[Создание userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-create.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Создание нового [объекта userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|
|[Удаление userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).|
|[Обновление userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-update.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Обновление свойств объекта [userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор производительности процесса запуска устройства для аналитики пользовательского интерфейса.|
|processName|String|Имя процесса запуска устройства для аналитики пользовательского интерфейса.|
|productName|String|Имя продукта процесса запуска устройства для аналитики пользовательского интерфейса.|
|publisher|String|Издатель процесса запуска устройства для аналитики пользовательских интерфейсов.|
|deviceCount|Int64|Процесс запуска устройства аналитики пользовательских интерфейсов суммирован.|
|medianImpactInMs|Int32|Медиана процесса запуска устройств для аналитики пользовательских интерфейсов в миллисекунд.|
|totalImpactInMs|Int32|Процесс запуска устройства для аналитики пользовательских интерфейсов полностью влияет на миллисекунд.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "id": "String (identifier)",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "deviceCount": 1024,
  "medianImpactInMs": 1024,
  "totalImpactInMs": 1024
}
```



