---
title: тип ресурса userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: Объект производительности приложения для аналитики пользовательского интерфейса содержит сведения о производительности приложения в версии ОС.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62c0fc4ec2ca220a4544664be567d0f7aedf8629
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081040"
---
# <a name="userexperienceanalyticsapphealthappperformancebyosversion-resource-type"></a>тип ресурса userExperienceAnalyticsAppHealthAppPerformanceByOSVersion

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности приложения для аналитики пользовательского интерфейса содержит сведения о производительности приложения в версии ОС.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список пользователейExperienceAnalyticsAppHealthAppPerformanceByOSVersions](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-list.md)|[коллекция userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Список свойств и связей [объектов userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|
|[Get userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Чтение свойств и связей [объекта userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|
|[Создание userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Создание нового [объекта userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|
|[Удаление userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|
|[Обновление userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Обновление свойств объекта [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности версии версии пользовательского интерфейса для аналитики приложений.|
|osVersion|String|Версия ос приложения.|
|osBuildNumber|String|Число сборки ос приложения.|
|activeDeviceCount|Int32|Количество устройств, на которых приложение было активным. Допустимые значения 2147483648 2147483647|
|appName|String|Имя приложения.|
|appDisplayName|String|Удобное имя приложения.|
|appPublisher|String|Издатель приложения.|
|appUsageDuration|Int32|Общее время использования приложения в минутах. Допустимые значения 2147483648 2147483647|
|appCrashCount|Int32|Количество сбоей для приложения. Допустимые значения 2147483648 2147483647|
|meanTimeToFailureInMinutes|Int32|Время сбоя для приложения в минутах. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
  "id": "String (identifier)",
  "osVersion": "String",
  "osBuildNumber": "String",
  "activeDeviceCount": 1024,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": 1024,
  "appCrashCount": 1024,
  "meanTimeToFailureInMinutes": 1024
}
```



