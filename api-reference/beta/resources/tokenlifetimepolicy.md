---
title: Тип ресурса tokenLifetimePolicy
description: Представляет политику, которая может управлять сроком действия маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bcfe06a8a42db4b0cfd5c8dab8da2b753e195f2c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155512"
---
# <a name="tokenlifetimepolicy-resource-type"></a>Тип ресурса tokenLifetimePolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику, которая может управлять сроком действия маркера доступа JWT, маркера ИД или маркера SAML 1.1/2.0, выданного Azure Active Directory (Azure AD). Жизненный цикл маркера можно задать для всех приложений в вашей организации, мультитенантного приложения (охватывающего несколько организаций) или отдельного субъекта-службы в вашей организации.  Дополнительные сведения о сценарии см. в сведениях [о настраиваемых сроках действия маркеров в Azure Active Directory.](/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

>Примечание. Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.

Наследуется от [stsPolicy.](stsPolicy.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание tokenLifetimePolicy](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Создание объекта tokenLifetimePolicy. |
| [Get tokenLifetimePolicy](../api/tokenlifetimepolicy-get.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Чтение свойств и связей объекта tokenLifetimePolicy. |
| [Перечисление типов ресурсов tokenLifetimePolicy](../api/tokenlifetimepolicy-list.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Чтение свойств и связей объектов tokenLifetimePolicies. |
| [Обновление tokenLifetimePolicy](../api/tokenlifetimepolicy-update.md) | Нет | Обновление объекта tokenLifetimePolicy. |
| [Удаление tokenLifetimePolicy](../api/tokenlifetimepolicy-delete.md) | Нет | Удаление объекта tokenLifetimePolicy. |
| [List appliesTo](../api/tokenlifetimepolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получите список directoryObjects, к которые была применена эта политика. |
| [Назначение типа ресурса tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md) | Нет | Назначьте объект tokenLifetimePolicy [объекту application](application.md) или [servicePrincipal.](serviceprincipal.md) |
| [Список assigned tokenLifetimePolicy](../api/application-list-tokenlifetimepolicies.md) | Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md) | Список объектов tokenLifetimePolicy, которые назначены объекту [application](application.md) или [servicePrincipal.](serviceprincipal.md) |
| [Удаление типа ресурса tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md) | Нет | Удаление объекта tokenLifetimePolicy из [объекта application](application.md) или [servicePrincipal.](serviceprincipal.md) |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|definition|Коллекция String| Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображаемого имени для этой политики. Обязательно.|
|isOrganizationDefault|Boolean|Если установлено true, активирует эту политику. Для одного типа политики может быть несколько политик, но только одна может быть активирована в качестве организации по умолчанию. Необязательный, значение по умолчанию — false.|


### <a name="properties-of-a-token-lifetime-policy-definition"></a>Свойства определения политики жизненного срока действия маркера
Ниже properties form the JSON object that represents a token lifetime policy. Этот объект JSON необходимо **преобразовать** в строку с escape-кавычками, чтобы вставить его в **свойство** определения. Пример показан ниже в формате JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

>Примечание. Все сроки в этих свойствах заданы в формате "дд.чч:мм:сс".

>Примечание. Максимальное количество свойств, обозначаемого в "днях", составляет 1 секунду от заметимого количества дней. Например, максимальное значение 1 дня указывается как "23:59:59".

| Свойство     | Тип   |Описание| Min Value | Максимальное значение | Значение по умолчанию|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|Управляет тем, как долго маркеры доступа и маркеры ID считаются допустимым.|10 минут|1 день|1 час|
|Версия|Целое число|Установите значение 1. Обязательно.|Нет|Нет|Нет|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|appliesTo|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject,](directoryObject.md) к которую применена эта политика. Только для чтения.|

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