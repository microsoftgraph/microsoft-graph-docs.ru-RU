---
title: Тип ресурса signIn
doc_type: resourcePageType
description: Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
ms.openlocfilehash: ba1100b738c2904c6661e52df62171a11aa4dda3
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819351"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге. У вас должна быть Azure AD Premium P1 или P2 для скачивания журналов входа с помощью microsoft API Graph.

Доступность журналов входа регулируется политиками хранения Azure AD [данных](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Считывание свойств и связей объекта signIn.|
|[Подтвердить скомпрометированный](../api/signin-confirmcompromised.md)|Нет|Пометьте событие в Azure AD входа как рискованные.|
|[Подтверждение безопасности](../api/signin-confirmsafe.md)|Нет|Пометьте событие в Azure AD входа как безопасное.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appDisplayName|String|Имя приложения, отображаемое на портале Azure. Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|appId|String|Идентификатор приложения в Azure Active Directory. Поддерживает ( `$filter` только`eq` оператор).|
|appliedConditionalAccessPolicies|[Коллекция appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)|Список политик условного доступа, активированных соответствующим действием входа.|
|authenticationContextClassReferences|[Коллекция authenticationContext](authenticationcontext.md)|Содержит коллекцию значений, представляющих контексты проверки подлинности условного доступа, применяемые к входу.|
|authenticationDetails|[Коллекция authenticationDetail](authenticationdetail.md)|Результат попытки проверки подлинности и дополнительные сведения о методе проверки подлинности.|
|authenticationMethodsUsed|Коллекция строк|Используемые методы проверки подлинности. Возможные значения: `SMS`, `Authenticator App`, `App Verification code`, `Password`, , `FIDO`, или `PHS``PTA`.|
|authenticationProcessingDetails|Коллекция [keyValue](keyvalue.md)|Дополнительные сведения об обработке проверки подлинности, такие как имя агента в случае PTA/PHS или имя сервера или фермы в случае федеративной проверки подлинности.|
|authenticationProtocol|protocolType|Перечисляет тип протокола или тип предоставления, используемый при проверке подлинности. Возможные значения: `none`, `oAuth2`, `ropc`, `wsFederation`, `saml20`, `deviceCode`, `unknownFutureValue`. Для проверки подлинности, использующих протоколы, отличные от возможных перечисленных значений, тип протокола указан как `none`. |
|authenticationRequirement | Строка | Это обеспечивает наивысший уровень проверки подлинности, необходимый для успешного входа. Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|authenticationRequirementPolicies|[Коллекция authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md)|Источники требований к проверке подлинности, такие как условный доступ, многофакторная проверка подлинности для каждого пользователя, защита идентификации и параметры безопасности по умолчанию.|
|autonomousSystemNumber|Int32|Номер автономной системы (ASN) сети, используемой субъектом.|
|azureResourceId|Строка|Содержит полный идентификатор Azure Resource Manager для ресурса Azure, доступ к который был задан во время входа.|
|clientAppUsed|String|Устаревший клиент, используемый для действия входа. Например: , , , , `IMAP`, `MAPI`или `SMTP``POP`. `Modern clients``Exchange ActiveSync``Browser` Поддерживает ( `$filter` только`eq` оператор). |
|clientCredentialType|clientCredentialType|Описывает тип учетных данных, предоставленных клиентом или субъектом-службой Azure AD для проверки подлинности. Вы можете просмотреть clientCredentialType, чтобы отслеживать и устранять менее безопасные типы учетных данных или отслеживать клиенты и субъекты-службы с использованием аномальных типов учетных данных. Возможные значения: `none`, `clientSecret`, `clientAssertion`, `federatedIdentityCredential`, `managedIdentity`, `certificate`, `unknownFutureValue`.|
|conditionalAccessStatus|conditionalAccessStatus| Состояние активируемой политики условного доступа. Возможные значения: `success`, `failure`, или `notApplied``unknownFutureValue`. Поддерживает ( `$filter` только`eq` оператор).|
|correlationId|String|Идентификатор, отправляемый от клиента при запуске входа. Он используется для устранения неполадок с соответствующим действием входа при вызове службы поддержки. Поддерживает ( `$filter` только`eq` оператор).|
|createdDateTime|DateTimeOffset|Дата и время инициации входа. Тип Timestamp всегда представлен в формате времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает и `$orderby` `$filter` (`eq`и `le`только операторы `ge` ).|
|crossTenantAccessType|signInAccessType|Описывает тип межтенантного доступа, используемого субъектом для доступа к ресурсу. Возможные значения: `none`, `b2bCollaboration`, `b2bDirectConnect`, `microsoftSupport`, `serviceProvider`, `unknownFutureValue`. Если вход не пересекал границы клиента, значение равно `none`.|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения об устройстве, с которого выполнен вход. Включает такие сведения, как deviceId, ОС и браузер. Поддерживает (`$filter``eq`и `startsWith` только операторы) в **свойствах браузера** и **операционной** системы.|
|federatedCredentialId|Строка|Содержит идентификатор учетных данных федеративного удостоверения приложения, если для входа использовались учетные данные федеративного удостоверения.|
|flaggedForReview|Логическое|Во время неудачного входа пользователь может нажать кнопку в портал Azure, чтобы пометить событие сбоя для администраторов клиента. Если пользователь нажимает кнопку, чтобы пометить неудачный вход, это значение равно `true`.|
|homeTenantId|Строка|Идентификатор клиента пользователя, инициируемого входом. Неприменимо при входе в управляемое удостоверение или субъект-службу.|
|homeTenantName|Строка|Для входа пользователя — идентификатор клиента, членом которого является пользователь. Заполняется только в случаях, когда домашний клиент предоставил согласие на предоставление согласия Azure AD для отображения содержимого клиента.|
|id|Строка|Идентификатор, представляющий действие входа. Наследуется от [сущности](entity.md). Поддерживает ( `$filter` только`eq` оператор).|
|incomingTokenType|incomingTokenType|Указывает типы токенов, которые были Azure AD для проверки подлинности субъекта во время входа. Допустимые значения: `none`, `primaryRefreshToken`, `saml11`, `saml20`, `unknownFutureValue`, `remoteDesktopToken`. <br><br> **Обратите** Azure AD, что для проверки подлинности субъекта также использовались типы маркеров, не перечисленные в этом типе перечисления. Не выведите отсутствие маркера, если он не является одним из перечисленных типов. Кроме того, обратите внимание, что для `Prefer: include-unknown-enum-members` получения следующих значений в этом развиваемом перечислении необходимо использовать заголовок [запроса](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). `remoteDesktopToken`|
|ipAddress|String|IP-адрес клиента, с которого выполнен вход. Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|ipAddressFromResourceProvider|Строка|IP-адрес, используемый пользователем для доступа к поставщику ресурсов, используемый для определения соответствия условного доступа для некоторых политик. Например, когда пользователь взаимодействует с Exchange Online, здесь может быть записан EXCHANGE, получаемый от пользователя. Это значение часто бывает `null`.|
|isInteractive|Boolean|Указывает, является ли вход пользователя интерактивным. При интерактивном входе пользователь предоставляет фактор проверки подлинности для Azure AD. К этим факторам относятся пароли, ответы на запросы MFA, биометрические факторы или QR-коды, которые пользователь предоставляет Azure AD или связанному приложению. При неинтерактивном входе пользователь не предоставляет фактор проверки подлинности. Вместо этого клиентское приложение использует маркер или код для проверки подлинности или доступа к ресурсу от имени пользователя. Неинтерактивные входы обычно используются для входа клиента от имени пользователя в процессе, прозрачном для пользователя.|
|isTenantRestricted|Логическое|Показывает, применяется ли к событию входа политика Azure AD клиента.|
|location|[signInLocation](signinlocation.md)|Город, штат и двухбуквенный код страны, из которой выполнен вход. Поддерживает (`$filter``eq`и `startsWith` только операторы) в **свойствах city**, **state** и **countryOrRegion**.|
|networkLocationDetails|Коллекция [networkLocationDetail](networklocationdetail.md)|Сведения о сетевом расположении, включая тип используемой сети и ее имена.|
|originalRequestId|String|Идентификатор первого запроса в последовательности проверки подлинности. Поддерживает ( `$filter` только`eq` оператор).|
|privateLinkDetails|[privateLinkDetails](../resources/privatelinkdetails.md)|Содержит сведения о политике Azure AD Приватный канал, связанной с событием входа.|
|processingTimeInMilliseconds|Int|Время обработки запроса в миллисекундах в службе маркеров безопасности AD.|
|resourceDisplayName|Строка|Имя ресурса, в который пользователь выполнил вход. Поддерживает ( `$filter` только`eq` оператор).|
|resourceId|String|Идентификатор ресурса, в который пользователь выполнил вход. Поддерживает ( `$filter` только`eq` оператор).|
|resourceServicePrincipalId|Строка|Идентификатор субъекта-службы, представляющего целевой ресурс в событии входа.|
|resourceTenantId|Строка|Идентификатор клиента ресурса, на который ссылаются во время входа.|
|riskDetail|riskDetail|Причина определенного состояния пользователя, входа или события риска. Возможные значения: `none`, , `userPerformedSecuredPasswordChange``adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, , `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`или `adminConfirmedSigninCompromised``unknownFutureValue`. Значение `none` означает, что действия для пользователя или входа пока не выполнялись. Поддерживает ( `$filter` только`eq` оператор).<br> **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Возвращаются все остальные клиенты `hidden`.|
|riskEventTypes_v2|Коллекция строк|Список типов событий риска, связанных со входом. Возможные значения: `unlikelyTravel`, , `maliciousIPAddress``anonymizedIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, , `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`или `generic``unknownFutureValue`. Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|riskLevelAggregated|riskLevel|Совокупный уровень риска. Возможные значения: `none`, `low`, `medium`, , `high`, или `unknownFutureValue``hidden`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. Поддерживает ( `$filter` только`eq` оператор). <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Возвращаются все остальные клиенты `hidden`.|
|riskLevelDuringSignIn|riskLevel|Уровень риска во время входа. Возможные значения: `none`, `low`, `medium`, , `high`, или `unknownFutureValue``hidden`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. Поддерживает ( `$filter` только`eq` оператор). <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Возвращаются все остальные клиенты `hidden`.|
|riskState|riskState|Состояние риска пользователя, входа или события риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, , `atRisk`, или `unknownFutureValue``confirmedCompromised`. Поддерживает ( `$filter` только`eq` оператор).|
|servicePrincipalCredentialKeyId|Строка|Уникальный идентификатор учетных данных ключа, используемых субъектом-службой для проверки подлинности.|
|servicePrincipalCredentialThumbprint|Строка|Отпечаток сертификата, используемого субъектом-службой для проверки подлинности.|
|servicePrincipalId|Строка|Идентификатор приложения, используемый для входа. Это поле заполняется при входе с помощью приложения. Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|servicePrincipalName|String|Имя приложения, используемого для входа. Это поле заполняется при входе с помощью приложения. Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|sessionLifetimePolicies|[Коллекция sessionLifetimePolicy](sessionlifetimepolicy.md)|Все политики управления сеансами условного доступа, которые были применены во время события входа.|
|signInEventTypes|Коллекция строк|Указывает категорию входа, которую представляет событие. Для входа пользователя `interactiveUser` `nonInteractiveUser` категория может быть или соответствовать значению свойства **isInteractive** в ресурсе входа. Для входов с управляемым удостоверением используется категория `managedIdentity`. Для входа субъекта-службы категория **— servicePrincipal**. Возможные значения: `interactiveUser`, `nonInteractiveUser`, `servicePrincipal`, `managedIdentity`, `unknownFutureValue`. Поддерживает `$filter` (`eq`, `ne`).|
|signInIdentifier|Строка|Идентификация, предоставленная пользователем для входа. Это может быть userPrincipalName, но оно также заполняется при входе пользователя с использованием других идентификаторов.|
|signInIdentifierType|signInIdentifierType|Тип идентификатора входа. Возможные значения: `userPrincipalName`, `phoneNumber`, `proxyAddress`, `qrCode`, `onPremisesUserPrincipalName`, `unknownFutureValue`.|
|status|[signInStatus](signinstatus.md)|Состояние входа. Включает код ошибки и описание ошибки (в случае сбоя входа). Поддерживает ( `$filter` только`eq` оператор) для **свойства errorCode** .|
|tokenIssuerName|String|Имя поставщика удостоверений. Например, `sts.microsoft.com`. Поддерживает ( `$filter` только`eq` оператор).|
|tokenIssuerType|tokenIssuerType|Тип поставщика удостоверений. Допустимые значения: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`, `AzureADBackupAuth`, `ADFederationServicesMFAAdapter`, `NPSExtension`. Обратите внимание, что необходимо использовать `Prefer: include-unknown-enum-members` заголовок запроса для получения следующих значений в этом развиваемом перечислении[:](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`AzureADBackupAuth` , , . `ADFederationServicesMFAAdapter` `NPSExtension`|
|uniqueTokenIdentifier|Строка|Уникальный идентификатор запроса в кодировке Base64, используемый для отслеживания маркеров, выданных Azure AD при их активации у поставщиков ресурсов. |
|Useragent|Строка|Сведения об агенте пользователя, связанные со входом. Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|userDisplayName|String|Отображаемое имя пользователя. Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|userId|String|Идентификатор пользователя. Поддерживает ( `$filter` только`eq` оператор).|
|userPrincipalName|String|Имя участника-пользователя пользователя. Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|userType|signInUserType|Определяет, является ли пользователь участником или гостем в клиенте. Возможные значения: `member`, `guest`, `unknownFutureValue`.|
|mfaDetail (не рекомендуется)|Строка|Это свойство является устаревшим.|


## <a name="relationships"></a>Связи
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
  "authenticationContextClassReferences": [{"@odata.type": "microsoft.graph.authenticationContext"}],
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
  "azureResourceId": "String",
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "crossTenantAccessType": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "federatedCredentialId": "String",
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
  "sessionLifetimePolicies": [{"@odata.type": "microsoft.graph.sessionLifetimePolicy"}],
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
