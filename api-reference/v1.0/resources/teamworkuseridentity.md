---
title: Тип ресурса teamworkUserIdentity
description: Представляет пользователя в Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 86b827be0a7d947a627f41f97b4002b7406006ca
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917614"
---
# <a name="teamworkuseridentity-resource-type"></a>Тип ресурса teamworkUserIdentity

Пространство имен: microsoft.graph

Представляет пользователя **в Microsoft Teams**.


Наследуется от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Наследуется от [удостоверения](../resources/identity.md). Отображаемое имя пользователя. Необязательное свойство.|
|id|String|Наследуется от [удостоверения](../resources/identity.md). Идентификатор пользователя. |
|userIdentityType|teamworkUserIdentityType| Тип пользователя. Возможные значения: `aadUser`, , `onPremiseAadUser`, `anonymousGuest`, `federatedUser`, `personalMicrosoftAccountUser`, `skypeUser`, и `unknownFutureValue` `phoneUser``emailUser`.|

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

