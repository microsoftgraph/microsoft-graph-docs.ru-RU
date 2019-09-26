---
title: Тип ресурса Усерекспериенцеаналитиксметрик
description: Метрика аналитики взаимодействия с пользователем содержит показатель и единицы метрики категории взаимодействия с пользователем анлайтикс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 37364d18fbdbd7cbd8b92aefca3a02675d17ba45
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196688"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксметрик

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Метрика аналитики взаимодействия с пользователем содержит показатель и единицы метрики категории взаимодействия с пользователем анлайтикс.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксметрикс](../api/intune-devices-userexperienceanalyticsmetric-list.md)|Коллекция [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Список свойств и связей объектов [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .|
|[Получение Усерекспериенцеаналитиксметрик](../api/intune-devices-userexperienceanalyticsmetric-get.md)|[усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .|
|[Создание Усерекспериенцеаналитиксметрик](../api/intune-devices-userexperienceanalyticsmetric-create.md)|[усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Создание нового объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .|
|[Удаление Усерекспериенцеаналитиксметрик](../api/intune-devices-userexperienceanalyticsmetric-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md).|
|[Обновление Усерекспериенцеаналитиксметрик](../api/intune-devices-userexperienceanalyticsmetric-update.md)|[усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Обновление свойств объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор метрики аналитики взаимодействия с пользователем.|
|значение|Двойное|Значение метрики аналитики взаимодействия с пользователем.|
|устройств|String.|Единица измерения показателя взаимодействия с пользователем.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetric"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "String (identifier)",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "String"
}
```



