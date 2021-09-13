---
title: тип ресурса userExperienceAnalyticsDeviceStartupProcess
description: Сведения о процессе запуска устройства для аналитики пользовательского интерфейса.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0ff11a7ed29902ebde395dbb7d3ed183d1c63915
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125759"
---
# <a name="userexperienceanalyticsdevicestartupprocess-resource-type"></a>тип ресурса userExperienceAnalyticsDeviceStartupProcess

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о процессе запуска устройства для аналитики пользовательского интерфейса.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список пользователейExperienceAnalyticsDeviceStartupProcesses](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-list.md)|[коллекция userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Список свойств и связей [объектов userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|
|[Get userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-get.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Чтение свойств и связей [объекта userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|
|[Создание userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-create.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Создание нового [объекта userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|
|[Удаление userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|
|[Обновление userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-update.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Обновление свойств объекта [userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.|
|managedDeviceId|String|ID устройства аналитики пользовательского интерфейса.|
|processName|String|Имя процесса запуска устройства для аналитики пользовательского интерфейса.|
|productName|String|Имя продукта процесса запуска устройства для аналитики пользовательского интерфейса.|
|publisher|String|Издатель процесса запуска устройства для аналитики пользовательских интерфейсов.|
|startupImpactInMs|Int32|Влияние процесса запуска устройства для аналитики пользовательских интерфейсов в миллисекунд.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupProcess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "startupImpactInMs": 1024
}
```



