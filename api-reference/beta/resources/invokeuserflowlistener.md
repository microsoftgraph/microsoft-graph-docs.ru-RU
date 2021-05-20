---
title: тип ресурса invokeUserFlowListener
description: Прослушиватель, используемый для вызова потока пользователей во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 89f990ab4692ec7fd4d6ce3b94ee4c4d4846c6c4
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547213"
---
# <a name="invokeuserflowlistener-resource-type"></a>тип ресурса invokeUserFlowListener

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart. Это связывает приложение с потоком пользователей, который позволяет самостоятельной регистрации внешних удостоверений [для](/azure/active-directory/external-identities/self-service-sign-up-overview) приложения. После того как приложение связано с потоком пользователей, пользователи, которые идут в это приложение, смогут инициировать поток регистрации, который содержит учетную запись для гостей.

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
