---
title: Тип ресурса claimsMapping
description: Сопоставление утверждений от маркера с утверждениями, которые распознает и использует Azure Active Directory B2C.
author: namkedia
ms.localizationpriority: high
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3862cf564ce5df1924972e75dfb22a3ba0756429
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696213"
---
# <a name="claimsmapping-resource-type"></a>Тип ресурса claimsMapping

Пространство имен: microsoft.graph

После того как поставщик настраиваемых удостоверений отправит маркер идентификатора обратно в службу Azure AD B2C, Azure AD B2C сопоставляет утверждения от маркера с утверждениями, которые распознает и использует Azure AD B2C.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:-------|:---|:----------|
|userId|String|Утверждение, предоставляющее уникальный идентификатор для вошедшего пользователя. Это обязательное свойство.|
|displayName|Строка|Утверждение, предоставляющее отображаемое или полное имя для пользователя. Это обязательное свойство.|
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


