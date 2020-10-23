---
title: Тип ресурса Усерекспериенцеаналитиксапфеалсаппликатионперформанце
description: Объект производительности приложения Analytics User Experience содержит сведения о производительности приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 34c36d4103d1f5f9e61913480b75baee75906e89
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724440"
---
# <a name="userexperienceanalyticsapphealthapplicationperformance-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксапфеалсаппликатионперформанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности приложения Analytics User Experience содержит сведения о производительности приложения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксапфеалсаппликатионперформанцес](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-list.md)|Коллекция [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .|
|[Получение Усерекспериенцеаналитиксапфеалсаппликатионперформанце](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-get.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .|
|[Создание Усерекспериенцеаналитиксапфеалсаппликатионперформанце](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-create.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Создание нового объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .|
|[Удаление Усерекспериенцеаналитиксапфеалсаппликатионперформанце](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).|
|[Обновление Усерекспериенцеаналитиксапфеалсаппликатионперформанце](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-update.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Обновление свойств объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.|
|апфангкаунт|Int32|Число зависаний для приложения. Допустимые значения: от 2147483648 до 2147483647|
|апфеалсскоре|Двойное с плавающей точкой|Оценка работоспособности приложения. Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308|
|апфеалсстатус|Строка|Общее состояние работоспособности приложения.|
|аллоргшеалсскоре|Двойное с плавающей точкой|Медианный показатель работоспособности приложения во всех организациях. Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308|
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
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "String (identifier)",
  "appHangCount": 1024,
  "appHealthScore": "4.2",
  "appHealthStatus": "String",
  "allOrgsHealthScore": "4.2",
  "activeDeviceCount": 1024,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": 1024,
  "appCrashCount": 1024,
  "meanTimeToFailureInMinutes": 1024
}
```





