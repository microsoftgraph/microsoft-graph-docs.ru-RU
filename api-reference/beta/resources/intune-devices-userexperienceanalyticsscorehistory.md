---
title: тип ресурса userExperienceAnalyticsScoreHistory
description: История оценки результатов запуска устройства для аналитики пользовательского интерфейса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f82ebe1a22f42829049cc4e855e96249f6ec7ae
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/04/2022
ms.locfileid: "61711902"
---
# <a name="userexperienceanalyticsscorehistory-resource-type"></a>тип ресурса userExperienceAnalyticsScoreHistory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

История оценки результатов запуска устройства для аналитики пользовательского интерфейса.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsScoreHistories](../api/intune-devices-userexperienceanalyticsscorehistory-list.md)|[коллекция userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Список свойств и связей [объектов userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|
|[Get userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-get.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Чтение свойств и связей [объекта userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|
|[Создание userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-create.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Создание нового [объекта userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|
|[Удаление userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).|
|[Обновление userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-update.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Обновление свойств объекта [userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.|
|startupDateTime|DateTimeOffset|Время запуска устройства аналитики пользовательского интерфейса.|
|overallScore|Int32|Общая оценка аналитики пользовательского опыта. Оценка будет в диапазоне 0-100, 100 является идеальным показателем. Допустимые значения: от 0 до 100|
|startupScore|Int32|Оценка запуска устройства аналитики пользовательских интерфейсов. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|coreBootScore|Int32|Оценка загрузки основного загрузочного устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|coreSigninScore|Int32|Оценка основного входного знака устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|recommendedSoftwareScore|Int32|Оценка основного входного знака устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|appHealthOverallScore|Int32|Общее состояние здоровья приложения для аналитики пользовательского интерфейса.|
|workFromAnywhereScore|Int32|Аналитика пользовательских интерфейсов работает из любой точки.|
|batteryHealthScore|Int32|Оценка состояния заряда батареи для аналитики пользовательского интерфейса.|
|startupTotalDevices|Int32|Общее число устройств для производительности запуска для аналитики пользовательских интерфейсов.|
|recommendedSoftwareTotalDevices|Int32|Общее число устройств категории аналитики пользовательских интерфейсов рекомендуемого программного обеспечения.|
|appHealthTotalDevices|Int32|Общее число устройств для здоровья приложения для аналитики пользовательского интерфейса.|
|workFromAnywhereTotalDevices|Int32|Общее число устройств категории аналитики пользовательских интерфейсов работает из любой точки мира.|
|batteryHealthTotalDevices|Int32|Общее число устройств для здоровья батареи категории аналитики пользовательских интерфейсов.|
|restartScore|Int32|Оценка перезапуска. Оценка будет в диапазоне 0-100, 100 является идеальным показателем, 0 указывает на чрезмерные перезапуски. Допустимые значения от 0 до 9999999|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsScoreHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "String (identifier)",
  "startupDateTime": "String (timestamp)",
  "overallScore": 1024,
  "startupScore": 1024,
  "coreBootScore": 1024,
  "coreSigninScore": 1024,
  "recommendedSoftwareScore": 1024,
  "appHealthOverallScore": 1024,
  "workFromAnywhereScore": 1024,
  "batteryHealthScore": 1024,
  "startupTotalDevices": 1024,
  "recommendedSoftwareTotalDevices": 1024,
  "appHealthTotalDevices": 1024,
  "workFromAnywhereTotalDevices": 1024,
  "batteryHealthTotalDevices": 1024,
  "restartScore": 1024
}
```




