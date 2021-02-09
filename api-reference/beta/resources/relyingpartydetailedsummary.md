---
title: Тип ресурса relyingPartyDetailedSummary
description: Представляет в AD FS поднадзорную сторону.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a19132396f88797735801ee782c3c13e12a5e2ca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161126"
---
# <a name="relyingpartydetailedsummary-resource-type"></a>Тип ресурса relyingPartyDetailedSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поднадзорную сторону, настроенную со службами федерации Active Directory (AD FS), ее агрегированное использование и возможность переноса конфигурации с этой стороной в Azure Active Directory.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/relyingpartydetailedsummary-list.md) | [relyingPartyDetailedSummary](relyingpartydetailedsummary.md) | Получить список объектов **relyingPartyDetailedSummary.** |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения. Уникальный идентификатор, созданный на уровне API.| 
|relyingPartyId|String|Этот идентификатор используется для идентификации службящей стороны для этой службы федерации. Он используется при выдаче утверждений в подавную сторону.|
|serviceId|String|Уникально идентифицирует лес Active Directory.|
|migrationStatus|string| Указывает, может ли приложение быть перемещено в Azure AD или требуется более подробное исследование. Возможные значения: `ready`, `needsReview`, `additionalStepsRequired`.|
|migrationValidationDetails|Коллекция [keyValuePair](keyvaluepair.md)|Указывает все проверки, которые необходимо проверить для сведений о конфигурации приложений, чтобы оценить, готово ли приложение к перемещению в Azure AD. Возможные имена: `AdditionalWSFedEndpointCheckResult` , , , , , , ,  `AllowedAuthenticationClassReferencesCheckResult` , `AlwaysRequireAuthenticationCheckResult` , , ,   `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult` ,  `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` . Возможные значения результатов: `0` `1` , или `2` . `0` когда проверка проверки пройдена, когда проверка не пройдена, и когда проверка проверки является `1` `2` предупреждением. |
|relyingPartyName|String|Имя приложения или другой сущности в Интернете, использующей поставщика удостоверений для проверки подлинности пользователя, который хочет войти в систему.|
|failedSignInCount|Int64| Количество неудачных входов в службу федерации Active Directory за указанный период. |
|replyUrls|Коллекция String|Указывает, где ожидается получение маркера.|
|signInSuccessRate|Двойное с плавающей точкой|Количество успешных или успешных входов в службу федерации Active Directory (число успешных и неудачных входов) в указанном периоде.|
|successfulSignInCount|Int64|Количество успешных входов в службу федерации Active Directory.|
|totalSignInCount|Int64|Количество успешных и неудачных входов в службу федерации Active Directory в указанный период.|
|uniqueUserCount|Int64|Количество уникальных пользователей, которые вписались в приложение.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
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


