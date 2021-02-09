---
title: Тип ресурса userExperienceAnalyticsMetricHistory
description: История показателей аналитики пользовательского интерфейса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6a179a36a837a5eb8c4be71e4a9809ca20246d18
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157612"
---
# <a name="userexperienceanalyticsmetrichistory-resource-type"></a>Тип ресурса userExperienceAnalyticsMetricHistory

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

История показателей аналитики пользовательского интерфейса.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsMetricHistories](../api/intune-devices-userexperienceanalyticsmetrichistory-list.md)|[Коллекция userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Список свойств и связей объектов [userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|
|[Get userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-get.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Чтение свойств и связей объекта [userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|
|[Создание userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-create.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Создание объекта [userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|
|[Удаление userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-delete.md)|Нет|Удаляет [userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|
|[Обновление userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-update.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Обновление свойств объекта [userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор истории показателей аналитики пользовательского интерфейса.|
|metricDateTime|DateTimeOffset|Дата даты анализа пользовательского интерфейса.|
|metricType|String|Тип метрики аналитики пользовательского интерфейса.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|userExperienceAnalyticsMetric|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Показатель аналитики пользовательского интерфейса.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetricHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "String (identifier)",
  "metricDateTime": "String (timestamp)",
  "metricType": "String"
}
```




