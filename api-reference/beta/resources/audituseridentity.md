---
title: тип ресурсов auditUserIdentity
description: Открытый тип, который представляет сведения о удостоверении пользователя, а также сведения о домашнем клиенте.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fc3d4f2de96c878184d38ed3eae4bf795875e35f
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647242"
---
# <a name="audituseridentity-resource-type"></a>тип ресурсов auditUserIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Открытый тип, который представляет сведения о удостоверении пользователя, а также сведения о домашнем клиенте.

Наследуется от [userIdentity](../resources/useridentity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя пользователя. Унаследованный от [удостоверения](../resources/identity.md).|
|homeTenantId|String|Для входных входов пользователя идентификатор клиента, в который входит пользователь.|
|homeTenantName|String|Для входных входов пользователя имя клиента, членом которого является пользователь. Заполняется только в тех случаях, когда домашний клиент предоставил положительное согласие Azure AD для демонстрации контента клиента.|
|id|String|Уникальный идентификатор пользователя. Унаследованный от [удостоверения](../resources/identity.md).|
|ipAddress|String|IP-адрес Azure AD, обнаруженный для клиента пользователя. Наследуется от [userIdentity](../resources/useridentity.md).|
|userPrincipalName|String|Основное имя пользователя (UPN). Наследуется от [userIdentity](../resources/useridentity.md).|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditUserIdentity",
  "baseType": "microsoft.graph.userIdentity",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditUserIdentity",
  "displayName": "String",
  "id": "String (identifier)",
  "ipAddress": "String",
  "userPrincipalName": "String",
  "homeTenantId": "String",
  "homeTenantName": "String"
}
```

