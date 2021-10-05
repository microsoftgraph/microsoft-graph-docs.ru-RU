---
title: тип ресурса azureAdJoinPolicy
description: Представляет область политики клиента, Azure Active Directory, который контролирует регистрацию устройств с помощью Azure AD Join.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a57995b3ec3228d8b7be565165667ffc39aa5338
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127940"
---
# <a name="azureadjoinpolicy-resource-type"></a>тип ресурса azureAdJoinPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет область политики клиента Azure Active Directory Azure AD, который контролирует возможность пользователей и групп регистрировать удостоверения устройств в организации с помощью Azure AD Join.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedGroups|Коллекция строк|Идентификаторы групп, которые находятся в области политики. Требуется, когда **свойство appliesTo** задает `selected` . |
|allowedUsers|Коллекция строк|Идентификаторы пользователей, которые находятся в области политики. Требуется, когда **свойство appliesTo** задает `selected` .|
|appliesTo|policyScope|Указывает, следует ли блокировать или разрешить мелкозернистый контроль области политики. Возможные значения: `0` `none` (значение), `1` `all` (значение), `2` `selected` (значение), `3` `unknownFutureValue` (значение). <br/><br/>Значение по умолчанию — `1`. При задании по крайней мере один идентификатор пользователя или группы должен быть указан в `2` **allowedUsers** или **allowedGroups.**  Настройка этого свойства для удаления всех идентификаторов как `0` `1` в **allowedUsers,** так **и в allowedGroups.**|
|isAdminConfigurable|Логическое|Указывает, настраивается ли эта область политики администратором. Значение по умолчанию `false` . Если администратор включил intune (MEM) для управления устройствами, это свойство заданной и применяется По умолчанию `false`  `1` `all` (значение).|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureAdJoinPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureAdJoinPolicy",
  "appliesTo": "String",
  "isAdminConfigurable": "Boolean",
  "allowedUsers": [
    "String"
  ],
  "allowedGroups": [
    "String"
  ]
}
```
