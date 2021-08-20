---
title: тип ресурса userExperienceAnalyticsMetric
description: Показатель аналитики пользовательских интерфейсов содержит оценку и единицы метрики категории anlaytics пользовательского опыта.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e51ae807419adf240ebd5507869c00d1882281a84743156d34f7489a5623a00
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54200518"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a>тип ресурса userExperienceAnalyticsMetric

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Показатель аналитики пользовательских интерфейсов содержит оценку и единицы метрики категории anlaytics пользовательского опыта.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsMetrics](../api/intune-devices-userexperienceanalyticsmetric-list.md)|[коллекция userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Список свойств и связей [объектов userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)|
|[Get userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Чтение свойств и связей [объекта userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)|
|[Создание userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-create.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Создание нового [объекта userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)|
|[Удаление userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-delete.md)|Нет|Удаляет [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).|
|[Обновление userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Обновление свойств объекта [userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор метрики аналитики пользовательских интерфейсов.|
|значение|Двойное с плавающей точкой|Значение метрики аналитики пользовательских интерфейсов.|
|unit|Строка|Единица метрики аналитики пользовательского опыта.|

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




