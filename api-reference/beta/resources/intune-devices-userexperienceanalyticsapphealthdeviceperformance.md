---
title: Тип ресурса Усерекспериенцеаналитиксапфеалсдевицеперформанце
description: Объект производительности устройства аналитики взаимодействия с пользователем содержит сведения о производительности устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1e7a7775edf7893aeaefa75fc507b930cc8a5234
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733980"
---
# <a name="userexperienceanalyticsapphealthdeviceperformance-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксапфеалсдевицеперформанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности устройства аналитики взаимодействия с пользователем содержит сведения о производительности устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксапфеалсдевицеперформанцес](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-list.md)|Коллекция [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .|
|[Получение Усерекспериенцеаналитиксапфеалсдевицеперформанце](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-get.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .|
|[Создание Усерекспериенцеаналитиксапфеалсдевицеперформанце](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-create.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Создание нового объекта [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .|
|[Удаление Усерекспериенцеаналитиксапфеалсдевицеперформанце](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).|
|[Обновление Усерекспериенцеаналитиксапфеалсдевицеперформанце](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-update.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Обновление свойств объекта [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности устройства аналитики взаимодействия с пользователем.|
|deviceModel|String|Имя модели устройства.|
|девицемануфактурер|Строка|Название изготовителя устройства.|
|аппкрашкаунт|Int32|Количество сбоев приложений для устройства. Допустимые значения: от 2147483648 до 2147483647|
|крашедаппкаунт|Int32|Количество отдельных сбоев приложений для устройства. Допустимые значения: от 2147483648 до 2147483647|
|апфангкаунт|Int32|Количество зависаний приложения для устройства. Допустимые значения: от 2147483648 до 2147483647|
|меантиметофаилуреинминутес|Int32|Среднее время до сбоя устройства в минутах. Допустимые значения: от 2147483648 до 2147483647|
|девицеапфеалсскоре|Двойное с плавающей точкой|Показатель работоспособности приложения для устройства. Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308|
|девицеапфеалсстатус|Строка|Общее состояние работоспособности приложений для устройства.|
|deviceId|String|Идентификатор устройства.|
|deviceDisplayName|String|Имя устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "String (identifier)",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "appCrashCount": 1024,
  "crashedAppCount": 1024,
  "appHangCount": 1024,
  "meanTimeToFailureInMinutes": 1024,
  "deviceAppHealthScore": "4.2",
  "deviceAppHealthStatus": "String",
  "deviceId": "String",
  "deviceDisplayName": "String"
}
```





