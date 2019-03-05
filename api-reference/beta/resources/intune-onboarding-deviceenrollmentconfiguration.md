---
title: Тип ресурса deviceEnrollmentConfiguration
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d429856c8253a6c1bf47747d2c1ad481820ada9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150682"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>Тип ресурса deviceEnrollmentConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceEnrollmentConfigurations](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|Коллекция [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).|
|[Получение объекта deviceEnrollmentConfiguration](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).|
|[Действие setPriority](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|Нет|Н/Д|
|[Действие assign](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|Нет|Пока не задокументировано|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор конфигурации страницы состояния регистрации|
|displayName|String|Н/Д|
|description|String|Н/Д|
|priority|Int32|Пока не задокументировано|
|createdDateTime|DateTimeOffset|Н/Д|
|lastModifiedDateTime|DateTimeOffset|Н/Д|
|version|Int32|Пока не задокументировано|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список назначений групп для профиля конфигурации устройства.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```




