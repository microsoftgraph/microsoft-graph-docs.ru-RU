---
title: тип ресурса homeRealmDiscoveryPolicy
description: Представляет политику по контролю Azure Active Directory проверки подлинности для федерационных пользователей.
ms.localizationpriority: medium
author: hpsin
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: dec8466594981602cf6d933e26a5b2b0214ae011
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804740"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a>тип ресурса homeRealmDiscoveryPolicy

Пространство имен: microsoft.graph

Представляет политику управления поведением Azure Active Directory проверки подлинности для федераций, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федерадных доменах. Вы можете установить **homeRealmDiscoveryPolicy** для всех директоров служб в вашей организации или для определенных директоров служб в вашей организации. Дополнительные сведения о сценарии и политике см. в примере [Настройка входа Azure AD](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) в поведение приложения с помощью политики обнаружения домашней области, а также входа Azure Active Directory электронной почты в качестве альтернативного [входа.](/azure/active-directory/authentication/howto-authentication-use-email-signin)

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
|определение|Коллекция строк| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики. [Дополнительные сведения о](#properties-of-a-home-realm-discovery-policy-definition) схеме JSON для этого свойства см. в материале Свойства определения политики обнаружения домашней области. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображение имени для этой политики. Обязательный.|
|isOrganizationDefault|Boolean|Если установлено, `true`активирует эту политику. Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации. Необязательный, значение по умолчанию `false`.|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a>Свойства определения политики обнаружения домашней области
Свойства, представленные ниже, формируют объект JSON, который представляет политику срока службы маркера. Этот объект JSON **необходимо преобразовать в** строку с кавычками, которые будут вставлены в **свойство определения** . Пример показан ниже в формате JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{
        \"HomeRealmDiscoveryPolicy\": {
          \"AccelerateToFederatedDomain\":true,
          \"AllowCloudPasswordValidation\": false,
          \"PreferredDomain\":\"federated.example.edu\",
          \"AlternateIdLogin\":{
            \"Enabled\":true
          }
        }
      }"
  ]
```

| Свойство     | Тип   |Описание| 
|:---------------|:--------|:----------|
|AccelerateToFederatedDomain|Boolean| Настройка для `true` автоматического ускорения (обход обнаружения домашней области). Если `true` в клиенте есть только один проверенный и федераированный домен, пользователи будут доставлены непосредственно к федератированному поставщику удостоверений (например, ADFS) для регистрации. Если `true` в клиенте имеется несколько проверенных доменов, **необходимо укаменеть PreferredDomain** . Необязательное свойство.|
|AllowCloudPasswordValidation|Boolean| Установите, `true` чтобы разрешить приложению проверку подлинности федератированному пользователю, вручив учетные данные пользователя или пароля непосредственно Azure Active Directory конечной точке маркера. Работает только в том случае, если включена синхронизация паролей. Необязательное свойство.|
|AlternateIdLogin| Json |Установите, `{\"Enabled\": true}` чтобы разрешить вход в Azure AD с помощью электронной почты в [качестве альтернативного входа.](/azure/active-directory/authentication/howto-authentication-use-email-signin) Работает только при **наборе IsOrganizationDefault** `true`. Необязательное свойство.|
|PreferredDomain|String| Указывает домен, чтобы ускорить вход в. Он может быть опущен, если у клиента есть только один федераированный домен. Если он опущен и существует несколько проверенных федераированных доменов, эта политика не влияет. Обязательно, **если accelerateToFederatedDomain** является `true`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|appliesTo|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject](directoryObject.md) , к которую была применена эта политика. Только для чтения.|

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
