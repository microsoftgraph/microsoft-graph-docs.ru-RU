---
title: тип ресурса privateLinkDetails
description: Предоставляет сведения о частных ссылках в клиенте Azure AD
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8392b9a1a0e86a1f12a17d96c3fa7e8d06f7437b
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647253"
---
# <a name="privatelinkdetails-resource-type"></a>тип ресурса privateLinkDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о частной ссылке Azure, связанной с событием для входов. Дополнительные сведения о частной ссылке Azure см. в этой [ссылке.](/azure/private-link/private-link-overview) 



## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|policyId|String|Уникальный идентификатор для политики private Link. |
|policyName|String|Имя политики частных ссылок в Azure AD. |
|policyTenantId|String|Идентификатор клиента клиента клиента Azure AD, к котором принадлежит политика private Link.|
|resourceId|String|Путь azure Resource Manager (ARM) для ресурса политики private Link.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.privateLinkDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privateLinkDetails",
  "policyId": "String",
  "policyName": "String",
  "resourceId": "String",
  "policyTenantId": "String"
}
```
