---
title: тип ресурса hardwareConfiguration
description: Intune предоставит клиенту возможность настраивать параметры оборудования и биосов на зарегистрированных устройствах windows 10 Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d19f8f3b8efc3d60fb60bce18851a072a50d8895
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345625"
---
# <a name="hardwareconfiguration-resource-type"></a>тип ресурса hardwareConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность настраивать параметры оборудования и биосов на зарегистрированных устройствах windows 10 Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список аппаратныхконфигураций](../api/intune-deviceconfig-hardwareconfiguration-list.md)|[коллекция hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Список свойств и связей [объектов hardwareConfiguration.](../resources/intune-deviceconfig-hardwareconfiguration.md)|
|[Get hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-get.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Чтение свойств и связей [объекта hardwareConfiguration.](../resources/intune-deviceconfig-hardwareconfiguration.md)|
|[Создание hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-create.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Создание нового [объекта hardwareConfiguration.](../resources/intune-deviceconfig-hardwareconfiguration.md)|
|[Удаление hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-delete.md)|Нет|Удаляет [аппаратнуюконфигурацию.](../resources/intune-deviceconfig-hardwareconfiguration.md)|
|[Обновление оборудованияКонфигурация](../api/intune-deviceconfig-hardwareconfiguration-update.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Обновление свойств объекта [hardwareConfiguration.](../resources/intune-deviceconfig-hardwareconfiguration.md)|
|[Действие assign](../api/intune-deviceconfig-hardwareconfiguration-assign.md)|[коллекция hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор конфигурации оборудования|
|version|Int32|Версия конфигурации оборудования|
|displayName|String|Имя конфигурации оборудования|
|description|Строка|Описание конфигурации оборудования|
|createdDateTime|DateTimeOffset|Время создания конфигурации оборудования. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Время изменения конфигурации оборудования. Это свойство доступно только для чтения.|
|fileName|String|Имя файла конфигурации оборудования|
|configurationFileContent|Binary|Содержимое файла конфигурации оборудования|
|hardwareConfigurationFormat|[hardwareConfigurationFormat](../resources/intune-deviceconfig-hardwareconfigurationformat.md)|Тип Oem конфигурации оборудования. Возможные значения: `dell`, `surface`, `surfaceDock`.|
|roleScopeTagIds|Коллекция String|Список ID-тегов области для конфигурации оборудования|
|perDevicePasswordDisabled|Boolean|Значение, указывающее, отключен ли каждый devcive pasword|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Список групповых назначений для конфигурации оборудования|
|runSummary|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|Запуск сводки для конфигурации оборудования|
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




