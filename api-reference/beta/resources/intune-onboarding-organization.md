---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd8481ddea83194c7e1b769c70518c9ddff3f894
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42778017"
---
# <a name="organization-resource-type"></a>Тип ресурса organization

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список организаций](../api/intune-onboarding-organization-list.md)|Коллекция объектов [organization](../resources/intune-onboarding-organization.md)|Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).|
|[Get organization](../api/intune-onboarding-organization-get.md)|[organization](../resources/intune-onboarding-organization.md)|Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).|
|[Обновление организации](../api/intune-onboarding-organization-update.md)|[organization](../resources/intune-onboarding-organization.md)|Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).|
|[Действие setMobileDeviceManagementAuthority](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|Int32|Задание центра управления мобильными устройствами|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта.|
|mobileDeviceManagementAuthority|[мдмаусорити](../resources/intune-onboarding-mdmauthority.md)|Центр управления мобильными устройствами. Возможные значения: `unknown`, `intune`, `sccm`, `office365`.|
|цертификатеконнекторсеттинг|[цертификатеконнекторсеттинг](../resources/intune-onboarding-certificateconnectorsetting.md)|Параметр соединителя сертификатов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```



