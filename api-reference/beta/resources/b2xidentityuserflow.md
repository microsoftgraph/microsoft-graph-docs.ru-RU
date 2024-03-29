---
title: Тип ресурса b2xIdentityUserFlow
description: Представляет пользовательский поток самостоятельной регистрации в клиенте Azure Active Directory.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 32eea0f34fcfb1b932995e668c672b21c6b7984c
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695345"
---
# <a name="b2xidentityuserflow-resource-type"></a>Тип ресурса b2xIdentityUserFlow

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательский поток самостоятельной регистрации в клиенте Azure Active Directory.

Пользовательские потоки используются для включения интерфейса [самостоятельной регистрации](/azure/active-directory/external-identities/self-service-sign-up-overview) для гостевых пользователей в приложении. Пользовательские потоки определяют интерфейс, демонстрируемый пользователям при регистрации, в том числе [поставщиков удостоверений](/azure/active-directory/external-identities/identity-providers), которых они могут использовать для проверки подлинности, а также сведения о том, какие атрибуты собираются в процессе регистрации.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление пользовательских потоков](../api/identitycontainer-list-b2xuserflows.md)|Коллекция b2xIdentityUserFlow|Извлечение всех пользовательских потоков B2X.|
|[Получение пользовательского потока](../api/b2xidentityuserflow-get.md)|b2xIdentityUserFlow|Извлечение свойств пользовательского потока B2X.|
|[Создание пользовательского потока](../api/identitycontainer-post-b2xuserflows.md)|b2xIdentityUserFlow|Создание пользовательского потока B2X.|
|[Удаление пользовательского потока](../api/b2xidentityuserflow-delete.md)|Нет|Удаление пользовательского потока B2X.|
|[Перечисление поставщиков удостоверений](../api/b2xidentityuserflow-list-userflowidentityproviders.md)|Коллекция объектов [identityProvider](../resources/identityproviderbase.md)|Получение всех поставщиков удостоверений в пользовательском потоке B2X.|
|[Добавление поставщика удостоверений](../api/b2xidentityuserflow-userflowidentityproviders-update.md)|Нет|Добавление поставщика удостоверений в пользовательский поток B2X.|
|[Удаление поставщика удостоверений](../api/b2xidentityuserflow-delete-userflowidentityproviders.md)|Нет|Удаление поставщика удостоверений из пользовательского потока B2X.|
|[Перечисление поставщиков удостоверений](../api/b2xidentityuserflow-list-identityproviders.md) (не рекомендуется)|Коллекция объектов [identityProvider](../resources/identityProvider.md)|Получение всех поставщиков удостоверений в пользовательском потоке B2X.|
|[Добавление поставщика удостоверений](../api/b2xidentityuserflow-post-identityproviders.md) (не рекомендуется)|Нет|Добавление поставщика удостоверений в пользовательский поток B2X.|
|[Удаление поставщика удостоверений](../api/b2xidentityuserflow-delete-identityproviders.md) (не рекомендуется)|Нет|Удаление поставщика удостоверений из пользовательского потока B2X.|
|[Назначения атрибутов пользователя в списке](../api/b2xidentityuserflow-list-userattributeassignments.md)|Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Извлечение всех назначений атрибутов пользователя в потоке пользователей B2X.|
|[Создание назначения атрибута пользователя](../api/b2xidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Создание назначения атрибута пользователя в потоке пользователей B2X.|
|[Перечисление языков](../api/b2xidentityuserflow-list-languages.md)|Коллекция [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Получение всех языков в пользовательском потоке B2X.|
|[Получение конфигурации соединителей API для пользовательского потока](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md)|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)| Получение конфигурации для соединителей API, применяемых в пользовательском потоке. Параметр запроса $expand не поддерживается для этого метода.|
|[Настройка соединителя API в пользовательском потоке](../api/b2xidentityuserflow-put-apiConnectorConfiguration.md)|Нет| Настройка соединителя API для определенных шагов в пользовательском потоке путем обновления свойства [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md).|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|Строка|Имя пользовательского потока. Это обязательное значение, не изменяемое после создания. После создания перед именем будет добавлен префикс со значением `B2X_1_`.|
|userFlowType|userFlowType|Тип пользовательского потока. Для пользовательских потоков самостоятельной регистрации значением может быть только `signUpOrSignIn`, которое нельзя изменить после создания.|
|userFlowTypeVersion|Одинарное|Версия пользовательского потока. Для пользовательских потоков самостоятельной регистрации всегда применяется версия `1`.|
|apiConnectorConfiguration|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)|Настройка для включения соединителя API с целью использования в составе пользовательского потока самостоятельной регистрации. Вы можете получить значение этого объекта только с помощью метода [Получение userFlowApiConnectorConfiguration](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md).|

## <a name="relationships"></a>Отношения

| Связь       | Тип  |Описание|
|:---------------|:--------|:----------|
|userflowIdentityProviders|Коллекция [identityProviderBase](../resources/identityproviderbase.md)|Поставщики удостоверений, включенные в пользовательский поток.|
|identityProviders (не рекомендуется)|Коллекция объектов [identityProvider](../resources/identityprovider.md)|Поставщики удостоверений, включенные в пользовательский поток.|
|userAttributeAssignments|Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Назначения атрибутов пользователя, включенные в поток пользователей.|
|languages|Коллекция [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Языки, поддерживаемые при настройке в пользовательском потоке. Настройка языка включена по умолчанию в пользовательском потоке самостоятельной регистрации. Вы не можете создавать собственные языки в пользовательских потоках самостоятельной регистрации.|

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
    "userflowIdentityProviders": [{"@odata.type": "microsoft.graph.identityProviderBase"}],
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}],
    "languages": [{"@odata.type": "microsoft.graph.userFlowLanguageConfiguration"}],
    "apiConnectorConfiguration": {
      "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
    }
}
```
