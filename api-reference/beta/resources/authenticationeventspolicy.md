---
title: Тип ресурса authenticationEventsPolicy
description: События проверки подлинности используются для вызова пользовательских потоков в определенных точках потока проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4fe50176ebf49d79adc1db55c657bcf7fed8f096
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159955"
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

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|onSignupStart|[Коллекция authenticationListener](../resources/authenticationlistener.md)|Список применимых действий, которые необходимо принять при регистрации.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationEventsPolicy",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationEventsPolicy",
  "id": "String (identifier)"
}
```
