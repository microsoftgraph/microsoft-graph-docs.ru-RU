---
title: Тип ресурса riskDetection
description: обнаружения рисков
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6dad1999a6b0cea913f02bb1a072fa501a241157
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061106"
---
# <a name="riskdetection-resource-type"></a>Тип ресурса riskDetection

Пространство имен: microsoft.graph

Представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD постоянно оценивает риски пользователей[](riskyuser.md), а также риски входа приложений или [](signin.md) пользователей на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Дополнительные сведения о событиях риска см[. в Azure Active Directory identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
> 1. Для использования API обнаружения Azure AD Premium P1 или P2 требуется лицензия на Azure AD Premium P1 P2.
> 2. Доступность данных обнаружения рисков регулируется политиками хранения [данных Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов riskDetection](../api/riskdetection-list.md)|[Коллекция riskDetection](../resources/riskdetection.md)|Получение списка объектов [riskDetection](../resources/riskdetection.md) и их свойств.|
|[Получение riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|Чтение свойств и связей объекта [riskDetection](../resources/riskdetection.md) .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|действие|activityType|Указывает тип действия, с который связан обнаруженный риск. Возможные значения: `signin`, `user`, `unknownFutureValue`.|
|activityDateTime|DateTimeOffset|Дата и время возникновения рискованных действий. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь в формате UTC 1 января 2014 г. выглядит следующим образом: `2014-01-01T00:00:00Z`|
|additionalInfo|String|Дополнительные сведения, связанные с обнаружением рисков в формате JSON. Например, `"[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"`. Возможные ключи в строке JSON additionalInfo: `userAgent`, `alertUrl`, `relatedEventTimeInUtc`, , `relatedUserAgent`, `deviceInformation`, `relatedLocation`, `requestId`, `lastActivityTimeInUtc``correlationId`, `malwareName``clientLocation``clientIp`. `riskReasons` <br/>Дополнительные сведения о riskReasons и возможных значениях см. в [разделе значений riskReasons](#riskreasons-values). |
|correlationId|String|Идентификатор корреляции входа, связанного с обнаружением риска. Это свойство имеет значение `null` , если обнаружение риска не связано со входом в систему.|
|detectedDateTime|DateTimeOffset|Дата и время обнаружения риска. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь в формате UTC 1 января 2014 г. выглядит следующим образом: `2014-01-01T00:00:00Z`|
|detectionTimingType|riskDetectionTimingType|Время обнаружения риска (в режиме реального времени или в автономном режиме). Возможные значения: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|String|Уникальный идентификатор обнаружения риска. Наследуется [от сущности](../resources/entity.md)|
|ipAddress|String|Предоставляет IP-адрес клиента, с которого возник риск.|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления обнаружения рисков. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь в формате UTC 1 января 2014 г. выглядит следующим образом: `2014-01-01T00:00:00Z`|
|location|[signInLocation](../resources/signinlocation.md)|Расположение входа.|
|requestId|String|Идентификатор запроса для входа, связанного с обнаружением риска. Это свойство имеет значение NULL, если обнаружение риска не связано со входом.|
|riskDetail|riskDetail|Сведения об обнаруженном риске. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventType|String|Тип обнаруженного события риска. Возможные значения: , , , , `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials``investigationsThreatIntelligence``generic`, ,`adminConfirmedUserCompromised``passwordSpray` , `impossibleTravel`, `newCountry`, `anomalousToken`, `tokenIssuerAnomaly`, ,`suspiciousBrowser` , , `riskyIPAddress`, `mcasSuspiciousInboxManipulationRules`и .`unknownFutureValue``suspiciousInboxForwarding``maliciousIPAddress``anonymizedIPAddress``unlikelyTravel` Если обнаружение риска является обнаружением уровня "Премиум", будет отображаться `generic`. <br/>Дополнительные сведения о каждом значении см. [в описании значений riskEventType](#riskeventtype-values).|
|riskLevel|riskLevel|Уровень обнаруженного риска. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Состояние обнаруженного пользователя с риском или входа в систему. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|source|String|Источник обнаружения риска. Например, `activeDirectory`. |
|tokenIssuerType|tokenIssuerType|Указывает тип издателя маркера для обнаруженного риска входа. Возможные значения: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userDisplayName|String|Имя участника-пользователя. |
|userId|String|Уникальный идентификатор пользователя.|
|userPrincipalName|String|Имя участника-пользователя.|

### <a name="riskeventtype-values"></a>Значения riskEventType

| Имя | Отображаемое имя пользовательского интерфейса | Описание |
|--|--|--|
| unlikelyTravel | Неявные поездки | Идентифицирует два входа, исходящие из географически удаленных расположений, где по крайней мере одно из расположений также может быть неохвачено для пользователя с учетом поведения в прошлом.  |
| anonymizedIPAddress | Анонимный IP-адрес | Указывает входы с анонимного IP-адреса, например с помощью анонимного браузера или VPN. |
| maliciousIPAddress | Вредоносный IP-адрес | Указывает входы с вредоносного IP-адреса. IP-адрес считается вредоносным из-за высокой частоты сбоев из-за недопустимых учетных данных, полученных от IP-адреса или других источников репутации IP-адресов. |
| unfamiliarFeatures | Незнакомые свойства входа | Указывает входы с характеристиками, которые отойдите от прошлых свойств входа. |
| malwareInfectedIPAddress | IP-адрес, связанный с вредоносными программами | Указывает входы с IP-адресов, зараженных вредоносными программами. Не рекомендуется и больше не создается для новых обнаружений. |
| suspiciousIPAddress | Вредоносный IP-адрес | Идентифицирует имена входа с IP-адресов, которые на момент входа известны как вредоносные. |
| leakedCredentials | Утечка учетных данных. | Указывает, что утечка допустимых учетных данных пользователя. Этот общий доступ обычно осуществляется путем публикации общедоступных данных на темном веб-сайте, вставки сайтов или путем продажи учетных данных на черном рынке. Когда служба утечки учетных данных Майкрософт получает учетные данные пользователя из темного веб-сайта, вставки сайтов или других источников, они проверяются на соответствие текущим действительным учетным данным пользователей Azure AD, чтобы найти допустимые совпадения. |
| investigationsThreatIntelligence | Аналитика угроз Azure AD | Указывает действие входа, которое является необычным для данного пользователя или согласуется с известными шаблонами атак на основе внутренних и внешних источников аналитики угроз Корпорации Майкрософт. |
| Универсальный | Обнаружен дополнительный риск | Указывает, что пользователь не был включен для защиты идентификации. |
| adminConfirmedUserComprommed | Администратор подтвердил, что пользователь скомпрометирован | Указывает, что администратор подтвердил [, что пользователь скомпрометирован](../api/riskyuser-confirmcompromised.md). |
| passwordSpray | Распыление пароля | Указывает, что несколько имен пользователей атакуются с помощью общих паролей единым методом подбора, чтобы получить несанкционированный доступ. |
| anomalousToken | Аномальные маркеры | Указывает, что в маркере имеются аномальные характеристики, такие как необычное время существования маркера или токен, воспроизводимый из незнакомого расположения. |
| tokenIssuerAnomaly | Аномалия издателя маркеров | Указывает, что поставщик маркера SAML для связанного маркера SAML потенциально скомпрометирован. Утверждения, включенные в маркер, являются необычными или соответствуют известным шаблонам злоумышленников. |
| suspiciousBrowser | Подозрительный браузер | Подозрительные действия входа в нескольких клиентах из разных стран в одном браузере. |
| impossibleTravel | Неосуществимое перемещение | Обнаружено Microsoft Defender for Cloud Apps (MDCA). Идентифицирует два действия пользователя (один или несколько сеансов), исходящие из географически удаленных расположений в течение более короткого периода времени, чем время, затраченное пользователем на переход от первого расположения к второму, что означает, что другой пользователь использует те же учетные данные. | 
| newCountry | Новая страна | Это обнаружение обнаруживается Microsoft Cloud App Security (MCAS). Вход выполнен из расположения, которое не было недавно или никогда не было показано заданным пользователем. |
| riskyIPAddress | Действия с анонимного IP-адреса | Это обнаружение обнаруживается Microsoft Cloud App Security (MCAS). Пользователи были активны с IP-адреса, который был определен как анонимный IP-адрес прокси-сервера. |
| mcasSuspiulationInboxManipulationRules | Подозрительные правила обработки входящих сообщений. | Обнаружено Microsoft Defender for Cloud Apps (MDCA). Определяет подозрительные правила переадресации электронной почты, например, если пользователь создал правило папки "Входящие", которое пересылает копию всех сообщений электронной почты на внешний адрес.|
| suspiciousInboxForwarding | Подозрительная пересылка входящих сообщений. | Это обнаружение обнаруживается Microsoft Cloud App Security (MCAS). Он ищет подозрительные правила переадресации электронной почты, например, если пользователь создал правило папки "Входящие", которое пересылает копию всех сообщений электронной почты на внешний адрес. |
| unknownFutureValue | Н/Д | Значение sentinel для развиваемого перечисления. Не следует использовать. |

### <a name="riskreasons-values"></a>Значения riskReasons

| riskEventType | Значение | Отображаемая строка пользовательского интерфейса |
|--|--|--|
| `investigationsThreatIntelligence` | `suspiciousIP` | Вход был выполнен с подозрительного IP-адреса. |
| `investigationsThreatIntelligence` | `passwordSpray` | Эта учетная запись пользователя была атакуема распылением пароля. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "String (identifier)",
  "requestId": "String",
  "correlationId": "String",
  "riskEventType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "String",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "activityDateTime": "String (timestamp)",
  "detectedDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "additionalInfo": "String"
}
```
