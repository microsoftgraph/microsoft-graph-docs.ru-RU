---
title: Тип ресурса Усерекспериенцеаналитиксапфеалсдевицемоделперформанце
description: Объект производительности модели устройства Analytics User Experience содержит сведения о производительности модели устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 85980e65e8988b0c90b28c3283ac341e2eccf6c9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727409"
---
# <a name="userexperienceanalyticsapphealthdevicemodelperformance-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксапфеалсдевицемоделперформанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности модели устройства Analytics User Experience содержит сведения о производительности модели устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксапфеалсдевицемоделперформанцес](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-list.md)|Коллекция [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .|
|[Получение Усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-get.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .|
|[Создание Усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-create.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Создание нового объекта [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .|
|[Удаление Усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).|
|[Обновление Усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-update.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Обновление свойств объекта [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности модели устройства Analytics User Experience.|
|deviceModel|String|Имя модели устройства.|
|девицемануфактурер|Строка|Название изготовителя устройства.|
|активедевицекаунт|Int32|Количество активных устройств для модели. Допустимые значения: от 2147483648 до 2147483647|
|меантиметофаилуреинминутес|Int32|Среднее время до сбоя устройства модели в минутах. Допустимые значения: от 2147483648 до 2147483647|
|моделапфеалсскоре|Двойное с плавающей точкой|Показатель работоспособности приложения модели устройства. Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308|
|моделапфеалсстатус|Строка|Общее состояние работоспособности приложения модели устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "id": "String (identifier)",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "activeDeviceCount": 1024,
  "meanTimeToFailureInMinutes": 1024,
  "modelAppHealthScore": "4.2",
  "modelAppHealthStatus": "String"
}
```





