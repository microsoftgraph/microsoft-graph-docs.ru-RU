---
title: Тип ресурса secureScoreControlProfiles
description: Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641612"
---
# <a name="securescorecontrolprofiles-resource-type"></a>Тип ресурса secureScoreControlProfiles

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |Чтение свойства и метаданные объекта secureScoreControlProfiles.|


## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|   azureTenantId   |   String  |   Идентификатор GUID строки для клиента.  |
|   ИмяЭлементаУправления |   String  |   Имя элемента управления. |
|   title   |   String  |   Заголовок элемента управления.   |
| complianceInformation | [complianceInformation](complianceinformation.md) коллекции | Коллекции данных соответствия требованиям, связанных с безопасного элемента управления счета |
|   controlCategory |   String  |   Категория действие элемента управления (учетная запись, данные, устройства, приложения, инфраструктуры).  |
|   actionType  |   String  |   Действие типа (Config, просмотр, поведение) элемента управления. |
|   service |   String  |   Службы, которому принадлежит элемент управления (Exchange, Sharepoint, Azure AD). |
|   maxScore |  String  |   Текущая платформа получить максимальный показатель на указанной даты.   |
|   уровень |  String  |   Уровень элемента управления (Core, защите подробно, Дополнительно.)    |
|   userImpact |    String  | Влияние пользователей реализации управления (низкий, средний, высокий).    |
|   implementationCost |    String  |   Стоимость ресурса элемента управления implemmentating (низкий, средний, высокий). |
|   rank |  Int32   |   Стек корпорации Майкрософт ранжирования элемента управления.   |
|   угрозы безопасности |   Коллекция String   |   Список управления устраняет угрозы (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, спуфинг). |
|   устаревшие |    Boolean |   Флаг, указывающий, если элемент управления амортизации.   |
|   исправление |   String  |   Описание элемента управления, какие представлены сведения о устранение. |
|   remediationImpact | String  |   Описание влияния на пользователей исправлению. |
|   actionUrl | String  |   URL-адрес, где элемент управления может быть actioned. |
|   controlStateUpdates |   [secureScoreControlStateUpdate](securescorecontrolstateupdate.md) коллекции |    Флаг, указывающий, где клиент отметил элемента управления (игнорировать, сторонних анализа) (поддерживает [обновление](../api/securescorecontrolprofiles-update.md)). |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
