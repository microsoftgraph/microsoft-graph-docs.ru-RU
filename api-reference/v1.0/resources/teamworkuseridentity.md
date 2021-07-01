---
title: тип ресурса teamworkUserIdentity
description: Представляет пользователя в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ae7655a5b2c84cc01d354d32d25eb724d5f4a6c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211131"
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

