---
title: Тип ресурса windowsKioskConfiguration
description: Этот объект содержит описания объявленные методы, свойства и связи, предоставляемые элементом киоска ресурсов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f091d9700721a1be1baf5982b0fb8ce0fe3b00ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403961"
---
# <a name="windowskioskconfiguration-resource-type"></a>Тип ресурса windowsKioskConfiguration

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Этот объект содержит описания объявленные методы, свойства и связи, предоставляемые элементом киоска ресурсов.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsKioskConfigurations](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) коллекции|Свойства списка и связей объектов [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .|
|[Получение windowsKioskConfiguration](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).|Чтение свойства и связи объекта [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .|
|[Создание windowsKioskConfiguration](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).|Создание нового объекта [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .|
|[Удаление windowsKioskConfiguration](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|Нет|Удаляет [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).|
|[Обновление windowsKioskConfiguration](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).|Обновление свойства объекта [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .|

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
|kioskProfiles|[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) коллекции|Этот параметр политики позволяет определить список профилей киоска для базовой конфигурации. В этом семействе может содержать не более 3 элементы.|
|kioskBrowserDefaultUrl|String|Укажите URL-адрес по умолчанию, должен перейти браузер при запуске.|
|kioskBrowserEnableHomeButton|Логический|Кнопка браузера киоска Домашняя страница. По умолчанию домашняя страница кнопка отключена.|
|kioskBrowserEnableNavigationButtons|Логический|Включите buttons(forward/back) навигации киоска браузера. По умолчанию отключены кнопки перехода.|
|kioskBrowserEnableEndSessionButton|Логический|Кнопка браузера киоска окончания сеанса. По умолчанию отключена кнопка окончания сеанса.|
|kioskBrowserRestartOnIdleTimeInMinutes|Int32|Укажите время в минутах, сеанс находится в состоянии простоя до перезапуска браузера киоска новым состояние.  Допустимые значения: 1-1440. Допустимые значения 1 до 1440|
|kioskBrowserBlockedURLs|Коллекция String|Укажите URL-адреса, не должен перейти киоска браузеры|
|kioskBrowserBlockedUrlExceptions|Коллекция String|Укажите URL-адресов, которые может киоска браузера перейдите на|
|edgeKioskEnablePublicBrowsing|Логический|Включение общей обзора полноэкранном режиме для браузера Microsoft пограничного сервера. Значение по умолчанию — false.|
|edgeKioskResetAfterIdleTimeInMinutes|Int32|Задает время в минутах из последнего действия пользователя перед базовая Подписка пограничного сервера Microsoft восстанавливаются значения по умолчанию.  Допустимые значения: 0-1440. Значение по умолчанию равно 5. 0 указывает не reset. Допустимые значения 0 до 1440|

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
  "@odata.type": "microsoft.graph.windowsKioskConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "String",
      "profileName": "String",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "String",
            "name": "String",
            "appType": "String",
            "appUserModelId": "String",
            "appId": "String",
            "containedAppId": "String"
          }
        ],
        "showTaskBar": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "binary"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "String",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 1024,
  "kioskBrowserBlockedURLs": [
    "String"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "String"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "edgeKioskResetAfterIdleTimeInMinutes": 1024
}
```




