---
title: Тип ресурса delegatedAdminRelationshipCustomerParticipant
description: Представляет сведения об идентификации клиента в делегированной связи администратора.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 228681c0ade8f7b0db7ad3901e402049288cefd7
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704426"
---
# <a name="delegatedadminrelationshipcustomerparticipant-resource-type"></a>Тип ресурса delegatedAdminRelationshipCustomerParticipant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об идентификации клиента в делегированной связи администратора.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя клиента клиента, задаемое Azure AD. Только чтение|
|tenantId|String|Идентификатор клиента, назначаемого Azure AD.|

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

