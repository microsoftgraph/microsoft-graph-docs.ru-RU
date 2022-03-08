---
title: тип ресурса logicAppAppTriggerEndpointConfiguration
description: Сведения о конфигурации конечной точки приложения логики, связанной с расширением рабочего процесса пакета пользовательского доступа.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e7f97d944d2dffa8103ca53e04fd455d515fd41e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339670"
---
# <a name="logicapptriggerendpointconfiguration-resource-type"></a>тип ресурса logicAppAppTriggerEndpointConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о конфигурации конечной точки приложения логики, связанной с расширением рабочего процесса пакета пользовательского доступа. Производный от абстрактного [типа customExtensionEndpointConfiguration](customextensionendpointconfiguration.md) .

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---| 
|logicAppWorkflowName|String|Имя приложения логики.|
|resourceGroupName|Строка|Имя группы ресурсов Azure для приложения логики.|
|subscriptionId|String|Идентификатор подписки Azure для приложения логики.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.logicAppTriggerEndpointConfiguration",
  "baseType": "microsoft.graph.customExtensionEndpointConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.logicAppTriggerEndpointConfiguration",
  "subscriptionId": "String",
  "resourceGroupName": "String",
  "logicAppWorkflowName": "String"
}
```
