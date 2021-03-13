---
title: Тип ресурса claimsMapping
description: Сопоставление утверждений от маркера с утверждениями, которые распознает и использует Azure Active Directory B2C.
author: namkedia
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1863c6bf6f28e0e8ae8a3d1133330337a7420c0a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761844"
---
# <a name="claimsmapping-resource-type"></a>Тип ресурса claimsMapping

Пространство имен: microsoft.graph

После того как поставщик настраиваемых удостоверений отправит маркер идентификатора обратно в службу Azure AD B2C, Azure AD B2C сопоставляет утверждения от маркера с утверждениями, которые распознает и использует Azure AD B2C.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:-------|:---|:----------|
|userId|String|Утверждение, предоставляющее уникальный идентификатор для вошедшего пользователя. Это обязательное свойство.|
|displayName|String|Утверждение, предоставляющее отображаемое или полное имя для пользователя. Это обязательное свойство.|
|givenName;|String|Утверждение, предоставляющее имя пользователя.|
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


