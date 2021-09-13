---
title: тип ресурса userExperienceAnalyticsMetric
description: Показатель аналитики пользовательских интерфейсов содержит оценку и единицы метрики категории anlaytics пользовательского опыта.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 352a89293bb38e7f03bd7e83d003d465d052335b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125703"
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
|unit|String|Единица метрики аналитики пользовательского опыта.|

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



