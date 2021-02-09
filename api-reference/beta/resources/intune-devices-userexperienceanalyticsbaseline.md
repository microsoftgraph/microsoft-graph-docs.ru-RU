---
title: Тип ресурса userExperienceAnalyticsBaseline
description: Базовый объект аналитики пользовательского интерфейса содержит базовые значения, с которыми сравнивают показатели анализа пользовательского интерфейса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 106600e99e7002a39af93a8691980c41c6bf0697
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158452"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a>Тип ресурса userExperienceAnalyticsBaseline

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый объект аналитики пользовательского интерфейса содержит базовые значения, с которыми сравнивают показатели анализа пользовательского интерфейса.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsBaselines](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|[Коллекция userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Список свойств и связей объектов [userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Get userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Чтение свойств и связей объекта [userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Создание userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Создание объекта [userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Удаление userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|Нет|Удаляет [userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Обновление userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Обновление свойств объекта [userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор базового плана анализа пользовательского интерфейса.|
|displayName|String|Имя базового плана анализа пользовательского интерфейса.|
|overallScore|Int32|Общая оценка базовых показателей аналитики пользовательского интерфейса.|
|isBuiltIn|Boolean|Означает, является ли текущий базовый план коммерческим базовым уровнем медиана или настраиваемой базой данных.|
|createdDateTime|DateTimeOffset|Дата создания настраиваемой базовой параметров.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Показатели производительности загрузки устройства аналитики пользовательского интерфейса.|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Метрики метрики анализа пользовательского интерфейса.|
|rebootAnalyticsMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Показатели аналитики пользовательского интерфейса перезагружают метрики аналитики.|
|resourcePerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Показатели производительности ресурсов аналитики пользовательского интерфейса.|
|appHealthMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Показатели состояния приложения аналитики пользовательского интерфейса.|

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




