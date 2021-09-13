---
title: тип ресурса teamworkUserIdentity
description: Представляет пользователя в Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d6989f7b3c5689fefe8e9516e25fd6ff3777fe16
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128160"
---
# <a name="teamworkuseridentity-resource-type"></a>тип ресурса teamworkUserIdentity

Пространство имен: microsoft.graph

Представляет пользователя **в** Microsoft Teams.


Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Унаследованный от [удостоверения](../resources/identity.md). Отображаемое имя пользователя. Необязательное.|
|id|String|Унаследованный от [удостоверения](../resources/identity.md). ID пользователя. |
|userIdentityType|teamworkUserIdentityType| Тип пользователя. Возможные значения: `aadUser` `onPremiseAadUser` , , , , , `anonymousGuest` , `federatedUser` и `personalMicrosoftAccountUser` `skypeUser` `phoneUser` `unknownFutureValue` .|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkUserIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkUserIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "userIdentityType": "String"
}
```

