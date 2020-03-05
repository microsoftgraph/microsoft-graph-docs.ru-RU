---
title: Тип ресурса Усерекспериенцеаналитиксинсигхт
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b9e9e40916e92dd45726fb5bc04387f180bf8395
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528462"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксинсигхт

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|усерекспериенцеаналитиксметриЦид|String|Уникальный идентификатор аналитического интерфейса пользователя.|
|инсигхтид|String|Уникальный идентификатор аналитического интерфейса пользователя.|
|values|Коллекция [усерекспериенцеаналитиксинсигхтвалуе](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)|Значение аналитического интерфейса пользователя.|
|severity|[userExperienceAnalyticsInsightSeverity](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|Значение аналитического интерфейса пользователя. Возможные значения: `none`, `informational`, `warning`, `error`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
  "userExperienceAnalyticsMetricId": "String",
  "insightId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble",
      "value": "<Unknown Primitive Type Edm.Double>"
    }
  ],
  "severity": "String"
}
```



