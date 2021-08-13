---
title: тип ресурса teamworkUserIdentity
description: Представляет пользователя в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 107ff351d17cf999fa0d2dce085587f5b2ea16edd6bf5315ded551fe78554629
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146386"
---
# <a name="teamworkuseridentity-resource-type"></a>тип ресурса teamworkUserIdentity

Пространство имен: microsoft.graph

Представляет пользователя **в** Microsoft Teams.


Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Унаследованный от [удостоверения](../resources/identity.md). Отображаемое имя пользователя. Необязательно.|
|id|String|Унаследованный от [удостоверения](../resources/identity.md). ID пользователя. |
|userIdentityType|teamworkUserIdentityType| Тип пользователя. Возможные значения: `aadUser` `onPremiseAadUser` , , , , , `anonymousGuest` , `federatedUser` и `personalMicrosoftAccountUser` `skypeUser` `phoneUser` `unknownFutureValue` .|

## <a name="relationships"></a>Связи
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

