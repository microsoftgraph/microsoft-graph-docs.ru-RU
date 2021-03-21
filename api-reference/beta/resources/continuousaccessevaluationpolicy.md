---
title: тип ресурса continuousAccessEvaluationPolicy
description: Непрерывная оценка доступа (CAE) помогает в управлении сеансами проверки подлинности в режиме реального времени. CaE позволяет клиентам обрабатывать доступ к ресурсам, поддерживая события мгновенного отзыва.
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f34fdacf75b991ff339f4b7cdd823290438e8fea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962642"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a>тип ресурса continuousAccessEvaluationPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Непрерывная оценка доступа (CAE) управляет сеансами проверки подлинности в режиме реального времени. CaE позволяет клиентам обрабатывать доступ к ресурсам, поддерживая события мгновенного отзыва.  Дополнительные сведения см. в [оценке непрерывного доступа.](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-get.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|Ознакомьтесь с свойствами объекта [continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)|
|[Обновление continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-update.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|Обновление свойств объекта [continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)|
|
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Непрерывная оценка доступа автоматически блокирует доступ к ресурсам и приложениям в режиме реального времени при удалении доступа пользователя или изменениях IP-адресов клиента. Только для чтения.|
|displayName|Строка| Значение всегда `Continuous Access Evaluation` . Только для чтения.|
|groups|Коллекция строк|Коллекция идентификаторов групп в области для оценки. Все группы находятся в области, когда коллекция пуста.|
|id|Строка|Указывает идентификатор объекта [continuousAccessEvaluationPolicy.](#continuousaccessevaluationpolicy-resource-type) Только для чтения.|
|isEnabled|Boolean| `true` указать, следует ли проводить оценку непрерывного доступа; в противном `false` случае . |
|users|Коллекция строк|Коллекция идентификаторов пользователей в области для оценки. Все пользователи находятся в области, когда коллекция пуста.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "users": [
    "String"
  ],
  "groups": [
    "String"
  ]
}
```
