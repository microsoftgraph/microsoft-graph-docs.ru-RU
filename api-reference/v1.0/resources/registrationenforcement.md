---
title: тип ресурса registrationEnforcement
description: Принудительное выполнение регистрации во время регистрации.
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e46661280fac283123dde6c3820f68911658a6a5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019162"
---
# <a name="registrationenforcement-resource-type"></a>тип ресурса registrationEnforcement

Пространство имен: microsoft.graph

Принудительное выполнение регистрации во время регистрации. В настоящее время это может использоваться только для напоминания пользователям о том, как настроить целевые методы проверки подлинности (например, Microsoft Authenticator) с помощью `authenticationMethodsRegistrationCampaign` .

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|authenticationMethodsRegistrationCampaign|[authenticationMethodsRegistrationCampaign](../resources/authenticationmethodsregistrationcampaign.md)|Запустите кампании, чтобы напомнить пользователям о том, как настроить целевые методы проверки подлинности.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.registrationEnforcement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.registrationEnforcement",
  "authenticationMethodsRegistrationCampaign": {
    "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
  }
}
```
