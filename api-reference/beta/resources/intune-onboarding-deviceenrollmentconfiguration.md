---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34b62ec6a00e47ed307951a881e247e0914b5c0b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998291"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>Тип ресурса deviceEnrollmentConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый класс конфигурации регистрации устройств

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
|id|String|Уникальный идентификатор для учетной записи|
|displayName|Строка|Отображаемое имя конфигурации регистрации устройств|
|description|String|Описание конфигурации регистрации устройств|
|priority|Int32|Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета.|
|createdDateTime|DateTimeOffset|Созданная Дата и время в формате UTC для конфигурации регистрации устройств|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения конфигурации регистрации устройств в формате UTC|
|version|Int32|Версия конфигурации регистрации устройств|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
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





