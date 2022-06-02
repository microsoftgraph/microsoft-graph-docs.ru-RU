---
title: Тип ресурса userExperienceAnalyticsDeviceScope
description: Сущность области устройства аналитики пользовательского интерфейса содержит значения конфигурации области устройства, которые используются для применения фильтрации к отчетам аналитики конечных точек.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf5605a0f65dcf4e4d35026bf18d5499ab2a6c96
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858829"
---
# <a name="userexperienceanalyticsdevicescope-resource-type"></a>Тип ресурса userExperienceAnalyticsDeviceScope

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность области устройства аналитики пользовательского интерфейса содержит значения конфигурации области устройства, которые используются для применения фильтрации к отчетам аналитики конечных точек.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление userExperienceAnalyticsDeviceScopes](../api/intune-devices-userexperienceanalyticsdevicescope-list.md)|[Коллекция userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|Список свойств и связей объектов [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .|
|[Получение userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-get.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|Чтение свойств и связей объекта [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .|
|[Создание объекта userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-create.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|Создайте объект [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .|
|[Удаление userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-delete.md)|Нет|Удаляет [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md).|
|[Обновление userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-update.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|Обновление свойств объекта [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .|
|[Действие triggerDeviceScopeAction](../api/intune-devices-userexperienceanalyticsdevicescope-triggerdevicescopeaction.md)|[deviceScopeActionResult](../resources/intune-devices-devicescopeactionresult.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для конфигурации области устройства.|
|deviceScopeName|String|Имя конфигурации области устройства аналитики пользовательского интерфейса.|
|ownerId|String|Уникальный идентификатор пользователя (администратора), создавшего конфигурацию области устройства.|
|isBuiltIn|Boolean|Указывает, является ли конфигурация области устройства встроенной или пользовательской. Если значение равно TRUE, конфигурация области устройства является встроенной. Если значение равно FALSE, конфигурация области устройства является настраиваемой. Значение по умолчанию — FALSE.|
|enabled|Boolean|Указывает, включена или отключена область устройства. Если значение равно TRUE, область устройства включена. Если значение равно FALSE, область устройства отключена. Значение по умолчанию — FALSE.|
|status|[deviceScopeStatus](../resources/intune-devices-devicescopestatus.md)|Указывает состояние области устройства после включения области устройства. Возможные значения: none, computing, insufficientData или completed. Значение по умолчанию — none. Возможные значения: `none`, `computing`, `insufficientData`, `completed`, `unknownFutureValue`.|
|параметр|[deviceScopeParameter](../resources/intune-devices-devicescopeparameter.md)|Параметр конфигурации области устройства. В будущем он будет расширен для добавления дополнительных параметров. Например, параметр области устройства может быть версией ОС, типом диска, производителем устройства, моделью устройства или тегом области. Значение по умолчанию: scopeTag. Возможные значения: `none`, `scopeTag`, `unknownFutureValue`.|
|operator|[deviceScopeOperator](../resources/intune-devices-devicescopeoperator.md)|Оператор запроса конфигурации области устройства. Возможные значения: equals, notEquals, contains, notContains, greaterThan, lessThan. Значение по умолчанию: равно. Возможные значения: `none`, `equals`, `unknownFutureValue`.|
|valueObjectId|Строка|Уникальный идентификатор идентификатора тега области пользовательского устройства, используемого для создания конфигурации области устройства.|
|value|String|Значение предложения запроса конфигурации области устройства.|
|createdDateTime|DateTimeOffset|Указывает дату и время создания пользовательской области устройства.|
|lastModifiedDateTime|DateTimeOffset|Указывает дату и время последнего обновления для области пользовательского устройства.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScope",
  "id": "String (identifier)",
  "deviceScopeName": "String",
  "ownerId": "String",
  "isBuiltIn": true,
  "enabled": true,
  "status": "String",
  "parameter": "String",
  "operator": "String",
  "valueObjectId": "String",
  "value": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




