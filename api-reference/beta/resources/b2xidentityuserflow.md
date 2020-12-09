---
title: Тип ресурса b2xIdentityUserFlow
description: Представляет пользовательский поток в клиенте Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: e1051d60681e42012fd9df3fd8655a9e4cc745cd
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580965"
---
# <a name="b2xidentityuserflow-resource-type"></a>Тип ресурса b2xIdentityUserFlow

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательский поток в клиенте Azure Active Directory.

Пользовательские потоки используются для включения интерфейса [самостоятельной регистрации](/azure/active-directory/external-identities/self-service-sign-up-overview) для гостевых пользователей в приложении. Пользовательские потоки определяют интерфейс, демонстрируемый пользователям при регистрации, в том числе [поставщиков удостоверений](/azure/active-directory/external-identities/identity-providers), которых они могут использовать для проверки подлинности, а также сведения о том, какие атрибуты собираются в процессе регистрации.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление пользовательских потоков](../api/identitycontainer-list-b2xuserflows.md)|Коллекция b2xIdentityUserFlow|Извлечение всех пользовательских потоков B2X.|
|[Получение пользовательского потока](../api/b2xidentityuserflow-get.md)|b2xIdentityUserFlow|Извлечение свойств пользовательского потока B2X.|
|[Создание пользовательского потока](../api/identitycontainer-post-b2xuserflows.md)|b2xIdentityUserFlow|Создание пользовательского потока B2X.|
|[Удаление пользовательского потока](../api/b2xidentityuserflow-delete.md)|Нет|Удаление пользовательского потока B2X.|
|[Перечисление поставщиков удостоверений](../api/b2xidentityuserflow-list-identityproviders.md)|Коллекция объектов [identityProvider](../resources/identityProvider.md)|Получение всех поставщиков удостоверений в пользовательском потоке B2X.|
|[Добавление поставщика удостоверений](../api/b2xidentityuserflow-post-identityproviders.md)|Нет|Добавление поставщика удостоверений в пользовательский поток B2X.|
|[Удаление поставщика удостоверений](../api/b2xidentityuserflow-delete-identityproviders.md)|Нет|Удаление поставщика удостоверений из пользовательского потока B2X.|
|[Назначения атрибутов пользователя в списке](../api/b2xidentityuserflow-list-userattributeassignments.md)|Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Извлечение всех назначений атрибутов пользователя в потоке пользователей B2X.|
|[Создание назначения атрибута пользователя](../api/b2xidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Создание назначения атрибута пользователя в потоке пользователей B2X.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|Строка|Имя пользовательского потока. Это обязательное значение, не изменяемое после создания. После создания перед именем будет добавлен префикс со значением `B2X_1_`.|
|userFlowType|Строка|Тип пользовательского потока. Для пользовательских потоков самостоятельной регистрации значением может быть только `signUpOrSignIn`, которое нельзя изменить после создания.|
|userFlowTypeVersion|Одинарное|Версия пользовательского потока. Для пользовательских потоков B2X всегда используется версия `1`.|

## <a name="relationships"></a>Связи

| Связь       | Тип  |Описание|
|:---------------|:--------|:----------|
|identityProviders|Коллекция объектов [identityProvider](../resources/identityprovider.md)|Поставщики удостоверений, включенные в пользовательский поток.|
|userAttributeAssignments|Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Назначения атрибутов пользователя, включенные в поток пользователей.|

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}]
}
```
