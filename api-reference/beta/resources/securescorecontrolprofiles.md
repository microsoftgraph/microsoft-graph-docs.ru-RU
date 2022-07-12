---
title: Тип ресурса secureScoreControlProfile
description: Представляет оценку безопасности клиента для каждого контрольного данных. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 4d401b4003ef8ce0a4384daf16a03ce9d2851694
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735952"
---
# <a name="securescorecontrolprofile-resource-type"></a>Тип ресурса secureScoreControlProfile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет оценку безопасности клиента для каждого контрольного данных. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [Коллекция secureScoreControlProfile](securescorecontrolprofiles.md) |Получение коллекции объектов secureScoreControlProfile.|


## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|   azureTenantId   |   String  |   Строка GUID для идентификатора клиента.  |
|   controlName |   String  |   Имя элемента управления. |
|   title   |   String  |   Заголовок элемента управления.   |
| complianceInformation | [Коллекция complianceInformation](complianceinformation.md) | Коллекция сведений о соответствии требованиям, связанных с управлением оценкой безопасности |
|   controlCategory |   String  |   Категория действий управления (учетная запись, данные, устройство, приложения, инфраструктура).  |
|   actionType  |   String  |   Тип действия элемента управления (Config, Review, Behavior). |
|   service |   String  |   Служба, владеющую элементом управления (Exchange, Sharepoint, Azure AD). |
|   maxScore |  String  |   Текущая полученная максимальная оценка за указанную дату.   |
|   Уровня |  String  |   Уровень управления (Core, Глубина защиты, Дополнительно.)    |
|   userImpact |    String  | Влияние пользователя на реализацию контроля (низкий, средний, высокий).    |
|   implementationCost |    String  |   Затраты на ресурсы для управления имлемментациями (низкая, средняя, высокая). |
|   rank |  Int32   |   Рейтинг элементов управления в стеке корпорации Майкрософт.   |
|   Угроз |   Коллекция String   |   Список угроз, которые устраняет элемент управления (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling, spoofing). |
|   Устаревшие |    Логическое |   Флаг, указывающий, является ли элемент управления нерекомендуемым.   |
|   Исправления |   String  |   Описание того, что поможет устранить элемент управления. |
|   remediationImpact | String  |   Описание влияния на пользователей исправления. |
|   actionUrl | String  |   URL-адрес, по которому можно выполнить действие элемента управления. |
|   controlStateUpdates | [Коллекция secureScoreControlStateUpdate](securescorecontrolstateupdate.md) |    Флаг, указывающий, где клиент помечал элемент управления (игнорировать, thirdParty, reviewed) (поддерживает [обновление](../api/securescorecontrolprofiles-update.md)). |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "title": "String",
  "azureTenantId": "String (identifier)",
  "maxScore": 1024.13,
  "actionType": "String",
  "service": "String",
  "tier": "String",
  "userImpact": "string",
  "implementationCost ": "String",
  "rank ": 100,
  "threats": ["string"],
  "deprecated ": false,
  "remediation": "String",
  "remediationImpact ": "String",
  "actionUrl": "String",
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}],
  "controlCategory": "string",
  "lastModifiedDateTime": "String (timestamp)"
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


