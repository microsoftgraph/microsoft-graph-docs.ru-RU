---
title: Тип ресурса Усерекспериенцеаналитиксскорехистори
description: Журнал оценки запуска устройств Analytics Device (взаимодействие с пользователем).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52154b802c1162d860b9354a7910b68d0582e6ce
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401901"
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
|id|String|Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.|
|стартупдатетиме|DateTimeOffset|Дата и время запуска устройства Analytics Device Experience.|
|стартупскоре|Int32|Оценка запуска устройства Analytics для пользователя.|
|коребутскоре|Int32|Оценка загрузки ядра устройств для службы аналитики взаимодействия с пользователем.|
|коресигнинскоре|Int32|Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом.|
|рекоммендедсофтварескоре|Int32|Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом.|

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
  "recommendedSoftwareScore": 1024
}
```



