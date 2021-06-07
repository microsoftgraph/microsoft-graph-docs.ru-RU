---
title: Тип ресурса deviceAppManagement
description: Единичный объект управления приложениями на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8906e96a0218360bbe78d1c08dd4d8767568775
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752053"
---
# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Единичный объект управления приложениями на устройствах.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedAppPolicies|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Политики управляемых приложений.|
|iosManagedAppProtections|Коллекция [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Политики управляемых приложений для iOS.|
|androidManagedAppProtections|Коллекция [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|Политики управляемых приложений для Android.|
|defaultManagedAppProtections|Коллекция [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Политики управляемых приложений по умолчанию.|
|targetedManagedAppConfigurations|Коллекция [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Целевые конфигурации управляемых приложений.|
|mdmWindowsInformationProtectionPolicies|Коллекция [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, зарегистрированных с использованием MDM.|
|windowsInformationProtectionPolicies|Коллекция [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, не зарегистрированных с использованием MDM.|
|managedAppRegistrations|Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Регистрации управляемых приложений.|
|managedAppStatuses|Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)|Состояния управляемых приложений.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




