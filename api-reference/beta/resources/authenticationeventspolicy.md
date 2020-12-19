---
title: Тип ресурса authenticationEventsPolicy
description: События проверки подлинности используются для вызова пользовательских потоков в определенных точках потока проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cc8789fb0de21980571bdcb5254a7760045e61b0
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720358"
---
# <a name="authenticationeventspolicy-resource-type"></a>Тип ресурса authenticationEventsPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс, определяющий события в средстве проверки подлинности, при этом каждое событие дополнительно определяет доступные типы прослушивателей, которые можно создать для события. События являются неотъемлемой частью проверки подлинности; Этот ресурс не настраивается пользователем.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список прослушивателей onSignUpStart](../api/authenticationeventspolicy-list-onsignupstart.md)|[Коллекция authenticationListener](../resources/authenticationlistener.md)|Получите коллекцию ресурсов authenticationListener, поддерживаемых событием onSignupStart.|
|[Создание authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|Создайте новый объект authenticationListener для события onSignupStart.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики.|

## <a name="relationships"></a>Отношения

|Связь|Тип|Описание|
|:---|:---|:---|
|onSignupStart|[Коллекция authenticationListener](../resources/authenticationlistener.md)|Список применимых действий, которые необходимо принять при регистрации.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationEventsPolicy",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationEventsPolicy",
  "id": "String (identifier)"
}
```
