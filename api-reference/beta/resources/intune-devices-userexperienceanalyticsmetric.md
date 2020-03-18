---
title: Тип ресурса Усерекспериенцеаналитиксметрик
description: Метрика аналитики взаимодействия с пользователем содержит показатель и единицы метрики категории взаимодействия с пользователем анлайтикс.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0d7118bacfce358c2cd3788f6618e6025ddb9894
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783776"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксметрик

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Метрика аналитики взаимодействия с пользователем содержит показатель и единицы метрики категории взаимодействия с пользователем анлайтикс.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксметрикс](../api/intune-devices-userexperienceanalyticsmetric-list.md)|Коллекция [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Список свойств и связей объектов [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .|
|[Получение Усерекспериенцеаналитиксметрик](../api/intune-devices-userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .|
|[Создание Усерекспериенцеаналитиксметрик](../api/intune-devices-userexperienceanalyticsmetric-create.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Создание нового объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .|
|[Удаление Усерекспериенцеаналитиксметрик](../api/intune-devices-userexperienceanalyticsmetric-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md).|
|[Обновление Усерекспериенцеаналитиксметрик](../api/intune-devices-userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Обновление свойств объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор метрики аналитики взаимодействия с пользователем.|
|значение|Двойное с плавающей точкой|Значение метрики аналитики взаимодействия с пользователем.|
|устройств|String|Единица измерения показателя взаимодействия с пользователем.|

## <a name="relationships"></a>Связи
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



