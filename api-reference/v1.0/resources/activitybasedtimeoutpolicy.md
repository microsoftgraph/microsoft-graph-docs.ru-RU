---
title: тип ресурса activityBasedTimeoutPolicy
description: Представляет политику, которая может контролировать время ожидания простоя для веб-сеансов для приложений, которые поддерживают функции времени ожидания на основе действий.
ms.localizationpriority: medium
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6b3bfaec22fcbf8c4586c0d990bf38d4c4ad2a0d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094515"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a>тип ресурса activityBasedTimeoutPolicy

Пространство имен: microsoft.graph

Представляет политику, которая может контролировать время ожидания простоя для веб-сеансов для приложений, которые поддерживают функции времени ожидания на основе действий. Приложения применяют автоматическую вывеску после периода бездействия. Этот тип политики можно применять только на уровне организации (задав свойство **isOrganizationDefault).** `true`

Наследует [от stsPolicy](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список действийBasedTimeoutPolicies](../api/activitybasedtimeoutpolicy-list.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Чтение свойств и связей объектов activityBasedTimeoutPolicy. |
| [Создание activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Создание объекта activityBasedTimeoutPolicy. |
| [Get activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-get.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Чтение свойств и связей объекта activityBasedTimeoutPolicy. |
| [Обновление activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-update.md) | Нет | Обновление объекта activityBasedTimeoutPolicy. |
| [Удаление activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-delete.md) | Нет | Удаление объекта activityBasedTimeoutPolicy. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Уникальный идентификатор для этой политики. Только для чтения.|
|определение|Коллекция String| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|Строка| Описание этой политики.|
|displayName|String| Отображение имени для этой политики. Обязательное.|
|isOrganizationDefault|Boolean|Если заданной для true, активирует эту политику. Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации. Необязательный, значение по умолчанию является ложным.|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a>Свойства определения политики политики времени на основе действий
Свойства ниже формируют объект JSON, который представляет политику времени, основанную на действиях. Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.** Пример показан ниже в формате JSON:

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

>**Примечание:** Все периоды времени в этих свойствах указаны в формате "dd.hh:mm:ss".

>**Примечание:** Максимальные значения свойств, обозначаемого в "днях", на 1 секунду меньше замечаемого числа дней. Например, максимальное значение 1 дня указывается как "23:59:59".

| Свойство     | Тип   |Описание|
|:-------------|:------|:---------|
|Версия|Целое число|Версия политики. Значение 1. Обязательное.|
|ApplicationPolicies|Объект JSON|Коллекция политики приложений. Политика приложения — это сочетание ApplicationId и WebSessionIdleTimeout: <br> <ul><li>**ApplicationId:** Допустимые значения:<ul><li> по умолчанию: применяет политику ко всем приложениям, которые поддерживают функции периодиа времени на основе действий, но не имеют переопределения, определенного для приложений</li><li> c44b4083-3bb0-49c1-b47d-974e53cbdf3c3c: применяет политику к порталу Azure</li></ul></li><li>**WebSessionIdleTimeout:** период бездействия пользователя, после которого веб-сеанс пользователя считается истекшим. Минимальное значение — 5 минут; максимальное значение — 1 день.</li></ul> |


## <a name="relationships"></a>Отношения

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

