---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fbab98a859128ab2700888ca0671b7551d50346e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079188"
---
# <a name="organization-resource-type"></a>Тип ресурса organization

Пространство имен: microsoft.graph

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
|id|Строка|GUID объекта.|
|mobileDeviceManagementAuthority|[мдмаусорити](../resources/intune-onboarding-mdmauthority.md)|Центр управления мобильными устройствами. Возможные значения: `unknown`, `intune`, `sccm`, `office365`.|

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
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->









