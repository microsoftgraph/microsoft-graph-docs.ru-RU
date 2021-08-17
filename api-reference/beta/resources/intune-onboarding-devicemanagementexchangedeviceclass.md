---
title: тип ресурса deviceManagementExchangeDeviceClass
description: Класс устройства в Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 27f74ea0e26fc5f5371bdc864cb4da3c4730c31910b8b1ec366c571eecfa6ade
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178852"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a>тип ресурса deviceManagementExchangeDeviceClass

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс устройства в Exchange.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя класса устройства, на которое будет влиять это правило.|
|type|[deviceManagementExchangeAccessRuleType](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|Тип устройства, на которое влияет это правило, например Model, Family. Возможные значения: `family`, `model`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```




