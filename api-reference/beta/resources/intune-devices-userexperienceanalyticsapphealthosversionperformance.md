---
title: тип ресурса userExperienceAnalyticsAppHealthOSVersionPerformance
description: Объект для аналитики пользовательского интерфейса оси содержит сведения о производительности версии ОС.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d6d43ad592821546c9eab32c3681ae7ab9747def7fe71c18b72ef579f4c3bb28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54133217"
---
# <a name="userexperienceanalyticsapphealthosversionperformance-resource-type"></a>тип ресурса userExperienceAnalyticsAppHealthOSVersionPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект для аналитики пользовательского интерфейса оси содержит сведения о производительности версии ОС.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsAppHealthOSVersionPerformances](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-list.md)|[коллекция userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|
|[Get userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-get.md)|[userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|
|[Создание userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-create.md)|[userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Создание нового [объекта userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|
|[Удаление userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md).|
|[Обновление userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-update.md)|[userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Обновление свойств объекта [userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности версии оси для пользовательского интерфейса аналитики оси.|
|osVersion|String|Версия ОС, установленная на устройстве.|
|osBuildNumber|Строка|Номер сборки ОС, установленный на устройстве.|
|activeDeviceCount|Int32|Количество активных устройств для версии ОС. Допустимые значения 2147483648 2147483647|
|meanTimeToFailureInMinutes|Int32|Время сбоя для версии ОС в минутах. Допустимые значения 2147483648 2147483647|
|osVersionAppHealthScore|Двойное с плавающей точкой|Оценка состояния здоровья приложения в версии ОС. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|osVersionAppHealthStatus|Строка|Общее состояние состояния здоровья приложения в версии ОС.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "id": "String (identifier)",
  "osVersion": "String",
  "osBuildNumber": "String",
  "activeDeviceCount": 1024,
  "meanTimeToFailureInMinutes": 1024,
  "osVersionAppHealthScore": "4.2",
  "osVersionAppHealthStatus": "String"
}
```




