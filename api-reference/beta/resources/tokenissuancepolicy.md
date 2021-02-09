---
title: Тип ресурса tokenIssuancePolicy
description: Представляет политику для указания характеристик маркеров SAML, выдавляемой Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aae5bd4c252549f92d784b45eaf2d5af15a32db6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159880"
---
# <a name="tokenissuancepolicy-resource-type"></a>Тип ресурса tokenIssuancePolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику для указания характеристик маркеров SAML, выдавляемой Azure AD. Политики выдачи маркеров можно использовать для:

- Настройка параметров подписи
- Настройка алгоритма подписи
- Настройка версии маркера SAML

Наследуется от [stsPolicy.](stsPolicy.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание tokenIssuancePolicy](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Создание объекта tokenIssuancePolicy. |
| [Get tokenIssuancePolicy](../api/tokenissuancepolicy-get.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Чтение свойств и связей объекта tokenIssuancePolicy. |
| [Список tokenIssuancePolicy](../api/tokenissuancepolicy-list.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Чтение свойств и связей объектов tokenIssuancePolicy. |
| [Обновление tokenIssuancePolicy](../api/tokenissuancepolicy-update.md) | Нет | Обновление объекта tokenIssuancePolicy. |
| [Удаление tokenIssuancePolicy](../api/tokenissuancepolicy-delete.md) | Нет | Удаление объекта tokenIssuancePolicy. |
| [List appliesTo](../api/tokenissuancepolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получите список directoryObjects, к которые была применена эта политика. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|definition|Коллекция String| Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображаемого имени для этой политики. Обязательно.|
|isOrganizationDefault|Boolean|Игнорируйте это свойство. Политика выдачи маркеров может применяться только к тем или иным основным службам и не может быть установлена глобально для организации.|


### <a name="properties-of-a-token-issuance-policy-definition"></a>Свойства определения политики выдачи маркеров
Свойства формируют объект JSON, который представляет политику выдачи маркеров. Этот объект JSON необходимо **преобразовать** в строку с escape-кавычками, чтобы вставить его в **свойство** определения. Ниже приводится пример в формате JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|TokenResponseSigningPolicy|String|Представляет параметры подписи сертификатов, доступные в Azure AD. Поддерживаемые значения: `ResponseOnly` , `TokenOnly` , `ResponseAndToken` .  |
|SamlTokenVersion|String|Версия маркера SAML. Поддерживаемые значения: `1.1` , `2.0` . |
|SigningAlgorithm|String|Алгоритм подписи, который Azure AD использует для подписи маркера SAML. Поддерживаемые значения: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` , `http://www.w3.org/2000/09/xmldsig#rsa-sha1` .|
|Версия|Целое число|Установите значение 1. Обязательный.|


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
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
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
  "description": "tokenIssuancePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


