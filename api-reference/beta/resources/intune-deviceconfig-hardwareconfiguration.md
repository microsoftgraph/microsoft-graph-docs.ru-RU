---
title: тип ресурса hardwareConfiguration
description: Intune предоставит клиенту возможность настраивать параметры оборудования и биосов на зарегистрированных устройствах windows 10 Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 895ee4740b588c96fbd10c1b62821ab68e29b54d
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290947"
---
# <a name="hardwareconfiguration-resource-type"></a>тип ресурса hardwareConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность настраивать параметры оборудования и биосов на зарегистрированных устройствах windows 10 Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список аппаратныхконфигураций](../api/intune-deviceconfig-hardwareconfiguration-list.md)|[коллекция hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Список свойств и связей [объектов hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .|
|[Get hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-get.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Чтение свойств и связей [объекта hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .|
|[Создание hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-create.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Создание нового [объекта hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .|
|[Удаление hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-delete.md)|Нет|Удаляет [аппаратнуюконфигурацию](../resources/intune-deviceconfig-hardwareconfiguration.md).|
|[Обновление оборудованияКонфигурация](../api/intune-deviceconfig-hardwareconfiguration-update.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Обновление свойств объекта [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .|
|[назначение действияHardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-assignhardwareconfiguration.md)|[коллекция hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Н/Д|
|[Действие assign](../api/intune-deviceconfig-hardwareconfiguration-assign.md)|[коллекция hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор конфигурации оборудования|
|version|Int32|Версия конфигурации оборудования (например. 1, 2, 3 ...)|
|displayName|String|Имя конфигурации оборудования|
|description|String|Описание конфигурации оборудования|
|createdDateTime|DateTimeOffset|Время создания конфигурации оборудования. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Время изменения конфигурации оборудования. Это свойство доступно только для чтения.|
|fileName|String|Имя файла конфигурации оборудования|
|configurationFileContent|Binary|Содержимое файла конфигурации оборудования|
|hardwareConfigurationFormat|[hardwareConfigurationFormat](../resources/intune-deviceconfig-hardwareconfigurationformat.md)|Тип Oem конфигурации оборудования (например. DELL, HP, Surface и SurfaceDock). Возможные значения: `dell`, `surface`, `surfaceDock`.|
|roleScopeTagIds|Коллекция String|Список ID-тегов области для конфигурации оборудования|
|perDevicePasswordDisabled|Логическое|Значение, указывающее, отключен ли каждый devcive pasword|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Список ids группы пользователей Azure AD, к которые будет применена конфигурация оборудования. Поддерживаются только группы безопасности и Office 365 группы.|
|runSummary|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|Сводка результатов попытки настройки параметров оборудования|
|deviceRunStates|[коллекция hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Список состояния запуска для конфигурации оборудования на всех устройствах|
|userRunStates|[коллекция hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Список состояния запуска для конфигурации оборудования для всех пользователей|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfiguration",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "fileName": "String",
  "configurationFileContent": "binary",
  "hardwareConfigurationFormat": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "perDevicePasswordDisabled": true
}
```




