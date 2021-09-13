---
title: тип ресурса userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails
description: Объект производительности приложения для аналитики пользовательских интерфейсов содержит производительность приложения с помощью сведений о версии приложения.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: febfdbccfb3fd939928c8ddcb9897d133fc12837
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091302"
---
# <a name="userexperienceanalyticsapphealthappperformancebyappversiondetails-resource-type"></a>тип ресурса userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности приложения для аналитики пользовательских интерфейсов содержит производительность приложения с помощью сведений о версии приложения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetailses](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-list.md)|[коллекция userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|Список свойств и связей [объектов userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|
|[Get userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|Чтение свойств и связей [объекта userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|
|[Создание userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|Создание нового [объекта userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|
|[Удаление userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md).|
|[Обновление userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|Обновление свойств объекта [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности приложения для аналитики пользовательского интерфейса.|
|deviceCountWithCrashes|Int32|Общее число устройств, которые сообщили об одном или нескольких сбоях приложения для этого приложения и версии. Допустимые значения 2147483648 2147483647|
|isMostUsedVersion|Логический|Является ли версия приложения наиболее используемой версией для этого приложения.|
|isLatestUsedVersion|Логическое|Является ли версия приложения последней версией для используемого приложения.|
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
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails",
  "id": "String (identifier)",
  "deviceCountWithCrashes": 1024,
  "isMostUsedVersion": true,
  "isLatestUsedVersion": true,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appVersion": "String",
  "appCrashCount": 1024
}
```



