---
title: Тип ресурса writebackConfiguration
description: Представляет состояние обратной записи для Azure AD облачных групп (Microsoft 365 и группы безопасности).
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 5b2dffd738684838ac0265f1f745f0071ec0aa60
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447767"
---
# <a name="writebackconfiguration-resource-type"></a>Тип ресурса writebackConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние обратной записи для Azure AD облачных групп (Microsoft 365 и группы безопасности).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включена ли обратная запись облачных групп в локальную службу Active Directory. Значение по умолчанию — `true` для групп Microsoft 365 и `false` групп безопасности.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.writebackConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.writebackConfiguration",
  "isEnabled": "Boolean"
}
```

