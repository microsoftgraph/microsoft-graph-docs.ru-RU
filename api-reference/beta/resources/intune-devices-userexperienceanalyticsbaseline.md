---
title: тип ресурса userExperienceAnalyticsBaseline
description: Базовый объект аналитики пользовательских интерфейсов содержит базовые значения, с которыми можно сравнить оценки аналитики пользовательских интерфейсов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8d33eec55a5e7309a0ed80fd7fcf4d62b780a1f8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141451"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a>тип ресурса userExperienceAnalyticsBaseline

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый объект аналитики пользовательских интерфейсов содержит базовые значения, с которыми можно сравнить оценки аналитики пользовательских интерфейсов.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsBaselines](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|[коллекция userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Список свойств и связей [объектов userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Get userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Чтение свойств и связей [объекта userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Создание userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Создание нового [объекта userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Удаление userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|Нет|Удаляет [userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Обновление userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Обновление свойств объекта [userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор базовой базы аналитики пользовательского интерфейса.|
|displayName|Строка|Имя базовой базы аналитики пользовательского интерфейса.|
|overallScore|Int32|Общая оценка базовой базы аналитики пользовательских интерфейсов.|
|isBuiltIn|Boolean|Означает, является ли текущий базовый уровень коммерческим медианым или настраиваемой базовой базой.|
|createdDateTime|DateTimeOffset|Дата создания настраиваемой базовой линии.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Показатели производительности загрузки устройств для аналитики пользовательского интерфейса.|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Метрики для аналитики пользовательских интерфейсов.|
|rebootAnalyticsMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Аналитика пользовательских интерфейсов перезагружает метрики аналитики.|
|resourcePerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Показатели производительности ресурсов аналитики пользовательского опыта.|
|appHealthMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Показатели здоровья приложения для аналитики пользовательского интерфейса.|
|workFromAnywhereMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Аналитика пользовательских интерфейсов работает из любой метрики.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
  "isBuiltIn": true,
  "createdDateTime": "String (timestamp)"
}
```




