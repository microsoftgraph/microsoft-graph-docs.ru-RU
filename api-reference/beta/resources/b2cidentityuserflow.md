---
title: Тип ресурса b2cIdentityUserFlow
description: Представляет пользовательский поток в клиенте Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 61c3a206ee07eb7e8474e501f9064a20c6cc3840
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581091"
---
# <a name="b2cidentityuserflow-resource-type"></a>Тип ресурса b2cIdentityUserFlow

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательский поток в клиенте Azure Active Directory B2C.

Чтобы помочь с настройкой наиболее распространенных задач идентификации для ваших приложений, Azure Active Directory B2C содержит заранее определенные настраиваемые политики, называемые [пользовательскими потоками](/azure/active-directory-b2c/user-flow-overview). Пользовательский поток позволяет вам определить, как пользователи взаимодействуют с вашим приложением, когда они выполняют такие задачи, как вход, регистрация, изменение профиля или сброс пароля. Вы можете создать множество пользовательских потоков различных типов в своем клиенте и использовать их в приложении по мере необходимости. С помощью пользовательских потоков вы можете управлять следующими возможностями:

- Типы учетных записей, используемые для входа, например учетные записи социальных сетей, таких как Facebook, или локальные учетные записи
- Атрибуты, собираемые у пользователей, такие как имя, почтовый индекс и размер обуви
- Многофакторная проверка подлинности Azure
- Настройка пользовательского интерфейса
- Сведения, получаемые приложением в маркере

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление пользовательских потоков](../api/identitycontainer-list-b2cuserflows.md)|Коллекция b2cIdentityUserFlow|Извлечение всех пользовательских потоков B2C.|
|[Получение пользовательского потока](../api/b2cidentityuserflow-get.md)|b2cIdentityUserFlow|Извлечение свойств пользовательского потока B2C.|
|[Создание пользовательского потока](../api/identitycontainer-post-b2cuserflows.md)|b2cIdentityUserFlow|Создание пользовательского потока B2C.|
|[Удаление пользовательского потока](../api/b2cidentityuserflow-delete.md)|Нет|Удаление пользовательского потока B2C.|
|[Перечисление поставщиков удостоверений](../api/b2cidentityuserflow-list-identityproviders.md)|Коллекция объектов [identityProvider](../resources/identityProvider.md)|Получение всех поставщиков удостоверений в пользовательском потоке B2C.|
|[Добавление поставщика удостоверений](../api/b2cidentityuserflow-post-identityproviders.md)|Нет|Добавление поставщика удостоверений в пользовательский поток B2C.|
|[Удаление поставщика удостоверений](../api/b2cidentityuserflow-delete-identityproviders.md)|Нет|Удаление поставщика удостоверений из пользовательского потока B2C.|
|[Назначения атрибутов пользователя в списке](../api/b2cidentityuserflow-list-userattributeassignments.md)|Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Извлечение всех назначений атрибутов пользователя в потоке пользователей B2C.|
|[Создание назначения атрибута пользователя](../api/b2cidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Создание назначения атрибута пользователя в потоке пользователей B2C.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|Строка|Имя пользовательского потока. Это обязательное значение, не изменяемое после создания. После создания перед именем будет добавлен префикс со значением `B2C_1_`.|
|userFlowType|Строка|[Тип пользовательского потока](/azure/active-directory-b2c/user-flow-versions). Поддерживаемые значения для **userFlowType**:<br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|userFlowTypeVersion|Одинарное|Версия пользовательского потока.|

## <a name="relationships"></a>Связи

| Связь       | Тип  |Описание|
|:---------------|:--------|:----------|
|identityProviders|Коллекция объектов [identityProvider](../resources/identityprovider.md)|Поставщики удостоверений, включенные в пользовательский поток.|
|userAttributeAssignments|Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Назначения атрибутов пользователя, включенные в поток пользователей.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
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
