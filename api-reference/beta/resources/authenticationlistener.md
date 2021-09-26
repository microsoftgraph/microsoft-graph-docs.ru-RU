---
title: тип ресурса authenticationListener
description: Определяет слушателя для оценки во время события проверки подлинности.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5528dda667d225d8963ac476542122e2ec8c48c3
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766497"
---
# <a name="authenticationlistener-resource-type"></a>тип ресурса authenticationListener

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет слушателя, который должен оценивать, когда событие проверки подлинности происходит при проверке подлинности. АутентификацияListener абстрактна и является базовым классом различных типов слушателей, которые можно оценить во время события проверки подлинности. 

Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart.. Это связывает приложение с потоком пользователей, что позволяет самообслуживывать [процесс регистрации.](/azure/active-directory/external-identities/self-service-sign-up-overview) После того как приложение связано с потоком пользователей, пользователи, которые идут в это приложение, смогут инициировать поток регистрации, который содержит учетную запись для гостей.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список onSignUpStart](../api/authenticationeventspolicy-list-onsignupstart.md)|[коллекция authenticationListener](../resources/authenticationlistener.md)|Получите коллекцию ресурсов authenticationListener, поддерживаемую событием onSignupStart.|
|[Создание authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|Создайте новый объект authenticationListener для события onSignupStart.|
|[Обновление проверки подлинностиListener](../api/authenticationlistener-update.md)|[authenticationListener](../resources/authenticationlistener.md)|Обновление указанного слушателя, определенного для события onSignupStart в конвейере проверки подлинности.|
|[Put authenticationListener](../api/authenticationlistener-put.md)|[authenticationListener](../resources/authenticationlistener.md)|Замените свойства объекта authenticationListener.|
|[Получить проверку подлинностиListener](../api/authenticationlistener-get.md)|[authenticationListener](../resources/authenticationlistener.md)|Получите указанный слушатель, определенный для события onSignupStart в конвейере проверки подлинности.|
|[Удаление проверки подлинностиListener](../api/authenticationlistener-delete.md)|Нет|Удаление указанного слушателя, определенного для события onSignupStart в конвейере проверки подлинности.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор действия.|
|priority|Int32|Приоритет слушателя. Определяет порядок оценки, когда в событии имеется несколько слушателей. Приоритет оценивается от низкого до высокого.|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Фильтр на основе источника проверки подлинности, который используется для определения оценки прослушиваемого. В настоящее время это ограничивается оценками на основе приложения, в которое пользователь проходит проверку подлинности.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  }
}
```
