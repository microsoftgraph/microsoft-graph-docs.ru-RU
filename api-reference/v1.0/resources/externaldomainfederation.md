---
title: тип ресурса externalDomainFederation
description: Тип externalDomainFederation определяет домен, не нанимаемый клиентом, с настроенным поставщиком удостоверений в качестве источника удостоверений для связанной организации.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: af47b7516e656ad85cbe1f8ef2fde3f0681ee89c
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242758"
---
# <a name="externaldomainfederation-resource-type"></a>тип ресурса externalDomainFederation

Пространство имен: microsoft.graph


Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md) Значение указывает, что этот тип определяет домен с настроенным поставщиком удостоверений в качестве источника удостоверений `@odata.type` `#microsoft.graph.externalDomainFederation` для связанной организации.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя источника удостоверений, как правило, также доменное имя. Только для чтения. |
|domainName|String|Доменное имя. Только для чтения. |
|issuerUri|Строка|IssuerURI входящих федераций. Только для чтения. |

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalDomainFederation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalDomainFederation",
  "issuerUri": "String",
  "domainName": "String",
  "displayName": "String"
}
```


