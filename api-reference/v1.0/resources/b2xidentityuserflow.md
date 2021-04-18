---
title: Тип ресурса b2xIdentityUserFlow
description: Представляет пользовательский поток самостоятельной регистрации в клиенте Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 650bd158bda9c257fc277a9b251e68a90713b7e0
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883318"
---
# <a name="b2xidentityuserflow-resource-type"></a>Тип ресурса b2xIdentityUserFlow

Пространство имен: microsoft.graph

Представляет пользовательский поток самостоятельной регистрации в клиенте Azure Active Directory.

Пользовательские потоки используются для включения интерфейса [самостоятельной регистрации](/azure/active-directory/external-identities/self-service-sign-up-overview) для гостевых пользователей в приложении. Пользовательские потоки определяют интерфейс, демонстрируемый пользователям при регистрации, в том числе [поставщиков удостоверений](/azure/active-directory/external-identities/identity-providers), которых они могут использовать для проверки подлинности, а также сведения о том, какие атрибуты собираются в процессе регистрации.

Наследует от базового класса [identityUserFlow](../resources/identityuserflow.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление пользовательских потоков](../api/identitycontainer-list-b2xuserflows.md)|Коллекция b2xIdentityUserFlow|Получение всех пользовательских потоков самостоятельной регистрации.|
|[Получение пользовательского потока](../api/b2xidentityuserflow-get.md)|b2xIdentityUserFlow|Получение свойств пользовательского потока самостоятельной регистрации.|
|[Создание пользовательского потока](../api/identitycontainer-post-b2xuserflows.md)|b2xIdentityUserFlow|Создание пользовательского потока самостоятельной регистрации.|
|[Удаление пользовательского потока](../api/b2xidentityuserflow-delete.md)|Нет|Удаление пользовательского потока самостоятельной регистрации.|
|[Перечисление поставщиков удостоверений](../api/b2xidentityuserflow-list-identityproviders.md)|Коллекция объектов [identityProvider](../resources/identityProvider.md)|Получение всех поставщиков удостоверений в пользовательском потоке самостоятельной регистрации.|
|[Добавление поставщика удостоверений](../api/b2xidentityuserflow-post-identityproviders.md)|Нет|Добавление поставщика удостоверений в пользовательский поток самостоятельной регистрации.|
|[Удаление поставщика удостоверений](../api/b2xidentityuserflow-delete-identityproviders.md)|Нет|Удаление поставщика удостоверений из пользовательского потока самостоятельной регистрации.|
|[Назначения атрибутов пользователя в списке](../api/b2xidentityuserflow-list-userattributeassignments.md)|Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Получение всех назначений атрибутов пользователя в пользовательском потоке самостоятельной регистрации.|
|[Создание назначения атрибута пользователя](../api/b2xidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Создание назначения атрибутов пользователя в пользовательском потоке самостоятельной регистрации.|
|[Перечисление языков](../api/b2xidentityuserflow-list-languages.md)|Коллекция [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Получение всех языков в пользовательском потоке самостоятельной регистрации.|
|[Получение конфигурации соединителей API для пользовательского потока](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md)|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)| Получение конфигурации для соединителей API, применяемых в пользовательском потоке самостоятельной регистрации. Параметр запроса $expand не поддерживается для этого метода.|
|[Настройка соединителя API в пользовательском потоке](../api/b2xidentityuserflow-put-apiConnectorConfiguration.md)|Нет| Настройка соединителя API для определенных шагов в пользовательском потоке самостоятельной регистрации путем обновления свойства [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md).|

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
|identityProviders|Коллекция объектов [identityProvider](../resources/identityprovider.md)|Поставщики удостоверений, включенные в пользовательский поток.|
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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}],
    "languages": [{"@odata.type": "microsoft.graph.userFlowLanguageConfiguration"}],
    "apiConnectorConfiguration": {
      "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
    }
}
```
