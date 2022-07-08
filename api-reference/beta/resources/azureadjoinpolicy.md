---
title: Тип ресурса azureAdJoinPolicy
description: Представляет область политики клиента Azure Active Directory, который управляет регистрацией устройств с помощью Azure AD Join.
author: myra-ramdenbourg
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 46abc16a3982f7f9d22881f02cf13225d1daadcf
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66689981"
---
# <a name="azureadjoinpolicy-resource-type"></a>Тип ресурса azureAdJoinPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет область политики клиента Azure Active Directory (Azure AD), которая управляет возможностью пользователей и групп регистрировать удостоверения устройств в организации с помощью Azure AD Join.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedGroups|Коллекция объектов string|Идентификаторы групп, которые находятся в области действия политики. Требуется, если **свойству appliesTo** задано значение `selected`. |
|allowedUsers|Коллекция объектов string|Идентификаторы пользователей, которые находятся в области действия политики. Требуется, если **свойству appliesTo** задано значение `selected`.|
|appliesTo|policyScope|Указывает, следует ли блокировать или разрешать детальное управление областью политики. Возможные значения: `0` (то есть `none`), `1` (то есть `all`), `2` (то есть `selected`), `3` (то есть `unknownFutureValue`). <br/><br/>Значение по умолчанию — `1`. Если задано значение `2`,в **allowedUsers** или **allowedGroups** должен быть указан по крайней мере один идентификатор пользователя или группы.  Установка или удаление `0` всех `1` идентификаторов в **allowedUsers** и **allowedGroups**.|
|isAdminConfigurable|Логическое|Указывает, настраивается ли администратором эта область политики. Значение по умолчанию — `false`.. Если администратор включил Intune (MEM) для управления устройствами, `false` это свойство устанавливается и применяется **к** `1` значениям по умолчанию (т. е. ).`all`|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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
