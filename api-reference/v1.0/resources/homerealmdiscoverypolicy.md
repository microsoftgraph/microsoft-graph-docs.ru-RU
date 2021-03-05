---
title: тип ресурса homeRealmDiscoveryPolicy
description: Представляет политику управления поведением проверки подлинности Azure Active Directory для федерационных пользователей.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 78fee8908291619a819b1d62108d149c39b0ae68
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444415"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a>тип ресурса homeRealmDiscoveryPolicy

Пространство имен: microsoft.graph

Представляет политику управления поведением проверки подлинности Azure Active Directory для федерационных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федерадных доменах. Вы можете установить **homeRealmDiscoveryPolicy** для всех директоров служб в вашей организации или для определенных директоров служб в вашей организации. Дополнительные сведения о сценарии и политике см. в материале Настройка входа [Azure AD](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) в поведение приложения с помощью политики обнаружения домашней области, а также входа в [Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin)с помощью электронной почты в качестве альтернативного входа.

Наследует [от stsPolicy](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление типов ресурсов homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-list.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Чтение свойств и связей объектов homeRealmDiscoveryPolicies. |
| [Создание homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Создание объекта homeRealmDiscoveryPolicy. |
| [Get homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-get.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Чтение свойств и отношений объекта homeRealmDiscoveryPolicy. |
| [Обновление homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-update.md) | Нет | Обновление объекта homeRealmDiscoveryPolicy. |
| [Удаление homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-delete.md) | Нет | Удаление объекта homeRealmDiscoveryPolicy. |
| [Список применяетсяTo](../api/homerealmdiscoverypolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получите список directoryObjects, к которые была применена эта политика. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|определение|Коллекция строк| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображение имени для этой политики. Обязательно.|
|isOrganizationDefault|Логический|Если заданной для true, активирует эту политику. Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации. Необязательный, значение по умолчанию является ложным.|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a>Свойства определения политики обнаружения домашней области
Свойства, представленные ниже, формируют объект JSON, который представляет политику срока службы маркера. Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.** Пример показан ниже в формате JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\",
      \"AlternateIdLogin\":{\"Enabled\":true}}}"
  ]
```

| Свойство     | Тип   |Описание| 
|:---------------|:--------|:----------|
|AccelerateToFederatedDomain|Логический| Настройка для `true` автоматического ускорения (обход обнаружения домашней области). Если в клиенте есть только один проверенный и федераированный домен, пользователи будут доставлены непосредственно к федератированному поставщику удостоверений `true` (например, ADFS) для регистрации. Если в клиенте имеется несколько проверенных `true` доменов, необходимо укаменеть **PreferredDomain.** Необязательно.|
|PreferredDomain|String| Указывает домен, чтобы ускорить вход в. Он может быть опущен, если у клиента есть только один федераированный домен. Если он опущен и существует несколько проверенных федераированных доменов, эта политика не влияет. Обязательно, **если accelerateToFederatedDomain** `true` является .|
|AllowCloudPasswordValidation|Логический| Установите, чтобы разрешить приложению проверку подлинности федерарно настроенного пользователя путем вручения учетных данных пользователя или пароля непосредственно в конечной точке маркера `true` Azure Active Directory. Работает только в том случае, если включена синхронизация паролей. Необязательно.|
|AlternateIdLogin| Json |Установите {"Включено": true} чтобы разрешить вход в Azure AD с помощью электронной почты в качестве [альтернативного входа.](/azure/active-directory/authentication/howto-authentication-use-email-signin) Работает только при **наборе IsOrganizationDefault** `true` . Необязательно.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|appliesTo|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject,](directoryObject.md) к которую была применена эта политика. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "homeRealmDiscoveryPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
