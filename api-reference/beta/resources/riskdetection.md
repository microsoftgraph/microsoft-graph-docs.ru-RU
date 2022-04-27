---
title: Тип ресурса riskDetection
description: Представляет все обнаружения рисков в клиентах AzureAD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5e27d1df57ac4242f74cca746b7dc8890f004c7a
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060488"
---
# <a name="riskdetection-resource-type"></a>Тип ресурса riskDetection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD постоянно оценивает риски пользователей[](riskyuser.md), а также риски входа приложений или [](signin.md) пользователей на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Дополнительные сведения о событиях риска см[. в Azure Active Directory identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
> 1. Для использования API обнаружения Azure AD Premium P1 или P2 требуется лицензия на Azure AD Premium P1 P2.
> 2. Доступность данных обнаружения рисков регулируется политиками хранения [данных Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление riskDetection](../api/riskdetection-list.md) | [Коллекция riskDetection](riskdetection.md)|Вывод списка обнаружений рисков и их свойств.|
|[Получение riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|Получение определенного обнаружения рисков и его свойств.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|id|string|Уникальный идентификатор обнаружения риска. |
|requestId|string|Идентификатор запроса для входа, связанного с обнаружением риска. Это свойство имеет значение NULL, если обнаружение риска не связано со входом.|
|correlationId|string|Идентификатор корреляции входа, связанного с обнаружением риска. Это свойство имеет значение NULL, если обнаружение риска не связано со входом. |
|riskEventType|string|Тип обнаруженного события риска. Возможные значения: , , , , `unfamiliarFeatures``malwareInfectedIPAddress`, , `suspiciousIPAddress``leakedCredentials`, `investigationsThreatIntelligence`,`adminConfirmedUserCompromised``generic`, , `mcasSuspiciousInboxManipulationRules``mcasImpossibleTravel`, , `investigationsThreatIntelligenceSigninLinked`и . `maliciousIPAddressValidCredentialsBlockedIP``unknownFutureValue``maliciousIPAddress``anonymizedIPAddress``unlikelyTravel` <br/> Дополнительные сведения о каждом значении см. [в описании значений riskEventType](#riskeventtype-values).|
|riskState|riskState|Состояние обнаруженного пользователя с риском или входа в систему. Возможные значения: , , , , , , `atRisk`и `unknownFutureValue``confirmedCompromised`. `dismissed``remediated``confirmedSafe``none` |
|riskLevel|riskLevel|Уровень обнаруженного риска. Возможные значения: , , , , `hidden`. `none``unknownFutureValue``high``medium``low` <br />**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут возвращены `hidden`.|
|riskDetail|riskDetail|Сведения об обнаруженном риске. Возможные значения: , , , , , `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe``userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised``unknownFutureValue``adminConfirmedUserCompromised``hidden`. `userPerformedSecuredPasswordReset``userPerformedSecuredPasswordChange``adminGeneratedTemporaryPassword``none` <br />**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут возвращены `hidden`.|
|source|string|Источник обнаружения риска. Например, `activeDirectory`. |
|detectionTimingType|riskDetectionTimingType|Время обнаружения риска (в режиме реального времени или в автономном режиме). Возможные значения: `notDefined`, `realtime`, `nearRealtime`, `offline`. `unknownFutureValue` |
|действие|activityType|Указывает тип действия, с который связан обнаруженный риск. Возможные значения: `signin`, `user`. `unknownFutureValue` |
|tokenIssuerType|tokenIssuerType|Указывает тип издателя маркера для обнаруженного риска входа. Возможные значения: `AzureAD`, `ADFederationServices` и `unknownFutureValue`. |
|ipAddress|string|Предоставляет IP-адрес клиента, с которого возник риск. |
|location|[signInLocation](signinlocation.md)|Расположение входа. |
|activityDateTime|DateTimeOffset|Дата и время возникновения рискованных действий. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|detectedDateTime|DateTimeOffset|Дата и время обнаружения риска. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления обнаружения рисков. |
|userId|строка|Уникальный идентификатор пользователя.  Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|userDisplayName|string|Имя пользователя. |
|userPrincipalName|string|Имя участника-пользователя. |
|additionalInfo|string|Дополнительные сведения, связанные с обнаружением рисков в формате JSON. |
|riskType (не рекомендуется)|riskEventType|Список типов событий риска.<br />**Примечание:** Это свойство является устаревшим. Вместо **этого используйте riskEventType** . |

### <a name="riskeventtype-values"></a>Значения riskEventType

| Member | Описание |
|--|--|
| unlikelyTravel | Идентифицирует два входа, исходящие из географически удаленных расположений, где по крайней мере одно из расположений также может быть неохвачено для пользователя с учетом поведения в прошлом.  |
| anonymizedIPAddress | Указывает входы с анонимного IP-адреса, например с помощью анонимного браузера или VPN. |
| maliciousIPAddress | Указывает на входы с IP-адресов, известных как вредоносные. Не рекомендуется и больше не создается для новых обнаружений. |
| unfamiliarFeatures | Указывает входы с характеристиками, которые отойдите от прошлых свойств входа. |
| malwareInfectedIPAddress | Указывает входы с IP-адресов, зараженных вредоносными программами |
| suspiciousIPAddress | Идентифицирует имена входа с IP-адресов, которые на момент входа известны как вредоносные. |
| leakedCredentials | Указывает, что утечка допустимых учетных данных пользователя. Этот общий доступ обычно осуществляется путем публикации общедоступных данных на темном веб-сайте, вставки сайтов или путем продажи учетных данных на черном рынке. Когда служба утечки учетных данных Майкрософт получает учетные данные пользователя из темного веб-сайта, вставки сайтов или других источников, они проверяются на соответствие текущим действительным учетным данным пользователей Azure AD, чтобы найти допустимые совпадения. |
| investigationsThreatIntelligence | Указывает действие входа, которое является необычным для данного пользователя или согласуется с известными шаблонами атак на основе внутренних и внешних источников аналитики угроз Корпорации Майкрософт. |
| Универсальный | Указывает, что пользователь не был включен для защиты идентификации. |
| adminConfirmedUserComprommed | Указывает, что администратор подтвердил [, что пользователь скомпрометирован](../api/riskyusers-confirmcompromised.md). |
| mcasImpossibleTravel | Обнаружено Microsoft Defender for Cloud Apps (MDCA). Идентифицирует два действия пользователя (один или несколько сеансов), исходящие из географически удаленных расположений в течение более короткого периода времени, чем время, затраченное пользователем на переход от первого расположения к второму, что означает, что другой пользователь использует те же учетные данные. |
| mcasSuspiulationInboxManipulationRules | Обнаружено Microsoft Defender for Cloud Apps (MDCA). Определяет подозрительные правила переадресации электронной почты, например, если пользователь создал правило папки "Входящие", которое пересылает копию всех сообщений электронной почты на внешний адрес.|
| investigationsThreatIntelligenceSigninLinked | Определяет действия, которые нетипичены с известными шаблонами атак на основе аналитики угроз |
| maliciousIPAddressValidCredentialsBlockedIP | Указывает, что вход выполнен с использованием допустимых учетных данных с вредоносного IP-адреса. |
| unknownFutureValue | Значение sentinel для развиваемого перечисления. Не следует использовать. |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskDetection"
}-->

```json
{
 "id": "string",
    "requestId": "string",
    "correlationId": "string",
    "riskType": {"@odata.type": "microsoft.graph.riskEventType"},
    "riskState": {"@odata.type": "microsoft.graph.riskState"},
    "riskLevel": {"@odata.type": "microsoft.graph.riskLevel"},
    "riskDetail": {"@odata.type": "microsoft.graph.riskDetail"},
    "source": "string",
    "detectionTimingType": {"@odata.type": "microsoft.graph.riskDetectionTimingType"},
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"},
    "tokenIssuerType": {"@odata.type": "microsoft.graph.tokenIssuerType"},
    "ipAddress": "string",
    "location": {"@odata.type": "microsoft.graph.signInLocation"},
    "activityDateTime": "string (timestamp)",
    "detectedDateTime": "string (timestamp)",
    "lastUpdatedDateTime": "string (timestamp)",
    "userId": "string",
    "userDisplayName": "string",
    "userPrincipalName": "string",
    "additionalInfo": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskDetections resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
