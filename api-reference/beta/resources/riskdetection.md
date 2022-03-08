---
title: тип ресурса riskDetection
description: Представляет все обнаружения рисков в клиентах AzureAD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 231141c3ff679af50b5f42652c64b3da18edc005
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335219"
---
# <a name="riskdetection-resource-type"></a>тип ресурса riskDetection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD непрерывно оценивает риски пользователей [](riskyuser.md) и рисков, связанных с входом приложения или пользователя на основе различных сигналов и машинного обучения.[](signin.md) Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Дополнительные сведения о событиях риска см. [в Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
>Для использования API обнаружения Azure AD Premium P1 или P2 необходимо иметь лицензию на использование Azure AD Premium P1 P2.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[List riskDetection](../api/riskdetection-list.md) | [коллекция riskDetection](riskdetection.md)|Список обнаружения рисков и их свойств.|
|[Get riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|Получите определенное обнаружение рисков и его свойства.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|id|string|Уникальный ID обнаружения рисков. |
|requestId|string|Запрос iD входного знака, связанного с обнаружением рисков. Это свойство является null, если обнаружение риска не связано с входом.|
|correlationId|Строка|Корреляция ID входного знака, связанного с обнаружением риска. Это свойство является null, если обнаружение риска не связано с входом. |
|riskEventType|string|Тип обнаруженного события риска. Возможные значения: , , , , , , `suspiciousIPAddress``leakedCredentials`, `investigationsThreatIntelligence`,`adminConfirmedUserCompromised``mcasImpossibleTravel``generic` , `mcasSuspiciousInboxManipulationRules``maliciousIPAddressValidCredentialsBlockedIP``unknownFutureValue``investigationsThreatIntelligenceSigninLinked`и . `malwareInfectedIPAddress``unfamiliarFeatures``maliciousIPAddress``anonymizedIPAddress``unlikelyTravel` <br/> Дополнительные сведения о каждом значении см. в [сведениях о значениях riskEventType](#riskeventtype-values).|
|riskState|riskState|Состояние обнаруженного рискованного пользователя или входной записи. Возможные значения , `none``confirmedSafe`, `remediated`, `dismissed`, , `atRisk`и `confirmedCompromised``unknownFutureValue`. |
|riskLevel|riskLevel|Уровень обнаруженного риска. Возможные значения , `low``medium`, `high`, `hidden`, `none``unknownFutureValue`. <br />**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут возвращены `hidden`.|
|riskDetail|riskDetail|Сведения об обнаружении риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `hidden``unknownFutureValue``userPassedMFADrivenByRiskBasedPolicy``adminDismissedAllRiskForUser``adminConfirmedSigninCompromised``adminConfirmedUserCompromised`, . <br />**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут возвращены `hidden`.|
|source|string|Источник обнаружения рисков. Например, `activeDirectory`. |
|detectionTimingType|riskDetectionTimingType|Сроки обнаружения риска (в режиме реального времени и в автономном режиме). Возможные значения , `notDefined``realtime`, `nearRealtime`, `offline``unknownFutureValue`. |
|действие|activityType|Указывает тип активности, с чем связан обнаруженный риск. Возможные значения , `signin`. `user``unknownFutureValue` |
|tokenIssuerType|tokenIssuerType|Указывает тип эмитента маркеров для обнаруженного риска входного знака. Возможные значения: `AzureAD`, `ADFederationServices` и `unknownFutureValue`. |
|ipAddress|string|Предоставляет IP-адрес клиента, откуда возник риск. |
|location|[signInLocation](signinlocation.md)|Расположение входного знака. |
|activityDateTime|DateTimeOffset|Дата и время возникновения рискованных действий. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|detectedDateTime|DateTimeOffset|Дата и время обнаружения риска. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления обнаружения рисков. |
|userId|строка|Уникальный идентификатор пользователя.  Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|userDisplayName|string|Имя пользователя. |
|userPrincipalName|string|Имя участника-пользователя. |
|additionalInfo|string|Дополнительные сведения, связанные с обнаружением рисков в формате JSON. |
|riskType (неподготовленный)|riskEventType|Список типов событий риска.<br />**Примечание:** Это свойство обесценилось. Вместо **этого используйте riskEventType** . |

### <a name="riskeventtype-values"></a>значения riskEventType

| Member | Описание |
|--|--|
| unlikelyTravel | Определяет два входных знака, происходящих из географически удаленных расположений, где по крайней мере одно из расположений также может быть нетипичным для пользователя, учитывая прошлое поведение.  |
| anonymizedIPAddress | Указывает входы с анонимного IP-адреса, например с помощью анонимного браузера или VPN. |
| maliciousIPAddress | Указывает входы с IP-адресов, известных как вредоносные. Обесценилось и больше не создается для новых обнаружений. |
| unfamiliarFeatures | Указывает входные знаки с характеристиками, которые отклоняться от свойств прошлых входных. |
| malwareInfectedIPAddress | Указывает входы с IP-адресов, зараженных вредоносными программами |
| suspiciousIPAddress | Идентифицирует логины с IP-адресов, которые на момент входа известны как вредоносные. |
| leakedCredentials | Указывает, что допустимые учетные данные пользователя были утечек. Этот общий доступ обычно делается путем публичной публикации в темной сети, на сайтах вклейки или путем торговли и продажи учетных данных на черном рынке. Когда служба учетных данных Майкрософт получает учетные данные пользователей из темного веб-сайта, сайтов вклейки или других источников, они проверяются на наличие действительных учетных данных пользователей Azure AD, чтобы найти допустимые совпадения. |
| investigationsThreatIntelligence | Указывает нестандартную для данного пользователя активность входной записи или согласуется с известными шаблонами атак на основе внутренних и внешних источников разведки угроз Майкрософт. |
| общий | Указывает, что пользователь не включен для защиты удостоверений. |
| AdminConfirmedUserCompromised | Указывает, что администратор подтвердил [, что пользователь скомпрометирован](../api/riskyusers-confirmcompromised.md). |
| mcasImpossibleTravel | Обнаружено Microsoft Defender для облачных приложений (MDCA). Определяет две действия пользователя (один или несколько сеансов), происходящих из географически удаленных расположений в течение периода времени, меньшего, чем время, за которое он должен был ездить из первого расположения во второе, что указывает на то, что другой пользователь использует те же учетные данные. |
| mcasSuspiciousInboxManipulationRules | Обнаружено Microsoft Defender для облачных приложений (MDCA). Определяет подозрительные правила переададки электронной почты, например, если пользователь создал правило "Входящие", которое передает копию всех электронных писем на внешний адрес.|
| investigationsThreatIntelligenceSigninLinked | Определяет необычные действия с известными шаблонами атак на основе сведении об угрозах |
| maliciousIPAddressValidCredentialsBlockedIP | Указывает, что вход был выполнен с действительными учетными данными с вредоносного IP-адреса. |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать. |


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
