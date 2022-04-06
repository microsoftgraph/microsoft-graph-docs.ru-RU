---
title: delegatedAdminRelationshipCustomerParticipant resource type
description: Представляет сведения об идентификации клиента в делегированной связи администратора.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 738ae13f0a999cecc7d1b24bb5ef2fec81302441
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589791"
---
# <a name="delegatedadminrelationshipcustomerparticipant-resource-type"></a>delegatedAdminRelationshipCustomerParticipant resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об идентификации клиента в делегированной связи администратора.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображает имя клиента клиента в качестве задатого Azure AD. Только чтение|
|tenantId|String|ID клиента, назначенного Azure AD, клиентского клиента.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipCustomerParticipant"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipCustomerParticipant",
  "tenantId": "String",
  "displayName": "String"
}
```

