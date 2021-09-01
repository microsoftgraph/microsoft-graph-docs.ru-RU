---
title: тип ресурса userExperienceAnalyticsMetric
description: Показатель аналитики пользовательских интерфейсов содержит оценку и единицы метрики категории anlaytics пользовательского опыта.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62d2714b35ee746a4f2dcdd99e44cbf88e7e83a4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787267"
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
|id|Строка|Уникальный идентификатор метрики аналитики пользовательских интерфейсов.|
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



