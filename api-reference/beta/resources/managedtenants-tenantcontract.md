---
title: тип ресурса tenantContract
description: Представляет сведения о связи между клиентом и управляющей организацией.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d2531120eda65f90cd541e9f536f74733d423ec8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791871"
---
# <a name="tenantcontract-resource-type"></a>тип ресурса tenantContract

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о связи между клиентом и управляющей организацией.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contractType|Int32|Тип отношений, которые существуют между управляющей сущностью и клиентом. Необязательно. Только для чтения.|
|defaultDomainName|String|Доменное имя по умолчанию для клиента. Обязательное. Только для чтения.|
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
