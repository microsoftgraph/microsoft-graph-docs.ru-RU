---
title: Тип ресурса Усерекспериенцеаналитиксскорехистори
description: Журнал оценки запуска устройств Analytics Device (взаимодействие с пользователем).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5b4ef00ccdab5ba6f1fab8087027e24a87e6f8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080770"
---
# <a name="userexperienceanalyticsscorehistory-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксскорехистори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Журнал оценки запуска устройств Analytics Device (взаимодействие с пользователем).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксскорехисториес](../api/intune-devices-userexperienceanalyticsscorehistory-list.md)|Коллекция [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Список свойств и связей объектов [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .|
|[Получение Усерекспериенцеаналитиксскорехистори](../api/intune-devices-userexperienceanalyticsscorehistory-get.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .|
|[Создание Усерекспериенцеаналитиксскорехистори](../api/intune-devices-userexperienceanalyticsscorehistory-create.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Создание нового объекта [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .|
|[Удаление Усерекспериенцеаналитиксскорехистори](../api/intune-devices-userexperienceanalyticsscorehistory-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md).|
|[Обновление Усерекспериенцеаналитиксскорехистори](../api/intune-devices-userexperienceanalyticsscorehistory-update.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Обновление свойств объекта [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.|
|стартупдатетиме|DateTimeOffset|Дата и время запуска устройства Analytics Device Experience.|
|стартупскоре|Int32|Оценка запуска устройства Analytics для пользователя. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.|
|коребутскоре|Int32|Оценка загрузки ядра устройств для службы аналитики взаимодействия с пользователем. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.|
|коресигнинскоре|Int32|Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.|
|рекоммендедсофтварескоре|Int32|Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.|
|рестартскоре|Int32|Оценка перезапуска. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель, 0 указывает на чрезмерные перегрузки. Допустимые значения — от 0 до 9999999|

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
  "startupScore": 1024,
  "coreBootScore": 1024,
  "coreSigninScore": 1024,
  "recommendedSoftwareScore": 1024,
  "restartScore": 1024
}
```






