---
title: Тип ресурса Усерекспериенцеаналитиксметричистори
description: Журнал метрики аналитики взаимодействия с пользователем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 025e6c7547faf956a6c10a5987a3e42369b7ac72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080819"
---
# <a name="userexperienceanalyticsmetrichistory-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксметричистори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Журнал метрики аналитики взаимодействия с пользователем.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксметричисториес](../api/intune-devices-userexperienceanalyticsmetrichistory-list.md)|Коллекция [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Список свойств и связей объектов [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .|
|[Получение Усерекспериенцеаналитиксметричистори](../api/intune-devices-userexperienceanalyticsmetrichistory-get.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .|
|[Создание Усерекспериенцеаналитиксметричистори](../api/intune-devices-userexperienceanalyticsmetrichistory-create.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Создание нового объекта [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .|
|[Удаление Усерекспериенцеаналитиксметричистори](../api/intune-devices-userexperienceanalyticsmetrichistory-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).|
|[Обновление Усерекспериенцеаналитиксметричистори](../api/intune-devices-userexperienceanalyticsmetrichistory-update.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Обновление свойств объекта [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор истории метрики аналитики взаимодействия с пользователем.|
|метрикдатетиме|DateTimeOffset|Дата и время метрики аналитики взаимодействия с пользователем.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|userExperienceAnalyticsMetric|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Метрика аналитики взаимодействия с пользователем.|

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
  "metricDateTime": "String (timestamp)"
}
```






