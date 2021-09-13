---
title: тип ресурса userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId
description: Объект производительности приложения для аналитики пользовательского интерфейса содержит производительность приложения по id-устройству версии приложения.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a730dc54bcd7095f21bf503cbf341dfd66187880
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081054"
---
# <a name="userexperienceanalyticsapphealthappperformancebyappversiondeviceid-resource-type"></a>тип ресурса userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности приложения для аналитики пользовательского интерфейса содержит производительность приложения по id-устройству версии приложения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список пользователейExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceIds](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-list.md)|[коллекция userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|Список свойств и связей [объектов userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|
|[Get userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|Чтение свойств и связей объекта [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|
|[Создание userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|Создайте новый [объект userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|
|[Удаление userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|
|[Обновление userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|Обновление свойств объекта [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности приложения для аналитики пользовательского интерфейса.|
|deviceId|String|ID устройства.|
|deviceDisplayName|String|Имя устройства.|
|processedDateTime|DateTimeOffset|Дата и время последнего вычисления статистики.|
|appName|String|Имя приложения.|
|appDisplayName|String|Удобное имя приложения.|
|appPublisher|String|Издатель приложения.|
|appVersion|String|Версия приложения.|
|appCrashCount|Int32|Количество сбоей для приложения. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceDisplayName": "String",
  "processedDateTime": "String (timestamp)",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appVersion": "String",
  "appCrashCount": 1024
}
```



