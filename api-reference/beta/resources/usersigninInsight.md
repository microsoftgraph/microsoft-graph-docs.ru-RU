---
title: тип ресурса userSignInInsight
description: В отзывах о доступе к Azure AD ресурс userSignInInsight представляет сведения, предоставляемые рецензентам в зависимости от последней даты и времени регистрации пользователя.
author: shubhamguptacal
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ca84ef57b6bb2431210ab3a6a91e80b7089d86bf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112555"
---
# <a name="usersignininsight-resource-type"></a>тип ресурса usersignininsight

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет сведения, предоставляемые рецензентам в зависимости от последней даты и времени регистрации пользователя.

Наследует от [governanceInsight](governanceinsight.md).

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание |
| :---------------| :---------- | :---------- |
| lastSignInDateTime | DateTimeOffset | Указывает, когда пользователь последний раз вписывался в |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSignInInsight",
  "baseType": "microsoft.graph.governanceInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSignInInsight",
  "lastSignInDateTime": "DateTimeOffset"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "usersignininsight resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
