---
title: Тип ресурса macOSTrustedRootCertificate
description: Профиль конфигурации OS X доверенного корневого сертификата.
ms.openlocfilehash: 11d486a2d87ecf710df73aead5ca02c924f5520b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080158"
---
# <a name="macostrustedrootcertificate-resource-type"></a>Тип ресурса macOSTrustedRootCertificate

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Профиль конфигурации OS X доверенного корневого сертификата.

Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список macOSTrustedRootCertificates](../api/intune-deviceconfig-macostrustedrootcertificate-list.md)|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) коллекции|Свойства списка и связей объектов [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .|
|[Получение macOSTrustedRootCertificate](../api/intune-deviceconfig-macostrustedrootcertificate-get.md)|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Чтение свойства и связи объекта [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .|
|[Создание macOSTrustedRootCertificate](../api/intune-deviceconfig-macostrustedrootcertificate-create.md)|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Создание нового объекта [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .|
|[Удаление macOSTrustedRootCertificate](../api/intune-deviceconfig-macostrustedrootcertificate-delete.md)|Нет|Удаляет [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).|
|[Обновление macOSTrustedRootCertificate](../api/intune-deviceconfig-macostrustedrootcertificate-update.md)|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Обновление свойства объекта [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия. Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью. Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|описание|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|trustedRootCertificate|Двоичный|Доверенного корневого сертификата.|
|certFileName|String|Имя файла для отображения в пользовательском Интерфейсе.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSTrustedRootCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "trustedRootCertificate": "binary",
  "certFileName": "String"
}
```





