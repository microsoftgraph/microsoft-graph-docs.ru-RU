---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad0543a521d66ed6e515afe806b583e247a75a07
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771182"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>Тип ресурса deviceEnrollmentConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый класс конфигурации регистрации устройств

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceEnrollmentConfigurations](../api/intune-shared-deviceenrollmentconfiguration-list.md)|Коллекция [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).|
|[Получение объекта deviceEnrollmentConfiguration](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).|
|**Адаптация**|
|[Действие setPriority](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|Нет|Н/Д|
|[Действие assign](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|Нет|Н/Д|
|**Набор политик**|
|[действие Хаспайлоадлинкс](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)|Пока не задокументировано|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для учетной записи|
|displayName|Строка|Отображаемое имя конфигурации регистрации устройств|
|description|String|Описание конфигурации регистрации устройств|
|priority|Int32|Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета.|
|createdDateTime|DateTimeOffset|Созданная Дата и время в формате UTC для конфигурации регистрации устройств|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения конфигурации регистрации устройств в формате UTC|
|version|Int32|Версия конфигурации регистрации устройств|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Адаптация**|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список назначений групп для профиля конфигурации устройства|

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



