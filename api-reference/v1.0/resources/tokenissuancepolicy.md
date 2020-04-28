---
title: Тип ресурса Токениссуанцеполици
description: Представляет политику, определяющую характеристики маркеров SAML, выданных Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ac50b952a075ec4ce4b9257fa28c0e5a9aba6096
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916895"
---
# <a name="tokenissuancepolicy-resource-type"></a>Тип ресурса Токениссуанцеполици

Пространство имен: microsoft.graph



Представляет политику, определяющую характеристики маркеров SAML, выданных Azure AD. Политики выдачи маркеров можно использовать для следующих действий:

- Настройка параметров подписывания
- Настройка алгоритма подписи
- Установка версии токена SAML

Наследуется от [стсполици](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Токениссуанцеполици](../api/tokenissuancepolicy-list.md) | [токениссуанцеполици](tokenissuancepolicy.md) | Чтение свойств и связей объектов Токениссуанцеполици. |
| [Создание Токениссуанцеполици](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [токениссуанцеполици](tokenissuancepolicy.md) | Создание объекта Токениссуанцеполици. |
| [Получение Токениссуанцеполици](../api/tokenissuancepolicy-get.md) | [токениссуанцеполици](tokenissuancepolicy.md) | Чтение свойств и связей объекта Токениссуанцеполици. |
| [Обновление Токениссуанцеполици](../api/tokenissuancepolicy-update.md) | Нет | Обновление объекта Токениссуанцеполици. |
| [Удаление Токениссуанцеполици](../api/tokenissuancepolicy-delete.md) | Нет | Удаление объекта Токениссуанцеполици. |
| [Список appliesTo](../api/tokenissuancepolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка Директорйобжектс, к которым применена эта политика. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|RDLC|Коллекция объектов string| Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики. Ниже приведены дополнительные сведения о схеме JSON для этого свойства. Обязательный.|
|description|String| Описание для этой политики.|
|displayName|Строка| Отображаемое имя для этой политики. Обязательный.|
|исорганизатиондефаулт|Boolean|Игнорировать это свойство. Политика выдачи маркеров может применяться только к субъектам служб и не может быть настроена глобально для Организации.|


### <a name="properties-of-a-token-issuance-policy-definition"></a>Свойства определения политики выдачи маркеров
Свойства формируют объект JSON, представляющий политику выдачи маркеров. Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** . Ниже приведен пример в формате JSON.

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
|токенреспонсесигнингполици|String|Представляет параметры подписи сертификатов, доступные в Azure AD. Поддерживаются следующие значения `ResponseOnly`: `TokenOnly`, `ResponseAndToken`,.  |
|самлтокенверсион|String|Версия маркера SAML. Поддерживаются следующие значения `1.1`: `2.0`,. |
|сигнингалгорисм|String|Использование алгоритма подписи для подписи маркера SAML в Azure AD. Поддерживаются следующие значения `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`: `http://www.w3.org/2000/09/xmldsig#rsa-sha1`,.|
|Версия|Целое число|Установите значение 1. Обязательный.|


## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Тег|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "baseType": "",
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
