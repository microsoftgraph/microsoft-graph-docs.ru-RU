---
title: тип ресурса userExperienceAnalyticsDeviceScores
description: Устройство аналитики пользовательских интерфейсов консолидирует различные оценки аналитики конечных точек.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3ecd5fefcb24d9672bac4ee597453e5c151d20df
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869043"
---
# <a name="userexperienceanalyticsdevicescores-resource-type"></a>тип ресурса userExperienceAnalyticsDeviceScores

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Устройство аналитики пользовательских интерфейсов консолидирует различные оценки аналитики конечных точек.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsDeviceScoreses](../api/intune-devices-userexperienceanalyticsdevicescores-list.md)|[коллекция userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Список свойств и связей [объектов userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|
|[Get userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-get.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Чтение свойств и связей [объекта userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|
|[Создание userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-create.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Создание нового [объекта userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|
|[Удаление userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md).|
|[Обновление userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-update.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Обновление свойств объекта [userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства аналитики пользовательских интерфейсов.|
|deviceName|String|Имя устройства аналитики пользовательского интерфейса.|
|model|String|Модель устройства аналитики пользовательских интерфейсов.|
|manufacturer|String|Производитель устройств аналитики пользовательских интерфейсов.|
|endpointAnalyticsScore|Двойное с плавающей точкой|Оценка устройства аналитики пользовательского интерфейса. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|startupPerformanceScore|Двойное с плавающей точкой|Оценка производительности запуска устройства для аналитики пользовательского интерфейса. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|appReliabilityScore|Двойное с плавающей точкой|Оценка надежности приложения приложения для аналитики пользовательского интерфейса. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceScores"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "id": "String (identifier)",
  "deviceName": "String",
  "model": "String",
  "manufacturer": "String",
  "endpointAnalyticsScore": "4.2",
  "startupPerformanceScore": "4.2",
  "appReliabilityScore": "4.2"
}
```




