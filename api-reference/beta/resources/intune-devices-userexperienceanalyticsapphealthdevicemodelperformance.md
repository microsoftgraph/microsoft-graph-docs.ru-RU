---
title: тип ресурса userExperienceAnalyticsAppHealthDeviceModelPerformance
description: Объект производительности модели модели пользовательского интерфейса содержит сведения о производительности модели устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: acc48d4f29b7030ae9c8e49fb5ea17be3d995601
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790131"
---
# <a name="userexperienceanalyticsapphealthdevicemodelperformance-resource-type"></a>тип ресурса userExperienceAnalyticsAppHealthDeviceModelPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности модели модели пользовательского интерфейса содержит сведения о производительности модели устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsAppHealthDeviceModelPerformances](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-list.md)|[коллекция userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|
|[Get userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-get.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|
|[Создание userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-create.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Создайте новый [объект userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|
|[Удаление userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).|
|[Обновление userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-update.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Обновление свойств объекта [userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности модели пользовательского интерфейса для аналитики устройств.|
|deviceModel|String|Имя модели устройства.|
|deviceManufacturer|Строка|Имя производителя устройства.|
|activeDeviceCount|Int32|Количество активных устройств для модели. Допустимые значения 2147483648 2147483647|
|meanTimeToFailureInMinutes|Int32|Время сбоя для устройства модели в минутах. Допустимые значения 2147483648 2147483647|
|modelAppHealthScore|Двойное с плавающей точкой|Оценка состояния здоровья приложения модели устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|modelAppHealthStatus|Строка|Общее состояние состояния здоровья приложения модели устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "id": "String (identifier)",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "activeDeviceCount": 1024,
  "meanTimeToFailureInMinutes": 1024,
  "modelAppHealthScore": "4.2",
  "modelAppHealthStatus": "String"
}
```



