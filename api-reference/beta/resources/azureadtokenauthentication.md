---
title: тип ресурса azureAdTokenAuthentication
description: Определяет приложение Azure AD, используемую для проверки подлинности с помощью расширения рабочего процесса пакета пользовательского доступа.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6e1161897cf09ae1ad25d312b8ba5ca2bdf31617
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339290"
---
# <a name="azureadtokenauthentication-resource-type"></a>тип ресурса azureAdTokenAuthentication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет приложение Azure AD, используемую для проверки подлинности логического приложения с расширением рабочего процесса пакета [пользовательского доступа](customaccesspackageworkflowextension.md). Требуется только ID приложения. Производный от [customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|resourceId|String|**AppID приложения** Azure AD для проверки подлинности логического приложения с расширением рабочего процесса пакетов пользовательского доступа.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureAdTokenAuthentication",
  "baseType": "microsoft.graph.customExtensionAuthenticationConfiguration"
}
-->

``` json
{ 
  "@odata.type": "#microsoft.graph.azureAdTokenAuthentication", 
  "resourceId": "String" 
 } 
```
