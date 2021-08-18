---
title: тип ресурса userExperienceAnalyticsRegressionSummary
description: Сводка регрессии для аналитики пользовательского интерфейса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: abd322dd8894bb35eefdf461e880ab109233acc8b114100adf9ecc369298a0d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54156116"
---
# <a name="userexperienceanalyticsregressionsummary-resource-type"></a>тип ресурса userExperienceAnalyticsRegressionSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка регрессии для аналитики пользовательского интерфейса.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-get.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Чтение свойств и связей [объекта userExperienceAnalyticsRegressionSummary.](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|
|[Обновление userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-update.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Обновление свойств объекта [userExperienceAnalyticsRegressionSummary.](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|
|[summarizeDeviceRegressionPerformance function](../api/intune-devices-userexperienceanalyticsregressionsummary-summarizedeviceregressionperformance.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор сводки регрессии аналитики пользовательского интерфейса.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|modelRegression|[коллекция userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Метрические значения для регрессии модели аналитики пользовательского опыта.|
|manufacturerRegression|[коллекция userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Метрические значения для регрессии производителя аналитики пользовательского интерфейса.|
|operatingSystemRegression|[коллекция userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Метрические значения для регрессии операционной системы аналитики пользовательского опыта.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "String (identifier)"
}
```




