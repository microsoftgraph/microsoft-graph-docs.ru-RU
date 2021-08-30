---
title: Тип ресурса authenticationFlowsPolicy
description: 'Представляет конфигурацию политики для интерфейса самостоятельной регистрации на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации. '
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 195f317785d9a0a3ee85c6bb58872d4c47cc8483
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696332"
---
# <a name="authenticationflowspolicy-resource-type"></a>Тип ресурса authenticationFlowsPolicy


Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет [конфигурацию политики для интерфейса самостоятельной регистрации](../resources/selfservicesignupauthenticationflowconfiguration.md) на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации. Содержит сведения об идентификаторе, отображаемое имя и описание, а также указывает, включена ли самостоятельная регистрация для политики.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:-------|:---|:----------|
|id|Строка| Унаследованное свойство. Идентификатор политики потоков проверки подлинности. Необязательно. Только для чтения.
|displayName|Строка| Унаследованное свойство. Понятное для пользователя имя политики. Это свойство не является ключевым. Необязательно. Только для чтения.|
|description|Строка|Унаследованное свойство. Описание политики. Это свойство не является ключевым. Необязательно. Только для чтения.|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) |Содержит параметры [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md), описывающие, включена ли самостоятельная регистрация. Это свойство не является ключевым. Необязательно. Только для чтения. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "openType": false
}
-->

``` json
{
   "id":"String (identifier)",
   "displayName":"String",
   "description":"String",
   "selfServiceSignUp":{
      "@odata.type":"#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
   }
}
```


