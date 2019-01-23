---
title: Тип ресурса androidTrustedRootCertificate
description: Android профиля конфигурации доверенного корневого сертификата
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 31f6b04a603516943ee62a6ae1b86c9cd70424b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399376"
---
# <a name="androidtrustedrootcertificate-resource-type"></a>Тип ресурса androidTrustedRootCertificate

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Android профиля конфигурации доверенного корневого сертификата


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidTrustedRootCertificates](../api/intune-deviceconfig-androidtrustedrootcertificate-list.md)|[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) коллекции|Свойства списка и связей объектов [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .|
|[Получение androidTrustedRootCertificate](../api/intune-deviceconfig-androidtrustedrootcertificate-get.md)|[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)|Чтение свойства и связи объекта [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .|
|[Создание androidTrustedRootCertificate](../api/intune-deviceconfig-androidtrustedrootcertificate-create.md)|[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)|Создание нового объекта [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .|
|[Удаление androidTrustedRootCertificate](../api/intune-deviceconfig-androidtrustedrootcertificate-delete.md)|Нет|Удаляет [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md).|
|[Обновление androidTrustedRootCertificate](../api/intune-deviceconfig-androidtrustedrootcertificate-update.md)|[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)|Обновление свойства объекта [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия. Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью. Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|trustedRootCertificate|Binary|Доверенный корневой сертификат|
|certFileName|String|Имя файла для отображения в пользовательском Интерфейсе.|

## <a name="relationships"></a>Отношения
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
  "@odata.type": "microsoft.graph.androidTrustedRootCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
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




