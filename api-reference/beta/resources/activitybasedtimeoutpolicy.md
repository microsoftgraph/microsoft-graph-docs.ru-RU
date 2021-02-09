---
title: Тип ресурса activityBasedTimeoutPolicy
description: Представляет политику, которая может управлять временем ожидания простоя веб-сеансов для приложений, которые поддерживают функции времени ожидания на основе действий.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62f18c7083f96abd7d1cf1d2840aa4e29ce66554
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155599"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a>Тип ресурса activityBasedTimeoutPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику, которая может управлять временем ожидания простоя веб-сеансов для приложений, которые поддерживают функции времени ожидания на основе действий. Приложения принудительно принудительно выключат автоматический вход после периода бездействия. Этот тип политики может применяться только на уровне организации (путем установки свойства **isOrganizationDefault** `true` в ).

Наследуется от [stsPolicy.](stsPolicy.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Создание объекта activityBasedTimeoutPolicy. |
| [Get activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-get.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Чтение свойств и связей объекта activityBasedTimeoutPolicy. |
| [Список activityBasedTimeoutPolicies](../api/activitybasedtimeoutpolicy-list.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Чтение свойств и связей объектов activityBasedTimeoutPolicy. |
| [Обновление activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-update.md) | Нет | Обновление объекта activityBasedTimeoutPolicy. |
| [Удаление activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-delete.md) | Нет | Удаление объекта activityBasedTimeoutPolicy. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|definition|Коллекция String| Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображаемого имени для этой политики. Обязательно.|
|isOrganizationDefault|Boolean|Если установлено true, активирует эту политику. Для одного типа политики может быть несколько политик, но только одна может быть активирована в качестве организации по умолчанию. Необязательный, значение по умолчанию — false.|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a>Свойства определения политики времени действия
Свойства ниже формируют объект JSON, который представляет политику времени действия. Этот объект JSON необходимо **преобразовать** в строку с escape-кавычками, чтобы вставить его в **свойство** определения. Пример показан ниже в формате JSON:

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

>Примечание. Все сроки в этих свойствах заданы в формате "дд.чч:мм:сс".

>Примечание. Максимальное количество свойств, обозначаемого в "днях", составляет 1 секунду от заметимого количества дней. Например, максимальное значение 1 дня указывается как "23:59:59".

| Свойство     | Тип   |Описание|
|:-------------|:------|:---------|
|Версия|Целое число|Версия политики. Установите значение 1. Обязательно.|
|ApplicationPolicies|Объект JSON|Коллекция политики приложений. Политика приложения — это сочетание ApplicationId и WebSessionIdleTimeout: <br> <ul><li>**ApplicationId**: допустимые значения:<ul><li> по умолчанию: применяет политику ко всем приложениям, которые поддерживают функцию времени действия, но не имеют переопределения для конкретного приложения</li><li> c44b4083-3bb0-49c1-b47d-974e53cbdf3c: применяет политику к порталу Azure</li></ul></li><li>**WebSessionIdleTimeout**: период бездействия пользователя, после которого веб-сеанс пользователя считается просроченным. Минимальное значение — 5 минут; максимальное значение — 1 день.</li></ul> |


## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityBasedTimeoutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

