---
title: Тип ресурса Усерекспериенцеаналитиксстартупскорехистори
description: Журнал оценки запуска устройств Analytics Device (взаимодействие с пользователем).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a0be4c680485975bf1bbb338609b2cf0817ba0d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783755"
---
# <a name="userexperienceanalyticsstartupscorehistory-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксстартупскорехистори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Журнал оценки запуска устройств Analytics Device (взаимодействие с пользователем).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксстартупскорехисториес](../api/intune-devices-userexperienceanalyticsstartupscorehistory-list.md)|Коллекция [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|Список свойств и связей объектов [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .|
|[Получение Усерекспериенцеаналитиксстартупскорехистори](../api/intune-devices-userexperienceanalyticsstartupscorehistory-get.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .|
|[Создание Усерекспериенцеаналитиксстартупскорехистори](../api/intune-devices-userexperienceanalyticsstartupscorehistory-create.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|Создание нового объекта [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .|
|[Удаление Усерекспериенцеаналитиксстартупскорехистори](../api/intune-devices-userexperienceanalyticsstartupscorehistory-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md).|
|[Обновление Усерекспериенцеаналитиксстартупскорехистори](../api/intune-devices-userexperienceanalyticsstartupscorehistory-update.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|Обновление свойств объекта [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .|

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
  "@odata.type": "microsoft.graph.userExperienceAnalyticsStartupScoreHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "id": "String (identifier)",
  "startupDateTime": "String (timestamp)",
  "startupScore": 1024,
  "coreBootScore": 1024,
  "coreSigninScore": 1024,
  "recommendedSoftwareScore": 1024
}
```



