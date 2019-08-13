---
title: Тип ресурса Усерекспериенцеаналитикскатегори
description: Сущность категории аналитики взаимодействия с пользователем содержит показатели и аналитические сведения о различных метриках категории.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c04f2caaa7b9ee6c093a58e4c8123250113b3a9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329649"
---
# <a name="userexperienceanalyticscategory-resource-type"></a>Тип ресурса Усерекспериенцеаналитикскатегори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность категории аналитики взаимодействия с пользователем содержит показатели и аналитические сведения о различных метриках категории.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Усерекспериенцеаналитикскатегори](../api/intune-devices-userexperienceanalyticscategory-get.md)|[усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md)|Чтение свойств и связей объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .|
|[Обновление Усерекспериенцеаналитикскатегори](../api/intune-devices-userexperienceanalyticscategory-update.md)|[усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md)|Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор категории аналитики взаимодействия с пользователем.|
|displayName|Строка|Имя категории аналитики взаимодействия с пользователем.|
|овераллскоре|Int32|Общий показатель категории аналитики взаимодействия с пользователем.|
|insights|Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)|Аналитика для категории аналитики взаимодействия с пользователем.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|метриквалуес|Коллекция [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Значения метрик для категории аналитики взаимодействия с пользователем.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```



