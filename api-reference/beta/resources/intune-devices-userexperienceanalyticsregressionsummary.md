---
title: Тип ресурса Усерекспериенцеаналитиксрегрессионсуммари
description: Сводка по регрессии аналитики взаимодействия с пользователем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d54a61e380c9bdb39d2f0e1ac9a5b41766380ee1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080784"
---
# <a name="userexperienceanalyticsregressionsummary-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксрегрессионсуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по регрессии аналитики взаимодействия с пользователем.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Усерекспериенцеаналитиксрегрессионсуммари](../api/intune-devices-userexperienceanalyticsregressionsummary-get.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) .|
|[Обновление Усерекспериенцеаналитиксрегрессионсуммари](../api/intune-devices-userexperienceanalyticsregressionsummary-update.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Обновление свойств объекта [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) .|
|[Функция Суммаризедевицерегрессионперформанце](../api/intune-devices-userexperienceanalyticsregressionsummary-summarizedeviceregressionperformance.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор сводки по регрессии аналитики взаимодействия с пользователем.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|моделрегрессион|Коллекция [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Значения метрик для регрессии модели аналитики взаимодействия с пользователем.|
|мануфактуреррегрессион|Коллекция [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Значения метрик для регрессии разработчиков аналитики взаимодействия с пользователем.|
|оператингсистемрегрессион|Коллекция [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Значения метрик для регрессии операционной системы аналитики взаимодействия с пользователем.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "String (identifier)"
}
```






