---
title: Тип ресурса claimsMapping
description: Сопоставление утверждений от маркера с утверждениями, которые распознает и использует Azure Active Directory B2C.
author: namkedia
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 07e2d7a008db5377869d12d426d8d3d1e440a40c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534122"
---
# <a name="claimsmapping-resource-type"></a>Тип ресурса claimsMapping
Пространство имен: microsoft.graph

После того как поставщик настраиваемых удостоверений отправит маркер идентификатора обратно в службу Azure AD B2C, Azure AD B2C сопоставляет утверждения от маркера с утверждениями, которые распознает и использует Azure AD B2C.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:-------|:---|:----------|
|userId|String|Утверждение, предоставляющее уникальный идентификатор для вошедшего пользователя. Обязательно.|
|displayName|String|Утверждение, предоставляющее отображаемое или полное имя для пользователя. Обязательно.|
|givenName|String|Утверждение, предоставляющее имя пользователя.|
|surname|String|Утверждение, предоставляющее фамилию пользователя.|
|email|String|Утверждение, предоставляющее электронный адрес пользователя.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.claimsMapping"
}
-->

``` json
{
  "userId": "String",
  "givenName": "String",
  "surname": "String",
  "email": "String",
  "displayName": "String"
  }
```

