---
title: Тип ресурса Релингпартидетаиледсуммари
description: Представляет проверяющую сторону в AD FS.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a3a6fd0ad84ce8e41902cd7c0e82a314fb1aa3ca
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524717"
---
# <a name="relyingpartydetailedsummary-resource-type"></a>Тип ресурса Релингпартидетаиледсуммари

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет проверяющую сторону, настроенную с помощью служб федерации Active Directory (AD FS), его агрегированное использование и возможность переноса конфигурации проверяющей стороны в Azure Active Directory.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/relyingpartydetailedsummary-list.md) | [релингпартидетаиледсуммари](relyingpartydetailedsummary.md) | Получение списка объектов **релингпартидетаиледсуммари** . |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения. Уникальный идентификатор, созданный на уровне API.| 
|релингпартид|String|Этот идентификатор используется для идентификации проверяющей стороны в службе Федерации. Он используется при выдаче утверждений проверяющей стороне.|
|serviceId|String|Уникальный идентификатор леса Active Directory.|
|мигратионстатус|string| Указывает, можно ли переместить приложение в Azure AD или потребовать больше расследований. Возможные значения: `ready`, `needsReview`, `additionalStepsRequired`.|
|мигратионвалидатиондетаилс|Коллекция [keyValuePair](keyvaluepair.md)|Указывает все проверки на правильность конфигурации приложений, которые позволяют оценить, готово ли приложение к перемещению в Azure AD. Возможные имена: `AdditionalWSFedEndpointCheckResult` ,,,,,,,,,,,,  `AllowedAuthenticationClassReferencesCheckResult` `AlwaysRequireAuthenticationCheckResult`   `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult`  `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult` ,  `DelegationAuthorizationRulesCheckResult` , `IssuanceAuthorizationRulesCheckResult` , `IssuanceTransformRulesCheckResult` . Возможные значения result: `0` , `1` , или `2` . `0` Когда проверка проверки пройдена, `1` при неудачной проверке и `2` при проверке на наличие предупреждения. |
|релингпартинаме|String|Имя приложения или другой сущности в Интернете, которая использует поставщика удостоверений для проверки подлинности пользователя, который хочет войти в систему.|
|фаиледсигнинкаунт|Int64| Количество неудачных входов в службу федерации Active Directory в указанном периоде. |
|replyUrls|Коллекция String|Указывает, где ожидается получение маркера проверяющей стороной.|
|сигнинсукцессрате|Двойное с плавающей точкой|Количество успешных/(количество успешных и неудачных входов + количество неудачных входов) в службе федерации Active Directory в указанном периоде.|
|сукцессфулсигнинкаунт|Int64|Количество успешных входов в службу федерации Active Directory.|
|тоталсигнинкаунт|Int64|Количество успешных и неудачных входных входов в службу федерации Active Directory в указанном периоде.|
|уникуеусеркаунт|Int64|Количество уникальных пользователей, выполнивших вход в приложение.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "failedSignInCount": 10,
  "id": "String (identifier)",
  "migrationStatus": "ready | needsReview | additionalStepsRequired",
  "migrationValidationDetails": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "relyingPartyId": "String",
  "relyingPartyName": "String",
  "replyUrls": ["String"],
  "serviceId": "String (identifier)",
  "signInSuccessRate": 90.0,
  "successfulSignInCount": 90,
  "totalSignInCount": 100,
  "uniqueUserCount": 10
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relyingPartyDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


