---
title: тип ресурса relyingPartyDetailedSummary
description: Представляет надеющийся участник в AD FS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6e840c47ed5170f95929d686fe9ff94be54ea1ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962114"
---
# <a name="relyingpartydetailedsummary-resource-type"></a>тип ресурса relyingPartyDetailedSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет доверяемую сторону, настроенную с помощью служб Федерации Active Directory (AD FS), ее агрегированное использование и возможность переноса конфигурации доверяющих сторон в Azure Active Directory.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/relyingpartydetailedsummary-list.md) | [relyingPartyDetailedSummary](relyingpartydetailedsummary.md) | Извлечение списка **объектов relyingPartyDetailedSummary.** |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения. Уникальный идентификатор, созданный на уровне API.| 
|relyingPartyId|Строка|Этот идентификатор используется для идентификации сторон, которые полагаются на эту службу Федерации. Он используется при выдаче утверждений стороне, которая полагается.|
|serviceId|Строка|Уникально определяет лес Active Directory.|
|migrationStatus|migrationStatus| Указание на возможность перемещений приложения в Azure AD или требуется дополнительное исследование. Возможные значения: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.|
|migrationValidationDetails|Коллекция [keyValuePair](keyvaluepair.md)|Указывает все проверки проверки, которые были сделаны в сведениях о конфигурации приложений, чтобы оценить, готово ли приложение к перемещению в Azure AD.|
|relyingPartyName|Строка|Имя приложения или другого объекта в Интернете, использующего поставщика удостоверений для проверки подлинности пользователя, который хочет войти в систему.|
|failedSignInCount|Int64| Количество сбойных входов в службу Федерации Active Directory за указанный период. |
|replyUrls|Коллекция String|Указывает, где надеющийся участник ожидает получения маркера.|
|signInSuccessRate|Двойное с плавающей точкой|Количество успешных / (количество успешных и количество неудачных входов) в службе Федерации Active Directory за указанный период.|
|successfulSignInCount|Int64|Количество успешных входов в службу Федерации Active Directory.|
|totalSignInCount|Int64|Количество неудачных входов с неудачным входом в службу Федерации Active Directory в указанный период.|
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


