---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3f4095db44b1b32c3c1adb5792dab99167909c41
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792556"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>Тип ресурса deviceEnrollmentConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|[действие hasPayloadLinks](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор учетной записи|
|displayName|String|Отображающее имя конфигурации регистрации устройства|
|description|Строка|Описание конфигурации регистрации устройства|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета.|
|createdDateTime|DateTimeOffset|Создано время даты в UTC конфигурации регистрации устройства|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время даты в UTC конфигурации регистрации устройства|
|version|Int32|Версия конфигурации регистрации устройства|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Адаптация**|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список групповых назначений для профиля конфигурации устройства|

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



