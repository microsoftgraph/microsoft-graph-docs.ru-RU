---
title: тип ресурса riskDetection
description: обнаружение рисков
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6b9cfd5ed1a170613563a18351132ef444d198d4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335929"
---
# <a name="riskdetection-resource-type"></a>тип ресурса riskDetection

Пространство имен: microsoft.graph представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD непрерывно оценивает риски пользователей [](riskyuser.md) и рисков, связанных с входом приложения или пользователя на основе различных сигналов и машинного обучения.[](signin.md) Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Дополнительные сведения о событиях риска см. [в Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
>Для использования API обнаружения Azure AD Premium P1 или P2 необходимо иметь лицензию на использование Azure AD Premium P1 P2.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список riskDetections](../api/riskdetection-list.md)|[коллекция riskDetection](../resources/riskdetection.md)|Получите список объектов [riskDetection](../resources/riskdetection.md) и их свойств.|
|[Get riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|Ознакомьтесь с свойствами и отношениями объекта [riskDetection](../resources/riskdetection.md) .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|действие|activityType|Указывает тип активности, с чем связан обнаруженный риск. Возможные значения: `signin`, `user`, `unknownFutureValue`.|
|activityDateTime|DateTimeOffset|Дата и время возникновения рискованных действий. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь UTC 1 января 2014 г. выглядит так: `2014-01-01T00:00:00Z`|
|additionalInfo|Строка|Дополнительные сведения, связанные с обнаружением рисков в формате JSON. Например, `"[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"`. Возможные ключи в строке additionalInfo JSON: `userAgent`, `alertUrl`, , `relatedEventTimeInUtc`, `relatedUserAgent`, `deviceInformation`, `requestId``malwareName``relatedLocation``lastActivityTimeInUtc``clientLocation``correlationId`, `clientIp`, . `riskReasons` <br/>Дополнительные сведения о riskReasons и возможных значениях см. в [этой](#riskreasons-values) информации. |
|correlationId|String|Корреляция ID входного знака, связанного с обнаружением риска. Это свойство, `null` если обнаружение риска не связано с входом.|
|detectedDateTime|DateTimeOffset|Дата и время обнаружения риска. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь UTC 1 января 2014 г. выглядит так: `2014-01-01T00:00:00Z`|
|detectionTimingType|riskDetectionTimingType|Сроки обнаружения риска (в режиме реального времени и в автономном режиме). Возможные значения: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|String|Уникальный ID обнаружения рисков. Унаследованный от [сущности](../resources/entity.md)|
|ipAddress|String|Предоставляет IP-адрес клиента, откуда возник риск.|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления обнаружения рисков. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь UTC 1 января 2014 г. выглядит так: `2014-01-01T00:00:00Z`|
|location|[signInLocation](../resources/signinlocation.md)|Расположение входного знака.|
|requestId|String|Запрос iD входного знака, связанного с обнаружением рисков. Это свойство является null, если обнаружение риска не связано с входом.|
|riskDetail|riskDetail|Сведения об обнаружении риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventType|Строка|Тип обнаруженного события риска. Возможные значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures``malwareInfectedIPAddress`, , `suspiciousIPAddress``impossibleTravel``leakedCredentials``adminConfirmedUserCompromised``generic``passwordSpray``investigationsThreatIntelligence`, `riskyIPAddress``suspiciousBrowser``mcasSuspiciousInboxManipulationRules``anomalousToken``tokenIssuerAnomaly``newCountry`и . `suspiciousInboxForwarding``unknownFutureValue` Если обнаружение риска является обнаружением премиум-класса, будет покажите `generic`. <br/>Дополнительные сведения о каждом значении см. в [сведениях о значениях riskEventType](#riskeventtype-values).|
|riskLevel|riskLevel|Уровень обнаруженного риска. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Состояние обнаруженного рискованного пользователя или входной записи. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|source|String|Источник обнаружения рисков. Например, `activeDirectory`. |
|tokenIssuerType|tokenIssuerType|Указывает тип эмитента маркеров для обнаруженного риска входного знака. Возможные значения: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userDisplayName|String|Имя участника-пользователя. |
|userId|String|Уникальный идентификатор пользователя.|
|userPrincipalName|String|Имя участника-пользователя.|

### <a name="riskeventtype-values"></a>значения riskEventType

| имя; | Имя отображения пользовательского интерфейса | Описание |
|--|--|--|
| unlikelyTravel | Нетипичный проезд | Определяет два входных знака, происходящих из географически удаленных расположений, где по крайней мере одно из расположений также может быть нетипичным для пользователя, учитывая прошлое поведение.  |
| anonymizedIPAddress | Анонимный IP-адрес | Указывает входы с анонимного IP-адреса, например с помощью анонимного браузера или VPN. |
| maliciousIPAddress | Вредоносный IP-адрес | Указывает входы с вредоносного IP-адреса. IP-адрес считается вредоносным на основе высоких показателей отказов из-за недействительных учетных данных, полученных с IP-адреса или других источников репутации IP. |
| unfamiliarFeatures | Незнакомые свойства для входов | Указывает входные знаки с характеристиками, которые отклоняться от свойств прошлых входных. |
| malwareInfectedIPAddress | Ip-адрес, связанный с вредоносными программами | Указывает входы с IP-адресов, зараженных вредоносными программами. Обесценилось и больше не создается для новых обнаружений. |
| suspiciousIPAddress | Вредоносный IP-адрес | Идентифицирует логины с IP-адресов, которые на момент входа известны как вредоносные. |
| leakedCredentials | Утечка учетных данных. | Указывает, что допустимые учетные данные пользователя были утечек. Этот общий доступ обычно делается путем публичной публикации в темной сети, на сайтах вклейки или путем торговли и продажи учетных данных на черном рынке. Когда служба учетных данных Майкрософт получает учетные данные пользователей из темного веб-сайта, сайтов вклейки или других источников, они проверяются на наличие действительных учетных данных пользователей Azure AD, чтобы найти допустимые совпадения. |
| investigationsThreatIntelligence | Аналитика угроз Azure AD | Указывает нестандартную для данного пользователя активность входной записи или согласуется с известными шаблонами атак на основе внутренних и внешних источников разведки угроз Майкрософт. |
| общий | Обнаружен дополнительный риск | Указывает, что пользователь не включен для защиты удостоверений. |
| AdminConfirmedUserCompromised | Администратор подтвердил, что пользователь скомпрометирован | Указывает, что администратор подтвердил [, что пользователь скомпрометирован](../api/riskyuser-confirmcompromised.md). |
| passwordSpray | Распыление пароля | Указывает на то, что несколько имен пользователей атакуются с помощью общих паролей единой грубой силой, чтобы получить несанкционированный доступ. |
| anomalousToken | Аномальный маркер | Указывает, что в маркере имеются аномальные характеристики, такие как необычный срок службы маркера или маркер, который играется из незнакомого расположения. |
| tokenIssuerAnomaly | Аномалия эмитента маркеров | Указывает, что эмитент маркера SAML для связанного маркера SAML потенциально скомпрометирован. Утверждения, включенные в маркер, являются необычными или совпадают с известными шаблонами злоумышленников. |
| suspiciousBrowser | Подозрительный браузер | Подозрительные действия по входу в нескольких клиентах из разных стран в одном браузере. |
| impossibleTravel | Неосуществимое перемещение | Обнаружено Microsoft Defender для облачных приложений (MDCA). Определяет две действия пользователя (один или несколько сеансов), происходящих из географически удаленных расположений в течение периода времени, меньшего, чем время, за которое он должен был ездить из первого расположения во второе, что указывает на то, что другой пользователь использует те же учетные данные. | 
| newCountry | Новая страна | Это обнаружение обнаруживается Microsoft Cloud App Security (MCAS). Вход произошел из расположения, которое не было недавно или никогда не посещало данного пользователя. |
| riskyIPAddress | Действие с анонимного IP-адреса | Это обнаружение обнаруживается Microsoft Cloud App Security (MCAS). Пользователи были активны с IP-адреса, который был идентифицирован как анонимный IP-адрес прокси. |
| mcasSuspiciousInboxManipulationRules | Подозрительные правила обработки входящих сообщений. | Обнаружено Microsoft Defender для облачных приложений (MDCA). Определяет подозрительные правила переададки электронной почты, например, если пользователь создал правило "Входящие", которое передает копию всех электронных писем на внешний адрес.|
| suspiciousInboxForwarding | Подозрительная пересылка входящих сообщений. | Это обнаружение обнаруживается Microsoft Cloud App Security (MCAS). Он ищет подозрительные правила переададки электронной почты, например, если пользователь создал правило почтовых ящиков, которое передает копию всех сообщений электронной почты на внешний адрес. |
| unknownFutureValue | Н/Д | Эволюционирующее значение sentinel. Не следует использовать. |

### <a name="riskreasons-values"></a>значения riskReasons

| riskEventType | Значение | Строка отображения пользовательского интерфейса |
|--|--|--|
| `investigationsThreatIntelligence` | `suspiciousIP` | Этот вход был с подозрительного IP-адреса |
| `investigationsThreatIntelligence` | `passwordSpray` | Эта учетная запись пользователя была атакована спреем пароля. |

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
