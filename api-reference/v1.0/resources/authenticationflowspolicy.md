---
title: Тип ресурса authenticationFlowsPolicy
description: 'Представляет конфигурацию политики для интерфейса самостоятельной регистрации на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации. '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ea0ca54c4be4e80043ac9560d2b8dd3744584aa9
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883056"
---
# <a name="authenticationflowspolicy-resource-type"></a>Тип ресурса authenticationFlowsPolicy

Пространство имен: microsoft.graph

Представляет [конфигурацию политики для интерфейса самостоятельной регистрации](../resources/selfservicesignupauthenticationflowconfiguration.md) на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации. Содержит такие сведения, как идентификатор, отображаемое имя и описание, а также указывает, включена ли для политики самостоятельная регистрация.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение политики потоков проверки подлинности](../api/authenticationflowspolicy-get.md)|authenticationFlowsPolicy|Получение конфигурации политики потоков проверки подлинности.|
|[Обновление политики потоков проверки подлинности](../api/authenticationflowspolicy-update.md)|authenticationFlowsPolicy|Обновление конфигурации политики потоков проверки подлинности.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:-------|:---|:----------|
|id|Строка| Унаследованное свойство. Идентификатор политики потоков проверки подлинности. Необязательно. Только для чтения.
|displayName|Строка| Унаследованное свойство. Понятное для пользователя имя политики. Необязательно. Только для чтения.|
|description|Строка|Унаследованное свойство. Описание политики. Необязательно. Только для чтения.|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) |Содержит параметры [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md), описывающие, включена ли самостоятельная регистрация. Необязательно. Только для чтения. |

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
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "selfServiceSignUp": {
    "@odata.type": "#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
  },
}
```
