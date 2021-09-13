---
title: Тип ресурса claimsMapping
description: Сопоставление утверждений от маркера с утверждениями, которые распознает и использует Azure Active Directory B2C.
author: namkedia
ms.localizationpriority: high
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d6c37ff5ac2aa52bb6873bccb1b9bb4287641336
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109369"
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

