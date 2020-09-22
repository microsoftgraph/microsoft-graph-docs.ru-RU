---
title: Тип ресурса claimsMapping
description: Сопоставление утверждений от маркера с утверждениями, которые распознает и использует Azure Active Directory B2C.
author: namkedia
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a08f661877ce78d7883f036ba70bed5f088b93e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021941"
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


