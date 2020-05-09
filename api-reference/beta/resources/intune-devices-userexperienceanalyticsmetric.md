---
title: Тип ресурса Усерекспериенцеаналитиксметрик
description: Метрика аналитики взаимодействия с пользователем содержит показатель и единицы метрики категории взаимодействия с пользователем анлайтикс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e8239ac7e4583841d3c8a095bc85d9c9eb9b9d78
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178397"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксметрик

Пространство имен: microsoft.graph

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
|id|Строка|Уникальный идентификатор метрики аналитики взаимодействия с пользователем.|
|значение|Двойное с плавающей точкой|Значение метрики аналитики взаимодействия с пользователем.|
|устройств|Строка|Единица измерения показателя взаимодействия с пользователем.|

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
  "value": "4.2",
  "unit": "String"
}
```



