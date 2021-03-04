---
title: тип ресурса invokeUserFlowListener
description: Прослушиватель, используемый для вызова потока пользователей во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7eee91460c623be982cb316edae1c3c2f0734b07
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442994"
---
# <a name="invokeuserflowlistener-resource-type"></a>тип ресурса invokeUserFlowListener

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart. Это связывает приложение с потоком пользователей, который позволяет самостоятельной регистрации внешних удостоверений [для](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) приложения. После того как приложение связано с потоком пользователей, пользователи, которые идут в это приложение, смогут инициировать поток регистрации, который содержит учетную запись для гостей.

Наследуется от абстрактного базового типа [authenticationListener](../resources/authenticationlistener.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор действия. Наследуется [от authenticationListener](../resources/authenticationlistener.md).|
|priority|Int32|Приоритет действия, используемого для определения одного из нескольких применимых действий. Наследуется [от authenticationListener](../resources/authenticationlistener.md).|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Фильтр на основе источника проверки подлинности, который используется для определения того, выполняется ли прослушиватель. Наследуется [от authenticationListener](../resources/authenticationlistener.md).|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|userFlow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|Поток пользователей, вызываемый при выполнении этого действия.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.invokeUserFlowListener",
  "baseType": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  },
  "userFlow": {
    "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
  }
}
```
