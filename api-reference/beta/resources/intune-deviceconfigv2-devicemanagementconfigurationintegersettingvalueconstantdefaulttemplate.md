---
title: deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate resource type
description: Стандартный шаблон параметра значение Constant Default
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9d0f4ba0fac13b7f127fe1749b598c94d981ee40
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128874"
---
# <a name="devicemanagementconfigurationintegersettingvalueconstantdefaulttemplate-resource-type"></a>deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate resource type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Стандартный шаблон параметра значение Constant Default


Наследует [от deviceManagementConfigurationIntegerSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|constantValue|Int32|Значение Constant по умолчанию. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate",
  "constantValue": 1024
}
```



