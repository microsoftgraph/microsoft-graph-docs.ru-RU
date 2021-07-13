---
title: тип ресурса tenantContract
description: Представляет сведения о связи между клиентом и управляющей организацией.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 104b475428efe82a2e56f823845b933149aeab18
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402699"
---
# <a name="tenantcontract-resource-type"></a>тип ресурса tenantContract

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о связи между клиентом и управляющей организацией.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contractType|Int32|Тип отношений, которые существуют между управляющей сущностью и клиентом. Необязательно. Только для чтения.|
|defaultDomainName|String|Доменное имя по умолчанию для клиента. Обязательный. Только для чтения.|
|displayName|String|Отображаемое имя для клиента. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContract"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContract",
  "contractType": "Integer",
  "displayName": "String",
  "defaultDomainName": "String"
}
```
