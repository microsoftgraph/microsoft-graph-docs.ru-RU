---
title: Тип ресурса b2cUserFlows
description: Представляет пользовательский поток в клиенте Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: e540f5b6ff21efd4ba904ddaf4dcb4868df75eff
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319828"
---
# <a name="b2cuserflows-resource-type"></a>Тип ресурса b2cUserFlows

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательский поток в клиенте Azure Active Directory B2C.

Чтобы помочь с настройкой наиболее распространенных задач идентификации для ваших приложений, Azure Active Directory B2C содержит заранее определенные настраиваемые политики, называемые [пользовательскими потоками](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-overview). Пользовательский поток позволяет вам определить, как пользователи взаимодействуют с вашим приложением, когда они выполняют такие задачи, как вход, регистрация, изменение профиля или сброс пароля. Вы можете создать множество пользовательских потоков различных типов в своем клиенте и использовать их в приложении по мере необходимости. С помощью пользовательских потоков вы можете управлять следующими возможностями:

- Типы учетных записей, используемые для входа, например учетные записи социальных сетей, таких как Facebook, или локальные учетные записи
- Атрибуты, собираемые у пользователей, такие как имя, почтовый индекс и размер обуви
- Многофакторная проверка подлинности Azure
- Настройка пользовательского интерфейса
- Сведения, получаемые приложением в маркере

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление пользовательских потоков](../api/b2cuserflows-list.md)|Коллекция b2cUserFlow|Извлечение всех пользовательских потоков.|
|[Получение пользовательского потока](../api/b2cuserflows-get.md)|b2cUserFlow|Извлечение свойств пользовательского потока.|
|[Создание пользовательского потока](../api/b2cuserflow-post-b2cuserflows.md)|b2cUserFlow|Создание пользовательского потока.|
|[Удаление пользовательского потока](../api/b2cuserflows-delete.md)|Нет|Удаление пользовательского потока.|
|[Перечисление поставщиков удостоверений](../api/b2cuserflows-list-identityproviders.md)|Коллекция объектов [identityProvider](../resources/identityProvider.md)|Получение всех поставщиков удостоверений в пользовательском потоке.|
|[Добавление поставщика удостоверений](../api/b2cuserflows-update-identityprovider.md)|Нет|Добавление поставщика удостоверений в пользовательский поток.|
|[Удаление поставщика удостоверений](../api/b2cuserflows-delete-identityprovider.md)|Нет|Удаление поставщика удостоверений из пользовательского потока.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|Строка|Имя пользовательского потока. Это обязательное значение, не изменяемое после создания. После создания перед именем будет добавлен префикс со значением `B2C_1_`.|
|userFlowType|Строка|[Тип пользовательского потока](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions). Поддерживаемые значения для **userFlowType**:<br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|userFlowVersion|Одинарное|Версия пользовательского потока.|

## <a name="relationships"></a>Связи

| Связь       | Тип  |Описание|
|:---------------|:--------|:----------|
|identityProviders|Коллекция объектов [identityProvider](../resources/identityprovider.md)|Поставщики удостоверений, включенные в пользовательский поток.|

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```
