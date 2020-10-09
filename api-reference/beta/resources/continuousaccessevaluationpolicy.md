---
title: Тип ресурса Континуаусакцессевалуатионполици
description: Оценка непрерывного доступа (КАЕ) помогает управлять сеансами проверки подлинности в режиме реального времени. КАЕ позволяет клиентам обрабатывать доступ к ресурсам, надерживая события для мгновенных вызовов.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8181c327a6ecc430d1bc631295dbc0482edb9eef
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404408"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a>Тип ресурса Континуаусакцессевалуатионполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Оценка непрерывного доступа (КАЕ) управляет сеансами проверки подлинности в режиме реального времени. КАЕ позволяет клиентам обрабатывать доступ к ресурсам, надерживая события для мгновенных вызовов.  Более подробную информацию можно узнать в статье [Оценка непрерывного доступа](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение Континуаусакцессевалуатионполици](../api/continuousaccessevaluationpolicy-get.md)|[континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md)|Чтение свойств объекта [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) .|
|[Обновление Континуаусакцессевалуатионполици](../api/continuousaccessevaluationpolicy-update.md)|[континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md)|Обновление свойств объекта [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) .|
|
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Оценка непрерывного доступа автоматически блокирует доступ к ресурсам и приложениям почти в режиме реального времени при удалении доступа пользователя или изменении IP-адреса клиента. Только для чтения.|
|displayName|String| Значение всегда — "Оценка непрерывного доступа". Только для чтения.|
|groups|Коллекция объектов string|Коллекция идентификаторов групп в области для оценки. Если коллекция пуста, все группы находятся в области действия.|
|id|String|Задает идентификатор объекта Континуаусакцессевалуатионполици. Только для чтения.|
|isEnabled|Boolean| `true` , чтобы указать, следует ли выполнять оценку непрерывного доступа; в противном случае `false` . |
|users|Коллекция объектов string|Коллекция идентификаторов пользователей в области для оценки. Если коллекция пуста, все пользователи находятся в области действия.|

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