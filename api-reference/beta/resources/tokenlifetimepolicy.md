---
title: тип ресурса tokenLifetimePolicy
description: Представляет политику, которая может контролировать срок службы маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: afc82ff81e9fd514cb95bd51ccb9df89e3577bd6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954974"
---
# <a name="tokenlifetimepolicy-resource-type"></a>тип ресурса tokenLifetimePolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику, которая может контролировать срок службы маркера доступа JWT, маркера ID или маркера SAML 1.1/2.0, выданного Azure Active Directory (Azure AD). Жизненный цикл маркера можно задать для всех приложений в вашей организации, мультитенантного приложения (охватывающего несколько организаций) или отдельного субъекта-службы в вашей организации.  Дополнительные сведения о сценарии см. [в материале Configurable token lifetimes in Azure Active Directory.](/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

>Примечание. Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.

Наследует [от stsPolicy](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание tokenLifetimePolicy](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Создание объекта tokenLifetimePolicy. |
| [Get tokenLifetimePolicy](../api/tokenlifetimepolicy-get.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Чтение свойств и связей объекта tokenLifetimePolicy. |
| [Перечисление типов ресурсов tokenLifetimePolicy](../api/tokenlifetimepolicy-list.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Чтение свойств и связей объектов tokenLifetimePolicies. |
| [Обновление tokenLifetimePolicy](../api/tokenlifetimepolicy-update.md) | Нет | Обновление объекта tokenLifetimePolicy. |
| [Удаление tokenLifetimePolicy](../api/tokenlifetimepolicy-delete.md) | Нет | Удаление объекта tokenLifetimePolicy. |
| [Список применяетсяTo](../api/tokenlifetimepolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получите список directoryObjects, к которые была применена эта политика. |
| [Назначение типа ресурса tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md) | Нет | Назначьте объект tokenLifetimePolicy [приложению](application.md) или [объекту servicePrincipal.](serviceprincipal.md) |
| [Список назначенного tokenLifetimePolicy](../api/application-list-tokenlifetimepolicies.md) | Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md) | Список объектов tokenLifetimePolicy, которые назначены объекту [приложения](application.md) или [servicePrincipal.](serviceprincipal.md) |
| [Удаление типа ресурса tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md) | Нет | Удалите объект tokenLifetimePolicy из [приложения](application.md) или [объекта servicePrincipal.](serviceprincipal.md) |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Уникальный идентификатор для этой политики. Только для чтения.|
|определение|Коллекция строк| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|Строка| Описание этой политики.|
|displayName|Строка| Отображение имени для этой политики. Обязательный.|
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

>Примечание. Все периоды времени в этих свойствах указаны в формате "dd.hh:mm:ss".

>Примечание. Максимальные значения для свойств, обозначаемого в "днях", на 1 секунду меньше замечаемого числа дней. Например, максимальное значение 1 дня указывается как "23:59:59".

| Свойство     | Тип   |Описание| Значение Min | Максимальное значение | Значение по умолчанию|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|Строка|Контролирует, как долго и доступ, и маркеры ID считаются допустимыми.|10 минут|1 день|1 час|
|Версия|Целое число|Значение 1. Обязательный.|Нет|Нет|Нет|

## <a name="relationships"></a>Связи

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
