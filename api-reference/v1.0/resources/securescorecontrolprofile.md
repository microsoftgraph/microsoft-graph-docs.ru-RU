---
title: secureScoreControlProfile type
description: Представляет безопасную оценку клиента на данные управления. По умолчанию он возвращает все элементы управления для клиента и может явно тянуть отдельные элементы управления.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 856ed0ca50a2aadb6945f5213de2f4b0f9ac286a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084106"
---
# <a name="securescorecontrolprofile-resource-type"></a>secureScoreControlProfile type

Пространство имен: microsoft.graph

Представляет безопасную оценку клиента на данные управления. По умолчанию он возвращает все элементы управления для клиента и может явно тянуть отдельные элементы управления.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) | [secureScoreControlProfile](securescorecontrolprofile.md) |Чтение свойств и метаданных объекта secureScoreControlProfiles.|
|[Получение объектов secureScoreControlProfile](../api/securescorecontrolprofile-get.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Чтение свойств и метаданных объекта secureScoreControlProfiles.|
|[Обновление securescorecontrolprofile](../api/securescorecontrolprofile-update.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Обновление объекта securescorecontrolprofile. |


## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|id|String|GUID или уникальный идентификатор, созданный поставщиком. Только для чтения. Обязательный.|
|azureTenantId|String|Строка GUID для ID клиента.|
|actionType|String|Тип действия управления (Config, Review, Behaviour).|
|actionUrl|Строка|URL-адрес, в котором можно использовать управление. |
|controlCategory|Строка|Категория действия управления (Identity, Data, Device, Apps, Infrastructure).|
|title|String|Название управления.|
|deprecated|Boolean|Флаг, чтобы указать, амортизации управления.|
|implementationCost|Строка|Затраты ресурсов на неопроверяющий контроль (низкий, умеренный, высокий).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения объекта профилей управления. Тип Timestamp представляет дату и время| 
|maxScore|Двойное с плавающей точкой|максимальная достижимая оценка для управления.|
|rank|Int32|Рейтинг управления стеком Майкрософт.|
|исправление|Строка|Описание того, что поможет исправлению этого управления.|
|remediationImpact|Строка|Описание влияния на пользователей исправлений.|
|service|String|Служба, которая владеет управлением (Exchange, Sharepoint, Azure AD).|
|угрозы|Коллекция String|Список угроз, которые устраняет управление (accountBreach, dataDeletion, dataExfiltration, dataSpillage,
elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling,spoofing).|
|tier|Строка|Уровень управления (Core, Defense in Depth, Advanced.)   |
|userImpact|Строка|Влияние пользователя на реализацию управления (низкий, умеренный, высокий).   |
|complianceInformation|[коллекция complianceInformation](complianceinformation.md)|Сбор сведений о соответствии требованиям, связанных с безопасным управлением счетами|
|controlStateUpdates|[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection|Флаг, чтобы указать, где у клиента отмечено управление (проигнорировано, thirdParty, рассмотрено) (поддерживает [обновление).](../api/securescorecontrolprofile-update.md)|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий сведения о поставщике продукта и службы безопасности, поставщике и подпрограмме (например, vendor=Microsoft; provider=SecureScore). Обязательный.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "id": "String (identifier)",
  "azureTenantId": "String",
  "actionType": "String",
  "actionUrl": "String",
  "controlCategory": "String",
  "title": "String", 
  "deprecated": "Boolean",
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": "Int32",
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": ["String"],
  "tier": "String",
  "userImpact": "String",
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}], 
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

