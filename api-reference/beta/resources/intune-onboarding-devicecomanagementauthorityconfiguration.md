---
title: Тип ресурса Девицекоманажементаусоритиконфигуратион
description: Конфигурация страницы центра Co-Management Windows 10
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c287911666880bf0d6e45dc348c36a33198aee93
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49337109"
---
# <a name="devicecomanagementauthorityconfiguration-resource-type"></a>Тип ресурса Девицекоманажементаусоритиконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация страницы центра Co-Management Windows 10


Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицекоманажементаусоритиконфигуратионс](../api/intune-onboarding-devicecomanagementauthorityconfiguration-list.md)|Коллекция [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Список свойств и связей объектов [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .|
|[Получение Девицекоманажементаусоритиконфигуратион](../api/intune-onboarding-devicecomanagementauthorityconfiguration-get.md)|[девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Чтение свойств и связей объекта [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .|
|[Создание Девицекоманажементаусоритиконфигуратион](../api/intune-onboarding-devicecomanagementauthorityconfiguration-create.md)|[девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Создание нового объекта [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .|
|[Удаление Девицекоманажементаусоритиконфигуратион](../api/intune-onboarding-devicecomanagementauthorityconfiguration-delete.md)|Нет|Удаляет объект [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).|
|[Обновление Девицекоманажементаусоритиконфигуратион](../api/intune-onboarding-devicecomanagementauthorityconfiguration-update.md)|[девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Обновление свойств объекта [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|String|Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|String|Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|Коллекция строк|Необязательные теги области применения роли для ограничений регистрации. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|манажеддевицеаусорити|Int32|Конфигурация центра управления Манажеддевицеаусорити|
|инсталлконфигуратионманажеражент|Boolean|Конфигурация центра управления Инсталлконфигуратионманажеражент|
|конфигуратионманажераженткоммандлинеаргумент|String|Конфигурация центра управления Конфигуратионманажераженткоммандлинеаргумент|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список назначений групп для профиля конфигурации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComanagementAuthorityConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ],
  "managedDeviceAuthority": 1024,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "String"
}
```




