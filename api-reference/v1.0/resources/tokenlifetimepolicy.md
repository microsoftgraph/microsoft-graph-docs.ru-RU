---
title: тип ресурса tokenLifetimePolicy
description: Представляет политику, которая может контролировать срок службы маркера доступа, выданного Azure Active Directory.
ms.localizationpriority: medium
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f6903abfc318c2b49601ef4aafb2a6d428637504
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143666"
---
# <a name="tokenlifetimepolicy-resource-type"></a>тип ресурса tokenLifetimePolicy

Пространство имен: microsoft.graph



Представляет политику, которая может контролировать срок службы маркера доступа JWT, маркера ID или маркера SAML 1.1/2.0, выданного Azure Active Directory (Azure AD). Жизненный цикл маркера можно задать для всех приложений в вашей организации, мультитенантного приложения (охватывающего несколько организаций) или отдельного субъекта-службы в вашей организации. 

>**Примечание:** Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.

Наследует [от stsPolicy](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление типов ресурсов tokenLifetimePolicy](../api/tokenlifetimepolicy-list.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Чтение свойств и связей объектов tokenLifetimePolicies. |
| [Создание tokenLifetimePolicy](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Создание объекта tokenLifetimePolicy. |
| [Get tokenLifetimePolicy](../api/tokenlifetimepolicy-get.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Чтение свойств и связей объекта tokenLifetimePolicy. |
| [Обновление tokenLifetimePolicy](../api/tokenlifetimepolicy-update.md) | Нет | Обновление объекта tokenLifetimePolicy. |
| [Удаление tokenLifetimePolicy](../api/tokenlifetimepolicy-delete.md) | Нет | Удаление объекта tokenLifetimePolicy. |
| [Список применяетсяTo](../api/tokenlifetimepolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получите список directoryObjects, к которые была применена эта политика. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|определение|Коллекция String| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображение имени для этой политики. Обязательно.|
|isOrganizationDefault|Boolean|Если `true` установлено, активирует эту политику. Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации. Необязательный, значение по умолчанию `false` .|


### <a name="properties-of-a-token-lifetime-policy-definition"></a>Свойства определения политики жизни маркера
Свойства, представленные ниже, формируют объект JSON, который представляет политику срока службы маркера. Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.** Пример показан ниже в формате JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

>**Примечание:** Все периоды времени в этих свойствах указаны в формате "dd.hh:mm:ss".

>**Примечание:** Максимальные значения свойств, обозначаемого в "днях", на 1 секунду меньше замечаемого числа дней. Например, максимальное значение 1 дня указывается как "23:59:59".

| Свойство     | Тип   |Описание| Значение Min | Максимальное значение | Значение по умолчанию|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|Контролирует, как долго и доступ, и маркеры ID считаются допустимыми.|10 минут|1 день|1 час|
|Версия|Целое число|Значение 1. Обязательно.|Нет|Нет|Нет|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|appliesTo|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject,](directoryObject.md) к которую была применена эта политика. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenLifetimePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
