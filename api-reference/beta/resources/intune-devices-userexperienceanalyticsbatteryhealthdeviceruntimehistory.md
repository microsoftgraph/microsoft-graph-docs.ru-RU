---
title: тип ресурса userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory
description: Объект истории истории запуска батареи для аналитики пользовательских интерфейсов содержит тенденцию времени работы устройства в течение 30 дней.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46c88e9bccacade261ca1dbe8f10e43a3e9b4d68
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338773"
---
# <a name="userexperienceanalyticsbatteryhealthdeviceruntimehistory-resource-type"></a>тип ресурса userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект истории истории запуска батареи для аналитики пользовательских интерфейсов содержит тенденцию времени работы устройства в течение 30 дней.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список пользователейExperienceAnalyticsBatteryHealthDeviceRuntimeHistories](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-list.md)|[коллекция userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|Список свойств и связей [объектов userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|
|[Get userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-get.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|Чтение свойств и связей [объекта userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|
|[Создание userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-create.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|Создайте новый [объект userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|
|[Удаление userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md).|
|[Обновление userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-update.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|Обновление свойств объекта [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта для аналитики пользовательского интерфейса для запуска заряда батареи.|
|deviceId|String|Уникальный идентификатор устройства, идентификатор устройства Intune DeviceID или SCCM.|
|runtimeDateTime|Строка|Время даты для экземпляра истории запуска.|
|estimatedRuntimeInMinutes|Int32|Предполагаемое время работы устройства при полной зарядке батареи. Единица в минутах. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory",
  "id": "String (identifier)",
  "deviceId": "String",
  "runtimeDateTime": "String",
  "estimatedRuntimeInMinutes": 1024
}
```




