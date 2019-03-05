---
title: Тип ресурса Виндовскиоскконфигуратион
description: Эта сущность предоставляет описания объявляемых методов, свойств и связей, предоставляемых ресурсом киоска.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 344d02c3d17c868686be75a72101b836851f0690
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143136"
---
# <a name="windowskioskconfiguration-resource-type"></a>Тип ресурса Виндовскиоскконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность предоставляет описания объявляемых методов, свойств и связей, предоставляемых ресурсом киоска.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовскиоскконфигуратионс](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|Коллекция [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md)|Список свойств и связей объектов [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) .|
|[Получение Виндовскиоскконфигуратион](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).|Чтение свойств и связей объекта [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) .|
|[Создание Виндовскиоскконфигуратион](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).|Создание нового объекта [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) .|
|[Удаление Виндовскиоскконфигуратион](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|Нет|Удаляет объект [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md).|
|[Обновление Виндовскиоскконфигуратион](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).|Обновление свойств объекта [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Киоскпрофилес|Коллекция [виндовскиоскпрофиле](../resources/intune-deviceconfig-windowskioskprofile.md)|Этот параметр политики позволяет определить список профилей киоска для конфигурации киоска. Эта коллекция может содержать не более 3 элементов.|
|Киоскбровсердефаултурл|String|Укажите URL-адрес по умолчанию, на который должен переходить браузер при запуске.|
|Киоскбровсеренаблехомебуттон|Логический|Включите кнопку Главная в браузере киоска. По умолчанию кнопка "домой" отключена.|
|Киоскбровсеренабленавигатионбуттонс|Логический|Включение кнопок навигации в браузере киосков (вперед и назад). По умолчанию кнопки навигации отключены.|
|Киоскбровсеренаблиндсессионбуттон|Логический|Включите кнопку End Session (завершить сеанс) в обозревателе киосков. По умолчанию кнопка End Session отключена.|
|Киоскбровсеррестартонидлетимеинминутес|Int32|Укажите время в минутах, в течение которого сеанс простаивает до тех пор, пока обозреватель киоска не перезапустится в обновленном состоянии.  Допустимые значения: 1-1440. Допустимые значения — от 1 до 1440|
|Киоскбровсерблоккедурлс|Коллекция строк|Указание URL-адресов, к которым не должны переходить браузеры киоска|
|Киоскбровсерблоккедурлексцептионс|Коллекция строк|Указание URL-адресов, на которые может перейти браузер с киоском|
|Еджекиоскенаблепубликбровсинг|Логический|Включение режима "общедоступный" в режиме киоска браузера для браузера Microsoft Edge. Значение по умолчанию — false.|
|Еджекиоскресетафтеридлетимеинминутес|Int32|Задает время (в минутах) от последнего действия пользователя до сброса Microsoft Edge киоска.  Допустимые значения: 0-1440. Значение по умолчанию — 5. 0 указывает на отсутствие сброса. Допустимые значения — от 0 до 1440|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
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




