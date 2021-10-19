---
title: тип ресурса deviceManagementConfigurationPolicyTemplateReference
description: Справочные сведения шаблона политики
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64bb59f9d96386260267890dbdce77c538afedcd
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60488355"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a>тип ресурса deviceManagementConfigurationPolicyTemplateReference

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Справочные сведения шаблона политики

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|templateId|String|Шаблон id|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|Семейство шаблонов ссылаемого шаблона. Это свойство доступно только для чтения. Возможные значения: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`, `baseline`.|
|templateDisplayName|String|Отображение имени шаблона ссылаемого шаблона. Это свойство доступно только для чтения.|
|templateDisplayVersion|String|Отображение шаблона версии ссылаемого шаблона. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
  "templateId": "String",
  "templateFamily": "String",
  "templateDisplayName": "String",
  "templateDisplayVersion": "String"
}
```



