---
title: тип ресурса teamworkDeviceConfiguration
description: Представляет сведения о конфигурации для Microsoft Teams устройства с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d913040b86bbb1b2e669bbbcb0d622326603ef5
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262584"
---
# <a name="teamworkdeviceconfiguration-resource-type"></a>тип ресурса teamworkDeviceConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации для устройства с [Microsoft Teams, включая](../resources/teamworkdevice.md) версии программного обеспечения, конфигурацию периферийных устройств (например, камеру, дисплей, микрофон и динамик), конфигурацию оборудования и конфигурацию Teams клиента.


Наследуется [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get teamworkDeviceConfiguration](../api/teamworkdeviceconfiguration-get.md)|[teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md)|Ознакомьтесь с свойствами и отношениями объекта [teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|cameraConfiguration|[teamworkCameraConfiguration](../resources/teamworkcameraconfiguration.md)|Конфигурация камеры. Применимо только для Комнаты Microsoft Teams устройств с включенной поддержкой.|
|createdBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, создавшего документ конфигурации устройства.|
|createdDateTime|DateTimeOffset|Дата и время создания документа конфигурации устройства.|
|displayConfiguration|[teamworkDisplayConfiguration](../resources/teamworkdisplayconfiguration.md)|Конфигурация дисплея.|
|hardwareConfiguration|[teamworkHardwareConfiguration](../resources/teamworkhardwareconfiguration.md)|Конфигурация оборудования. Применимо только для Комнаты Teams устройств с включенной поддержкой.|
|id|String|Идентификатор документа. Наследуется [от сущности](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, который в последний раз менял конфигурацию устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения конфигурации устройства.|
|microphoneConfiguration|[teamworkMicrophoneConfiguration](../resources/teamworkmicrophoneconfiguration.md)|Конфигурация микрофона. Применимо только для Комнаты Teams устройств с включенной поддержкой.|
|softwareVersions|[teamworkDeviceSoftwareVersions](../resources/teamworkdevicesoftwareversions.md)|Сведения, связанные с версиями программного обеспечения для устройства, такими как прошивка, операционная система, Teams клиента и агента администрирования.|
|speakerConfiguration|[teamworkSpeakerConfiguration](../resources/teamworkspeakerconfiguration.md)|Конфигурация динамика. Применимо только для Комнаты Teams устройств с включенной поддержкой.|
|systemConfiguration|[teamworkSystemConfiguration](../resources/teamworksystemconfiguration.md)|Конфигурация системы. Не применяется для Комнаты Teams устройств с включенной поддержкой.|
|teamsClientConfiguration|[teamworkTeamsClientConfiguration](../resources/teamworkteamsclientconfiguration.md)|Конфигурация Teams клиента. Применимо только для Комнаты Teams устройств с включенной поддержкой.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceConfiguration",
  "cameraConfiguration": {
    "@odata.type": "microsoft.graph.teamworkCameraConfiguration"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "displayConfiguration": {
    "@odata.type": "microsoft.graph.teamworkDisplayConfiguration"
  },
  "hardwareConfiguration": {
    "@odata.type": "microsoft.graph.teamworkHardwareConfiguration"
  },
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "microphoneConfiguration": {
    "@odata.type": "microsoft.graph.teamworkMicrophoneConfiguration"
  },
  "softwareVersions": {
    "@odata.type": "microsoft.graph.teamworkDeviceSoftwareVersions"
  },
  "speakerConfiguration": {
    "@odata.type": "microsoft.graph.teamworkSpeakerConfiguration"
  },
  "systemConfiguration": {
    "@odata.type": "microsoft.graph.teamworkSystemConfiguration"
  },
  "teamsClientConfiguration": {
    "@odata.type": "microsoft.graph.teamworkTeamsClientConfiguration"
  }
}
```

