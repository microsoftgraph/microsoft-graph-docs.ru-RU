---
title: Тип ресурса homeRealmDiscoveryPolicy
description: Представляет политику для управления поведением проверки подлинности Azure Active Directory для федерационных пользователей.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56e0d5b0e47c5f3ba5b37e4cbafad2138a2a7e79
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154210"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a>Тип ресурса homeRealmDiscoveryPolicy

Пространство имен: microsoft.graph

Представляет политику для управления поведением проверки подлинности Azure Active Directory для федерационных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федерационных доменах. Вы можете настроить **homeRealmDiscoveryPolicy** для всех основных служб в организации или для определенных ее основных служб. Дополнительные сведения о сценарии и политике см. в настройках поведения входа [в Azure AD](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) для приложения с помощью политики обнаружения домашней области, а также в входе в [Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin)с помощью электронной почты в качестве альтернативного ИД входа.

Наследуется от [stsPolicy.](stsPolicy.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление типов ресурсов homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-list.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Чтение свойств и связей объектов homeRealmDiscoveryPolicies. |
| [Создание homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Создание объекта homeRealmDiscoveryPolicy. |
| [Get homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-get.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Чтение свойств и связей объекта homeRealmDiscoveryPolicy. |
| [Обновление homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-update.md) | Нет | Обновление объекта homeRealmDiscoveryPolicy. |
| [Удаление homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-delete.md) | Нет | Удаление объекта homeRealmDiscoveryPolicy. |
| [List appliesTo](../api/homerealmdiscoverypolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получите список directoryObjects, к которые была применена эта политика. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|definition|Коллекция String| Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображаемого имени для этой политики. Обязательно.|
|isOrganizationDefault|Логическое|Если установлено true, активирует эту политику. Для одного типа политики может быть несколько политик, но только одна может быть активирована в качестве организации по умолчанию. Необязательный, значение по умолчанию — false.|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a>Свойства определения политики обнаружения домашней области
Ниже properties form the JSON object that represents a token lifetime policy. Этот объект JSON необходимо **преобразовать** в строку с escape-кавычками, чтобы вставить его в **свойство** определения. Пример показан ниже в формате JSON:

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
|AccelerateToFederatedDomain|Логическое| Установите для `true` автоматического ускорения (обход обнаружения домашней области). Если в клиенте имеется только один проверенный и федераированный домен, пользователи будут перенаправлены непосредственно к федератированному поставщику удостоверений `true` (например, ADFS) для входов. Если в клиенте имеется несколько проверенных доменов, необходимо `true` у указано **имя PreferredDomain.** Необязательно.|
|PreferredDomain|String| Указывает домен, в который необходимо ускорить вход. Его можно о пропущено, если у клиента есть только один федераированный домен. Если он опущен и существует несколько проверенных федераированных доменов, эта политика не действует. Обязательно, если **accelerateToFederatedDomain** `true` имеет .|
|AllowCloudPasswordValidation|Логическое| Установите, чтобы разрешить приложению проверку подлинности федератора, предостановив учетные данные пользователя или пароля непосредственно в конечной точке маркера `true` Azure Active Directory. Работает, только если включена синхронизация паролей. Необязательно.|
|AlternateIdLogin| Json |Установите {"Enabled": true}, чтобы разрешить вход в Azure AD с помощью электронной почты в качестве [альтернативного ИД входа.](/azure/active-directory/authentication/howto-authentication-use-email-signin) Работает только в **том случае, если для IsOrganizationDefault** установлено такое же `true` время. Необязательно.|

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
