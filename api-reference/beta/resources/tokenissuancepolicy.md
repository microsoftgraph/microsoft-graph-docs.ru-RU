---
title: Тип ресурса tokenIssuancePolicy
description: Представляет политику для указания характеристик токенов SAML, выданных Azure AD.
ms.localizationpriority: medium
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 257e2b98ffd2e63093b2c5f53b96f9565c13712f
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66767958"
---
# <a name="tokenissuancepolicy-resource-type"></a>Тип ресурса tokenIssuancePolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику для указания характеристик токенов SAML, выданных Azure AD. Политики выдачи маркеров можно использовать для:

- Настройка параметров подписывания
- Настройка алгоритма подписывания
- Настройка версии токена SAML

Наследуется от [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание tokenIssuancePolicy](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Создайте объект tokenIssuancePolicy. |
| [Получение tokenIssuancePolicy](../api/tokenissuancepolicy-get.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Чтение свойств и связей объекта tokenIssuancePolicy. |
| [Перечисление tokenIssuancePolicy](../api/tokenissuancepolicy-list.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Чтение свойств и связей объектов tokenIssuancePolicy. |
| [Обновление tokenIssuancePolicy](../api/tokenissuancepolicy-update.md) | Нет | Обновление объекта tokenIssuancePolicy. |
| [Удаление tokenIssuancePolicy](../api/tokenissuancepolicy-delete.md) | Нет | Удаление объекта tokenIssuancePolicy. |
| [List appliesTo](../api/tokenissuancepolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка объектов directoryObject, к которым применена эта политика. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|Определение|Коллекция объектов string| Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображаемое имя для этой политики. Обязательный.|
|isOrganizationDefault|Логический|Игнорируйте это свойство. Политика выдачи маркеров может применяться только к субъектам-службам и не может быть глобально задана для организации.|


### <a name="properties-of-a-token-issuance-policy-definition"></a>Свойства определения политики выдачи маркеров
Свойства формируют объект JSON, представляющий политику выдачи маркеров. Этот объект JSON необходимо преобразовать **в** строку с escape-кавычками, чтобы вставить его в **свойство** определения. Ниже приведен пример в формате JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":\"1\",\"EmitSAMLNameFormat\": \"true\"}}"
  ]
```


| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|TokenResponseSigningPolicy|String|Представляет параметры подписи сертификата, доступные в Azure AD. Поддерживаемые значения: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.  |
|SamlTokenVersion|String|Версия токена SAML. Поддерживаемые значения: `1.1`, `2.0`. |
|SigningAlgorithm|String|Алгоритм подписи, используемый Azure AD для подписывания маркера SAML. Поддерживаемые значения: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.|
|Version|Целое число|Задайте значение 1. Обязательный.|
| EmitSamlNameFormat | Логический | Если этот флажок выбран, Azure Active Directory добавит дополнительный атрибут NameFormat, описывающий формат имени для ограниченных, основных и необязательных утверждений для этого приложения. [Подробнее](/azure/active-directory/develop/reference-claims-mapping-policy-type#claim-sets) | 

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|appliesTo|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject](directoryObject.md) , к которой была применена эта политика. Только для чтения.|

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


