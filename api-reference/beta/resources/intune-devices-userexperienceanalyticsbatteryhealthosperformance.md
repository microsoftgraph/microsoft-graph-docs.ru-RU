---
title: тип ресурса userExperienceAnalyticsBatteryHealthOsPerformance
description: Объект для аналитики работоспособности ос батареи для пользователей содержит сведения, связанные с аккумулятором для всех версий операционной системы в организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 33807a4b7c1d624f086317795479b344368bcf5a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337205"
---
# <a name="userexperienceanalyticsbatteryhealthosperformance-resource-type"></a>тип ресурса userExperienceAnalyticsBatteryHealthOsPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект для аналитики работоспособности ос батареи для пользователей содержит сведения, связанные с аккумулятором для всех версий операционной системы в организации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsBatteryHealthOsPerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-list.md)|[коллекция userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|
|[Get userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-get.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|
|[Создание userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-create.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|Создайте новый [объект userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|
|[Удаление userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md).|
|[Обновление userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-update.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|Обновление свойств объекта [userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности операционной системы работоспособности батареи для аналитики пользовательского интерфейса.|
|activeDevices|Int32|Количество активных устройств для этой версии ос. Допустимые значения 2147483648 2147483647|
|osVersion|String|Версия операционной системы.|
|osBuildNumber|Строка|Создайте номер операционной системы.|
|averageMaxCapacityPercentage|Int32|Значение максимальной емкости для всех устройств с определенной версией операционной системы. Максимальная емкость измеряет полную мощность заряда по сравнению с проектной мощностью для аккумуляторов устройства.. Допустимые значения 2147483648 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|Значение предполагаемого времени работы на полном заряде для всех устройств с определенной версией операционной системы. Единица в минутах. Допустимые значения 2147483648 2147483647|
|averageBatteryAgeInDays|Int32|Значение времени автономной работы для всех устройств, работающих с определенной версией операционной системы в клиенте. Единица в днях. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "osVersion": "String",
  "osBuildNumber": "String",
  "averageMaxCapacityPercentage": 1024,
  "averageEstimatedRuntimeInMinutes": 1024,
  "averageBatteryAgeInDays": 1024
}
```




