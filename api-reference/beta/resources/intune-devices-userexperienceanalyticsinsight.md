---
title: Тип ресурса Усерекспериенцеаналитиксинсигхт
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 36277b147e7eabc6f28aef3877538ebbc429f381
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341240"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксинсигхт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|усерекспериенцеаналитиксметриЦид|String|Уникальный идентификатор аналитического интерфейса пользователя.|
|инсигхтид|String|Уникальный идентификатор аналитического интерфейса пользователя.|
|значение|Коллекция [усерекспериенцеаналитиксинсигхтвалуе](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)|Значение аналитического интерфейса пользователя.|

## <a name="relationships"></a>Отношения
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
  "value": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble"
    }
  ]
}
```



