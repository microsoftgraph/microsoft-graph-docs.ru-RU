---
title: Тип ресурса iosLobAppProvisioningConfiguration
description: В этом разделе приведены описания объявляемых методов, свойств и связей, предоставляемых ресурсом конфигурации подготовки бизнес-приложений iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2058ec295ab48b2e7300e298ea4801c9b2baec06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527416"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a>Тип ресурса iosLobAppProvisioningConfiguration

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этом разделе приведены описания объявляемых методов, свойств и связей, предоставляемых ресурсом конфигурации подготовки бизнес-приложений iOS.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosLobAppProvisioningConfigurations](../api/intune-shared-ioslobappprovisioningconfiguration-list.md)|Коллекция [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Список свойств и связей объектов [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .|
|[Получение iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Чтение свойств и связей объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .|
|[Создание iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-create.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Создание нового объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .|
|[Удаление iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-delete.md)|Нет|Удаляет объект [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).|
|[Обновление iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Обновление свойств объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .|
|**Приложения**|
|[Действие assign](../api/intune-shared-ioslobappprovisioningconfiguration-assign.md)|Нет|Н/Д|
|**Набор политик**|
|[действие Хаспайлоадлинкс](../api/intune-shared-ioslobappprovisioningconfiguration-haspayloadlinks.md)|Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|expirationDateTime|DateTimeOffset|Дата и время необязательного окончания срока действия профиля.|
|payloadFileName|String|Имя файла полезных данных (*. мобилепровисион | *.xml).|
|payload|Binary|Полезные данные (массив байтов в кодировке UTF8).|
|roleScopeTagIds|Коллекция String|Список тегов областей для данной сущности конфигурации подготовки бизнес-приложений iOS.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|description|String|Указанное администратором описание конфигурации устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|displayName|Строка|Указанное администратором имя конфигурации устройства.|
|version|Int32|Версия конфигурации устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Приложения**|
|groupAssignments|Коллекция [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|Связанные назначения групп.|
|assignments|Коллекция [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Связанные назначения групп для IosLobAppProvisioningConfiguration.|
|deviceStatuses|Коллекция [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Список состояний установки устройств для этой конфигурации мобильного приложения.|
|userStatuses|Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Список состояний установки пользователей для этой конфигурации мобильного приложения.|

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
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



