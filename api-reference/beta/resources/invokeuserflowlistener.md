---
title: Тип ресурса invokeUserFlowListener
description: Прослушиватель, используемый для вызова пользовательского потока во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0ca1c61d830a2ff98f2d72839129d75cc6287c36
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720437"
---
# <a name="invokeuserflowlistener-resource-type"></a>Тип ресурса invokeUserFlowListener

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart. Это связывает приложение с пользовательским потоком, что позволяет внешним удостоверениям самостоятельно зарегистрироваться [в](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) приложении. После того как приложение будет связано с потоком пользователей, пользователи, которые будут перейти к этому приложению, смогут инициировать процесс регистрации, который будет подготовка гостевой учетной записи.

Наследуется от абстрактного базового типа [authenticationListener.](../resources/authenticationlistener.md)

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор действия. Наследуется [от authenticationListener.](../resources/authenticationlistener.md)|
|priority|Int32|Приоритет действия, используемого для определения одного из нескольких применимых действий. Наследуется [от authenticationListener.](../resources/authenticationlistener.md)|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Фильтрация на основе источника проверки подлинности, используемого для определения того, выполняется ли прослушиватель. Наследуется [от authenticationListener.](../resources/authenticationlistener.md)|

## <a name="relationships"></a>Отношения

|Связь|Тип|Описание|
|:---|:---|:---|
|userFlow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|Пользовательский поток, который вызывается при выполнении этого действия.|

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
