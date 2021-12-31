---
title: Тип ресурса signIn
doc_type: resourcePageType
description: Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
ms.openlocfilehash: 04f489275de117a4ad3ad603748035b07aebfacc
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61646947"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге. Необходимо иметь лицензию Azure AD Premium P1 или P2 для загрузки журналов входа с помощью API microsoft Graph.

Доступность журналов входа регулируется политиками хранения данных [Azure AD.](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Считывание свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appDisplayName|String|Имя приложения, отображаемая на портале Azure. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|appId|String|Идентификатор приложения в Azure Active Directory. Поддерживает `$filter` `eq` (только оператор).|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection|Список политик условного доступа, которые вызываются соответствующей активностью регистрации.|
|authenticationDetails|[коллекция authenticationDetail](authenticationdetail.md)|Результат попытки проверки подлинности и дополнительные сведения о методе проверки подлинности.|
|authenticationMethodsUsed|Коллекция объектов string|Используемые методы проверки подлинности. Возможные значения: `SMS` , , , , , , или `Authenticator App` `App Verification code` `Password` `FIDO` `PTA` `PHS` .|
|authenticationProcessingDetails|Коллекция [keyValue](keyvalue.md)|Дополнительные сведения об обработке проверки подлинности, например имя агента в случае PTA/PHS или имени Server/farm в случае федератированной проверки подлинности.|
|authenticationProtocol|protocolType|Перечисляет тип протокола или тип гранта, используемый в проверке подлинности. Возможные значения: `none`, `oAuth2`, `ropc`, `wsFederation`, `saml20`, `deviceCode`, `unknownFutureValue`. Для проверки подлинности, которые используют протоколы, не указанные в списке, тип протокола указан как `none` . |
|authenticationRequirement | String | Это имеет наивысший уровень проверки подлинности, необходимой для успешной регистрации при входе. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|authenticationRequirementPolicies|[коллекция authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md)|Источники требования к проверке подлинности, такие как условный доступ, MFA для каждого пользователя, защита удостоверений и по умолчанию безопасности.|
|autonomousSystemNumber|Int32|Автономный номер системы (ASN) сети, используемой субъектом.|
|clientAppUsed|String|Устаревший клиент, используемый для действий по входу. Например: `Browser` `Exchange Active Sync` , `Modern clients` , , , `IMAP` , , `MAPI` или `SMTP` `POP` . Поддерживает `$filter` `eq` (только оператор). |
|conditionalAccessStatus|conditionalAccessStatus| Состояние срабатывуемой политики условного доступа. Возможные значения: `success` `failure` , , или `notApplied` `unknownFutureValue` . Поддерживает `$filter` `eq` (только оператор).|
|correlationId|String|Идентификатор, который отправляется от клиента при входе. Это используется для устранения неполадок соответствующей активности регистрации при вызове поддержки. Поддерживает `$filter` `eq` (только оператор).|
|createdDateTime|DateTimeOffset|Дата и время начала регистрации. Тип Timestamp всегда представлен в формате времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$orderby` и `$filter` `eq` `le` (и только `ge` операторов).|
|crossTenantAccessType|signInAccessType|Описывает тип меж клиента, используемый субъектом для доступа к ресурсу. Возможные значения: `none`, `b2bCollaboration`, `b2bDirectConnect`, `microsoftSupport`, `serviceProvider`, `unknownFutureValue`. Если вход не пересекал границы клиента, значение `none` .|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения об устройстве, откуда произошла входная информация. Включает такие сведения, как deviceId, OS и браузер. Поддерживает `$filter` `eq` (и `startsWith` только операторов) в **свойствах браузера** и **операционной системы.**|
|flaggedForReview|Boolean|При сбойном входе пользователь может нажать кнопку на портале Azure, чтобы отметить неудачное событие для администраторов клиентов. Если пользователь нажал кнопку, чтобы пометить неудачный вход, это значение `true` .|
|homeTenantId|String|Идентификатор клиента пользователя, инициировал вход. Не применимо в входе управляемых удостоверений или основных входных данных службы.|
|homeTenantName|String|Для входных входов пользователя идентификатор клиента, в который входит пользователь. Заполняется только в тех случаях, когда домашний клиент предоставил положительное согласие Azure AD для демонстрации контента клиента.|
|id|String|Идентификатор, представляющий действие входной записи. Наследуется от [сущности](entity.md). Поддерживает `$filter` `eq` (только оператор).|
|incomingTokenType|incomingTokenType|Указывает типы маркеров, которые были представлены Azure AD для проверки подлинности субъекта во входе. Допустимые значения: `none`, `primaryRefreshToken`, `saml11`, `saml20`, `unknownFutureValue`. <br><br> **ПРИМЕЧАНИЕ** Azure AD, возможно, также использовал типы маркеров, не указанные в этом типе Enum, для проверки подлинности субъекта. Не выводим об отсутствии маркера, если он не является одним из перечисленных типов. |
|ipAddress|String|IP-адрес клиента, откуда произошла входная. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|ipAddressFromResourceProvider|String|IP-адрес пользователя, используемый для достижения поставщика ресурсов, используемый для определения соответствия условному доступу для некоторых политик. Например, если пользователь взаимодействует с Exchange Online, Exchange, получаемый от пользователя, может быть записан здесь. Это значение часто `null` .|
|isInteractive|Boolean|Указывает, является ли вход пользователя интерактивным. В интерактивном входе пользователь предоставляет фактор проверки подлинности Azure AD. К этим факторам относятся пароли, ответы на вызовы MFA, биометрические факторы или коды QR, которые пользователь предоставляет Azure AD или связанному приложению. В неаактивную входную информацию пользователь не предоставляет фактор проверки подлинности. Вместо этого клиентские приложения используют маркер или код для проверки подлинности или доступа к ресурсу от имени пользователя. Неинактивные входные входы обычно используются для клиента, чтобы войти от имени пользователя в процессе, прозрачном для пользователя.|
|isTenantRestricted|Boolean|Показывает, был ли знак в событии объектом политики ограничения клиента Azure AD.|
|location|[signInLocation](signinlocation.md)|Код страны города, состояния и 2 буквы, откуда произошла входная. Поддерживает (и только операторов) в свойствах `$filter` `eq` `startsWith` **city,** **state** и **countryOrRegion.**|
|networkLocationDetails|Коллекция [networkLocationDetail](networklocationdetail.md)|Сведения о расположении сети, включая тип используемой сети и ее имена.|
|originalRequestId|String|Идентификатор первого запроса в последовательности проверки подлинности. Поддерживает `$filter` `eq` (только оператор).|
|privateLinkDetails|[privateLinkDetails](../resources/privatelinkdetails.md)|Содержит сведения о политике конфиденциальной ссылки Azure AD, связанной со знаком в случае.|
|processingTimeInMilliseconds|Int|Время обработки запроса в миллисекунде в AD STS.|
|resourceDisplayName|String|Имя ресурса, на который пользователь подписался. Поддерживает `$filter` `eq` (только оператор).|
|resourceId|String|Идентификатор ресурса, на который пользователь подписался. Поддерживает `$filter` `eq` (только оператор).|
|resourceTenantId|String|Идентификатор клиента ресурса, на который ссылается вход.|
|riskDetail|riskDetail|Причина определенного состояния рискованного пользователя, вход или событие риска. Возможные значения: `none` , , , , , , , , `adminGeneratedTemporaryPassword` или `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `unknownFutureValue` . Значение `none` означает, что действия для пользователя или входа пока не выполнялись. Поддерживает `$filter` `eq` (только оператор).<br> **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Все остальные клиенты `hidden` возвращаются.|
|riskEventTypes_v2|Коллекция объектов string|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel` , , , , , , , , `anonymizedIPAddress` или `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` . Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|riskLevelAggregated|riskLevel|Совокупный уровень риска. Возможные значения: `none` , , , , , или `low` `medium` `high` `hidden` `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. Поддерживает `$filter` `eq` (только оператор). <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Все остальные клиенты `hidden` возвращаются.|
|riskLevelDuringSignIn|riskLevel|Уровень риска при входе. Возможные значения: `none` , , , , , или `low` `medium` `high` `hidden` `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. Поддерживает `$filter` `eq` (только оператор). <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Все остальные клиенты `hidden` возвращаются.|
|riskState|riskState|Состояние риска для рискованного пользователя, вход или событие риска. Возможные значения: `none` , , , , , , или `confirmedSafe` `remediated` `dismissed` `atRisk` `confirmedCompromised` `unknownFutureValue` . Поддерживает `$filter` `eq` (только оператор).|
|servicePrincipalCredentialKeyId|String|Уникальный идентификатор учетных данных ключей, используемый директором службы для проверки подлинности.|
|servicePrincipalCredentialThumbprint|String|Отпечатки сертификата сертификата, используемого директором службы для проверки подлинности.|
|servicePrincipalId|String|Идентификатор приложения, используемый для регистрации. Это поле заполняется при входе в приложение. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|servicePrincipalName|String|Имя приложения, используемого для регистрации. Это поле заполняется при входе в приложение. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|signInEventTypes|Коллекция String|Указывает категорию знака в том, что представляет событие. Для входных входов пользователя категория может быть или соответствовать значению свойства `interactiveUser` `nonInteractiveUser` **isInteractive** на ресурсе signin. Для входов управляемых входов удостоверений категория `managedIdentity` . Для входов основного знака службы категория **servicePrincipal**. Возможные значения: `interactiveUser`, `nonInteractiveUser`, `servicePrincipal`, `managedIdentity`, `unknownFutureValue`. Поддерживает `$filter` `eq` (только оператор).|
|signInIdentifier|String|Идентификация, предоставленная пользователем для регистрации. Это может быть userPrincipalName, но оно также заполняется, когда пользователь подписывает другие идентификаторы.|
|signInIdentifierType|signInIdentifierType|Тип знака в идентификаторе. Возможные значения: `userPrincipalName`, `phoneNumber`, `proxyAddress`, `qrCode`, `onPremisesUserPrincipalName`, `unknownFutureValue`.|
|status|[signInStatus](signinstatus.md)|Состояние входного знака. Включает код ошибки и описание ошибки (в случае сбоя при входе). Поддерживает `$filter` `eq` (только оператор) в **свойстве errorCode.**|
|tokenIssuerName|String|Имя поставщика удостоверений. Например, `sts.microsoft.com`. Поддерживает `$filter` `eq` (только оператор).|
|tokenIssuerType|tokenIssuerType|Тип поставщика удостоверений. Допустимые значения: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`, `AzureADBackupAuth`. Обратите внимание, что вы должны использовать загон запроса, чтобы получить следующее значение `Prefer: include - unknown -enum-members` (ы) в этом [развиваемом переуме:](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `AzureADBackupAuth` .|
|uniqueTokenIdentifier|String|Уникальный идентификатор запроса base64, используемый для отслеживания маркеров, выдавлимых Azure AD при их погашении у поставщиков ресурсов. |
|userAgent|String|Сведения агента пользователя, относящиеся к входу. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|userDisplayName|String|Отображаемое имя пользователя. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|userId|String|Идентификатор пользователя. Поддерживает `$filter` `eq` (только оператор).|
|userPrincipalName|String|UpN пользователя. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|userType|signInUserType|Определяет, является ли пользователь участником или гостем в клиенте. Возможные значения: `member`, `guest`, `unknownFutureValue`.|
|mfaDetail (отстает)|String|Это свойство обесценилось.|


## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.signIn",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.signIn",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationRequirement": "String",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "autonomousSystemNumber": "Integer",
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "crossTenantAccessType": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "flaggedForReview": "Boolean",
  "id": "String (identifier)",
  "homeTenantId": "String",
  "homeTenantName": "String",
  "isInteractive": "Boolean",
  "isTenantRestricted": "Boolean",
  "ipAddress": "String",
  "ipAddressFromResourceProvider": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "privateLinkDetails": {
    "@odata.type": "microsoft.graph.privateLinkDetails"
  },
  "processingTimeInMilliseconds": "Integer",
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskEventTypes_v2": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "resourceTenantId": "String",
  "servicePrincipalCredentialKeyId": "String",
  "servicePrincipalCredentialThumbprint": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "signInEventTypes": [
    "String"
  ],
  "signInIdentifier": "String",
  "signInIdentifierType": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
