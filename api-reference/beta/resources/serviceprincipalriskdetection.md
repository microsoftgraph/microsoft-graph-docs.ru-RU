---
title: тип ресурса servicePrincipalRiskDetection
description: Представляет сведения о обнаруженном директоре службы риска в клиенте Azure AD.
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 63eb90a7147394eb6639083f7f965e8759262901
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519989"
---
# <a name="serviceprincipalriskdetection-resource-type"></a>тип ресурса servicePrincipalRiskDetection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о обнаруженных в клиенте Azure AD основных службах, которые могут быть обнаружены в опасности. Azure AD непрерывно оценивает риски на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем основным обнаружениям рисков службы в среде Azure AD.

Наследуется [от сущности](../resources/entity.md).

Дополнительные сведения о событиях риска см. в Azure Active Directory [Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection). 

>**Примечание:** Для использования API servicePrincipalRiskDetection необходимо иметь лицензию Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[List servicePrincipalRiskDetections](../api/identityprotectionroot-list-serviceprincipalriskdetections.md)|[коллекция servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md)|Список основных обнаружений рисков службы и их свойств.|
|[Get servicePrincipalRiskDetection](../api/serviceprincipalriskdetection-get.md)|[servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md)|Получите определенное основное обнаружение рисков службы и ее свойства.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|действие|activityType|Указывает тип активности, с чем связан обнаруженный риск.  Допустимые значения: `signin`, `unknownFutureValue`, `servicePrincipal`. Обратите внимание, что для `Prefer: include-unknown-enum-members` получения следующего значения(ы) в этом развиваемом переуме следует использовать загон [запроса](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `servicePrincipal`. |
|activityDateTime|DateTimeOffset|Дата и время возникновения рискованных действий. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|additionalInfo|Строка|Дополнительные сведения, связанные с обнаружением рисков. Это строковая величина представлена как объект JSON с избежавными кавычками. |
|appId|String|Уникальный идентификатор для связанного приложения.|
|correlationId|String|Корреляция ID действия входного знака, связанного с обнаружением рисков. Это свойство, `null` если обнаружение риска не связано с действием входного знака.|
|detectedDateTime|DateTimeOffset|Дата и время обнаружения риска. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|detectionTimingType|riskDetectionTimingType|Сроки обнаружения риска , будь то в режиме реального времени или в автономном режиме). Допустимые значения: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|String|Уникальный идентификатор обнаружения рисков. Наследуется [от сущности](../resources/entity.md).|
|ipAddress|String|Предоставляет IP-адрес клиента, откуда возник риск.|
|keyIds|Коллекция строк|Уникальный идентификатор (GUID) для учетных данных ключей, связанных с обнаружением рисков.|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления обнаружения рисков.|
|location|[signInLocation](signinlocation.md)|Расположение, откуда инициировался вход. |
|requestId|Строка|Запрос идентификатора действия входной записи, связанной с обнаружением рисков. Это свойство, `null` если обнаружение риска не связано с действием входного знака. Поддерживает `$filter` (`eq`).|
|riskDetail|riskDetail|Сведения об обнаружении риска. <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут возвращены `hidden`. <br/>Допустимые значения: `none`, `hidden`, `unknownFutureValue`, `adminConfirmedServicePrincipalCompromised`, `adminDismissedAllRiskForServicePrincipal`. Обратите внимание, что для `Prefer: include-unknown-enum-members` получения следующего значения (ы) [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`adminConfirmedServicePrincipalCompromised` `adminDismissedAllRiskForServicePrincipal`в этом развиваемом переуме.|
|riskEventType|Строка|Тип обнаруженного события риска. Возможные значения: `investigationsThreatIntelligence`, , `adminConfirmedServicePrincipalCompromised``generic`, , `suspiciousSignins``leakedCredentials``unknownFutureValue`. Поддерживает `$filter` (`eq`).|
|riskLevel|riskLevel|Уровень обнаруженного риска. <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут возвращены `hidden`. Допустимые значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Состояние обнаруженного доверителем или входной активностью. Допустимые значения: `none`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|servicePrincipalDisplayName|String|    Отображаемое имя для субъекта-службы.|
|servicePrincipalId|String|Уникальный идентификатор для субъекта-службы. Поддерживает `$filter` (`eq`).|
|source|String|Источник обнаружения рисков. Например, `identityProtection`.|
|tokenIssuerType|tokenIssuerType|Указывает тип эмитента маркеров для обнаруженного риска входного знака. Возможные значения: `AzureAD`, `UnknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipalRiskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalRiskDetection",
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
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String",
  "keyIds": [
    "String"
  ],
  "additionalInfo": "String"
}
```

