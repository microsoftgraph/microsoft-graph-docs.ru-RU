---
title: Тип ресурса Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион
description: Сущность производительности приложения аналитики "взаимодействие с пользователем" содержит сведения о производительности приложения по версии приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 04bfeb269bc41c8114ca11427c8a41e56e2c36aa
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724433"
---
# <a name="userexperienceanalyticsapphealthappperformancebyappversion-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность производительности приложения аналитики "взаимодействие с пользователем" содержит сведения о производительности приложения по версии приложения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсионс](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-list.md)|Коллекция [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .|
|[Получение Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .|
|[Создание Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|Создание нового объекта [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .|
|[Удаление Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).|
|[Обновление Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|Обновление свойств объекта [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.|
|аппверсион|Строка|Версия приложения.|
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
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
  "id": "String (identifier)",
  "appVersion": "String",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": 1024,
  "appCrashCount": 1024,
  "meanTimeToFailureInMinutes": 1024
}
```





