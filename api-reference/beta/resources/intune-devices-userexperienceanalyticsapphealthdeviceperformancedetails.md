---
title: Тип ресурса Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс
description: Объект производительности устройства аналитики взаимодействия с пользователем содержит сведения о производительности устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e8857c6a392437335c7324c139fa0b2c9880b12a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733978"
---
# <a name="userexperienceanalyticsapphealthdeviceperformancedetails-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности устройства аналитики взаимодействия с пользователем содержит сведения о производительности устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилсес](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-list.md)|Коллекция [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|
|[Получение Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-get.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|
|[Создание Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-create.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Создание нового объекта [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|
|[Удаление Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md).|
|[Обновление Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-update.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Обновление свойств объекта [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности устройства аналитики взаимодействия с пользователем.|
|eventDateTime|DateTimeOffset|Время возникновения события.|
|eventType|Строка|Тип события.|
|appDisplayName|String|Понятное имя приложения, для которого произошло событие.|
|deviceId|String|Идентификатор устройства.|
|deviceDisplayName|String|Имя устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "eventType": "String",
  "appDisplayName": "String",
  "deviceId": "String",
  "deviceDisplayName": "String"
}
```





