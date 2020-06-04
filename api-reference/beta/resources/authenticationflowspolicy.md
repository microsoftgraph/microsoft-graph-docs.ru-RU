---
title: Тип ресурса Аусентикатионфловсполици
description: 'Представляет конфигурацию политики взаимодействия с самостоятельной регистрацией на уровне клиента, с помощью которой внешние пользователи могут подписаться на утверждение. '
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 263b92c081545fc3ce337d25b4813d85fe034940
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556462"
---
# <a name="authenticationflowspolicy-resource-type"></a>Тип ресурса Аусентикатионфловсполици


Пространство имен: microsoft.graph

Представляет [конфигурацию политики взаимодействия с самостоятельной регистрацией](../resources/selfservicesignupauthenticationflowconfiguration.md) на уровне клиента, с помощью которой внешние пользователи могут подписаться на утверждение. Он содержит сведения об ИДЕНТИФИКАТОРе, отображаемое имя и описание, а также указывает, включена ли функция регистрации самостоятельных служб для этой политики.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:-------|:---|:----------|
|id|String| Унаследованное свойство. Идентификатор политики потоков проверки подлинности. Необязательное свойство. Только для чтения.
|displayName|Строка| Унаследованное свойство. Понятное для человека имя политики. Это свойство не является ключом. Необязательное свойство. Только для чтения.|
|description|String|Унаследованное свойство. Описание политики. Это свойство не является ключом. Необязательное свойство. Только для чтения.|
|селфсервицесигнуп|[селфсервицесигнупаусентикатионфловконфигуратион](../resources/selfservicesignupauthenticationflowconfiguration.md) |Содержит параметры [селфсервицесигнупаусентикатионфловконфигуратион](../resources/selfservicesignupauthenticationflowconfiguration.md) , которые сообщают, включена или отключена самостоятельная регистрация. Это свойство не является ключом. Необязательное свойство. Только для чтения. |

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "selfServiceSignUp": {
    "@odata.type": "#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
  },
}
```
