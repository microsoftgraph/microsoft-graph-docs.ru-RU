---
title: тип ресурса iosLobAppProvisioningConfiguration
description: В этом разделе описаны объявленные методы, свойства и связи, открытые ресурсом конфигурации приложений iOS Lob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c3745089ff34bc4bb0554b7e9364e112a11ab31
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472358"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a>тип ресурса iosLobAppProvisioningConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этом разделе описаны объявленные методы, свойства и связи, открытые ресурсом конфигурации приложений iOS Lob.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosLobAppProvisioningConfigurations](../api/intune-shared-ioslobappprovisioningconfiguration-list.md)|[коллекция iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Список свойств и связей объектов [iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|
|[Get iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Чтение свойств и связей объекта [iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|
|[Создание iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-create.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Создайте новый [объект iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|
|[Удаление iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-delete.md)|Нет|Удаляет [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).|
|[Обновление iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Обновление свойств объекта [iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|
|**Приложения**|
|[Действие assign](../api/intune-shared-ioslobappprovisioningconfiguration-assign.md)|Нет|Н/Д|
|**Набор политик**|
|[действие hasPayloadLinks](../api/intune-shared-ioslobappprovisioningconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|expirationDateTime|DateTimeOffset|Необязательный срок действия профиля.|
|payloadFileName|String|Имя файла полезной нагрузки (*.mobileprovision \| *.xml).|
|payload|Binary|Полезные данные (массив байтов в кодировке UTF8).|
|roleScopeTagIds|Коллекция строк|Список тегов области для этого объекта конфигурации конфигурации приложения iOS LOB.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|description|String|Указанное администратором описание конфигурации устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|displayName|String|Указанное администратором имя конфигурации устройства.|
|version|Int32|Версия конфигурации устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Приложения**|
|groupAssignments|[коллекция mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|Связанные групповые назначения.|
|assignments|[коллекция iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Связанные групповые назначения для IosLobAppProvisioningConfiguration.|
|deviceStatuses|[коллекция managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Список состояния установки устройства для этой конфигурации мобильного приложения.|
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




