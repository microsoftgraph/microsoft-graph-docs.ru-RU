---
title: Тип ресурса b2xUserFlows
description: Представляет пользовательский поток в клиенте Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 8f25f99ec54f1db6b68bf5617518d90cc51d3ecc
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319826"
---
# <a name="b2xuserflows-resource-type"></a>Тип ресурса b2xUserFlows

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательский поток в клиенте Azure Active Directory.

Пользовательские потоки используются для включения интерфейса [самостоятельной регистрации](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) для гостевых пользователей в приложении. Пользовательские потоки определяют интерфейс, демонстрируемый пользователям при регистрации, в том числе [поставщиков удостоверений](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers), которых они могут использовать для проверки подлинности, а также сведения о том, какие атрибуты собираются в процессе регистрации.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление пользовательских потоков](../api/b2xuserflows-list.md)|Коллекция b2xUserFlow|Извлечение всех пользовательских потоков.|
|[Получение пользовательского потока](../api/b2xuserflows-get.md)|b2xUserFlow|Извлечение свойств пользовательского потока.|
|[Создание пользовательского потока](../api/b2xuserflow-post-b2xuserflows.md)|b2xUserFlow|Создание пользовательского потока.|
|[Удаление пользовательского потока](../api/b2xuserflows-delete.md)|Нет|Удаление пользовательского потока.|
|[Перечисление поставщиков удостоверений](../api/b2xuserflows-list-identityproviders.md)|Коллекция объектов [identityProvider](../resources/identityProvider.md)|Получение всех поставщиков удостоверений в пользовательском потоке.|
|[Добавление поставщика удостоверений](../api/b2xuserflows-update-identityprovider.md)|Нет|Добавление поставщика удостоверений в пользовательский поток.|
|[Удаление поставщика удостоверений](../api/b2xuserflows-delete-identityprovider.md)|Нет|Удаление поставщика удостоверений из пользовательского потока.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|Строка|Имя пользовательского потока. Это обязательное значение, не изменяемое после создания. После создания перед именем будет добавлен префикс со значением `B2X_1_`.|
|userFlowType|Строка|Тип пользовательского потока. Для пользовательских потоков самостоятельной регистрации значением может быть только `signUpOrSignIn`, которое нельзя изменить после создания.|
|userFlowVersion|Одинарное|Версия пользовательского потока. Для пользовательских потоков B2X всегда используется версия `1`.|

## <a name="relationships"></a>Связи

| Связь       | Тип  |Описание|
|:---------------|:--------|:----------|
|identityProviders|Коллекция объектов [identityProvider](../resources/identityprovider.md)|Поставщики удостоверений, включенные в пользовательский поток.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "optionalProperties": [],
  "keyProperty": "id"
} -->

```json
{
    "id": "String (identifier)",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single",
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```
