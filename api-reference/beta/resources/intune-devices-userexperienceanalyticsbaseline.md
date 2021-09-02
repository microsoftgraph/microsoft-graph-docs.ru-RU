---
title: тип ресурса userExperienceAnalyticsBaseline
description: Базовый объект аналитики пользовательских интерфейсов содержит базовые значения, с которыми можно сравнить оценки аналитики пользовательских интерфейсов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 730537696691c1039e924817d653497fb147338b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803779"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a>тип ресурса userExperienceAnalyticsBaseline

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|id|String|Уникальный идентификатор базовой базы аналитики пользовательского интерфейса.|
|displayName|String|Имя базовой базы аналитики пользовательского интерфейса.|
|overallScore|Int32|Общая оценка базовой базы аналитики пользовательских интерфейсов.|
|isBuiltIn|Boolean|Означает, является ли текущий базовый уровень коммерческим медианым или настраиваемой базовой базой.|
|createdDateTime|DateTimeOffset|Дата создания настраиваемой базовой линии.|

## <a name="relationships"></a>Связи
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



