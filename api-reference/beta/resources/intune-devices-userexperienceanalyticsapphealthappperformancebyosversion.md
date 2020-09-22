---
title: Тип ресурса Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион
description: Сущность производительности приложения аналитики "взаимодействие с пользователем" содержит сведения о производительности приложения по версии ОС.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 673833ebcdccb90f5d691a7dad9d560da774add3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082134"
---
# <a name="userexperienceanalyticsapphealthappperformancebyosversion-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность производительности приложения аналитики "взаимодействие с пользователем" содержит сведения о производительности приложения по версии ОС.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсионс](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-list.md)|Коллекция [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .|
|[Получение Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-get.md)|[усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .|
|[Создание Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-create.md)|[усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Создание нового объекта [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .|
|[Удаление Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md).|
|[Обновление Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-update.md)|[усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Обновление свойств объекта [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности "версия приложения аналитики взаимодействия с пользователем".|
|osVersion|String|Версия операционной системы приложения.|
|осбуилднумбер|Строка|Номер сборки ОС приложения.|
|активедевицекаунт|Int32|Количество устройств, в которых приложение было активно. Допустимые значения: от 2147483648 до 2147483647|
|appName|String|Имя приложения.|
|appDisplayName|String|Понятное имя приложения.|
|апппублишер|Строка|Издатель приложения.|
|аппусажедуратион|Int32|Общее время использования приложения в минутах. Допустимые значения: от 2147483648 до 2147483647|
|аппкрашкаунт|Int32|Число сбоев для приложения. Допустимые значения: от 2147483648 до 2147483647|
|меантиметофаилуреинминутес|Int32|Среднее время до сбоя приложения в минутах. Допустимые значения: от 2147483648 до 2147483647|

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






