---
title: Тип ресурса iosLobAppProvisioningConfiguration
description: В этом разделе приведены описания объявленные методы, свойства и связи, предоставляемые элементом IOS бизнес-приложения подготовки конфигурации ресурсов.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 2d91508316ab0d164fbc2d4730e905112d82ba8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965609"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a>Тип ресурса iosLobAppProvisioningConfiguration

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В этом разделе приведены описания объявленные методы, свойства и связи, предоставляемые элементом IOS бизнес-приложения подготовки конфигурации ресурсов.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosLobAppProvisioningConfigurations](../api/intune-apps-ioslobappprovisioningconfiguration-list.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) коллекции|Свойства списка и связей объектов [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .|
|[Получение iosLobAppProvisioningConfiguration](../api/intune-apps-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Чтение свойства и связи объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .|
|[Создание iosLobAppProvisioningConfiguration](../api/intune-apps-ioslobappprovisioningconfiguration-create.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Создание нового объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .|
|[Удаление iosLobAppProvisioningConfiguration](../api/intune-apps-ioslobappprovisioningconfiguration-delete.md)|Нет|Удаляет [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).|
|[Обновление iosLobAppProvisioningConfiguration](../api/intune-apps-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Обновление свойства объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .|
|[Действие assign](../api/intune-apps-ioslobappprovisioningconfiguration-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|expirationDateTime|DateTimeOffset|Необязательный профиль истечение срока действия Дата и время.|
|payloadFileName|String|Имя файла полезной нагрузки (*.mobileprovision | *.xml).|
|payload|Binary|Полезные данные (массив байтов в кодировке UTF8).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|описание|Строка|Указанное администратором описание конфигурации устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|displayName|Строка|Указанное администратором имя конфигурации устройства.|
|version|Int32|Версия конфигурации устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) коллекции|Назначения связанную группу.|
|assignments|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) коллекции|Назначения связанную группу для IosLobAppProvisioningConfiguration.|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) коллекции|Список состояния установки устройства для этой конфигурации мобильного приложения.|
|userStatuses|Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Список состояния установки пользователя для этой конфигурации мобильного приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "String (identifier)",
  "expirationDateTime": "String (timestamp)",
  "payloadFileName": "String",
  "payload": "binary",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```





