---
title: Тип ресурса Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс
description: Объект производительности устройства аналитики взаимодействия с пользователем содержит сведения о производительности устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 834d2e2871e8ddf7366ddc1ea0e77398eeae48f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082122"
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
|[Получение Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-get.md)|[усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|
|[Создание Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-create.md)|[усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Создание нового объекта [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|
|[Удаление Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md).|
|[Обновление Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-update.md)|[усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Обновление свойств объекта [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|

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






