---
title: тип ресурса registrationEnforcement
description: Принудительное выполнение регистрации во время регистрации.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 86d3e974ccfebdf0011c9c19f881096e3fb2ba40
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682918"
---
# <a name="registrationenforcement-resource-type"></a>тип ресурса registrationEnforcement

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Принудительное выполнение регистрации во время регистрации. В настоящее время это может использоваться только для напоминания пользователям о том, как настроить целевые методы проверки подлинности (Microsoft Authenticator) с помощью "authenticationMethodsRegistrationCampaign".

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|authenticationMethodsRegistrationCampaign|[authenticationMethodsRegistrationCampaign](../resources/authenticationmethodsregistrationcampaign.md)|Запустите кампании, чтобы напомнить пользователям о настройке целевых методов проверки подлинности.|

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
