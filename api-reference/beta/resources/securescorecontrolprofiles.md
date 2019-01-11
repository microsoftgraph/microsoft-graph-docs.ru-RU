---
title: Тип ресурса secureScoreControlProfiles
description: Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.
localization_priority: Normal
ms.openlocfilehash: 866b2086ff5160744f848292cedf30c3cedf6daa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866222"
---
# <a name="securescorecontrolprofiles-resource-type"></a>Тип ресурса secureScoreControlProfiles

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |Чтение свойства и метаданные объекта secureScoreControlProfiles.|


## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|   azureTenantId   |   Строка  |   Идентификатор GUID строки для клиента.  |
|   ИмяЭлементаУправления |   Строка  |   Имя элемента управления. |
|   title   |   Строка  |   Заголовок элемента управления.   |
| complianceInformation | [complianceInformation](complianceinformation.md) коллекции | Коллекции данных соответствия требованиям, связанных с безопасного элемента управления счета |
|   controlCategory |   Строка  |   Категория действие элемента управления (учетная запись, данные, устройства, приложения, инфраструктуры).  |
|   actionType  |   String  |   Действие типа (Config, просмотр, поведение) элемента управления. |
|   service |   String  |   Службы, которому принадлежит элемент управления (Exchange, Sharepoint, Azure AD). |
|   maxScore |  Строка  |   Текущая платформа получить максимальный показатель на указанной даты.   |
|   уровень |  Строка  |   Уровень элемента управления (Core, защите подробно, Дополнительно.)    |
|   userImpact |    Строка  | Влияние пользователей реализации управления (низкий, средний, высокий).    |
|   implementationCost |    Строка  |   Стоимость ресурса элемента управления implemmentating (низкий, средний, высокий). |
|   rank |  Int32   |   Стек корпорации Майкрософт ранжирования элемента управления.   |
|   угрозы безопасности |   Коллекция строк   |   Список управления устраняет угрозы (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, спуфинг). |
|   устаревшие |    Логический |   Флаг, указывающий, если элемент управления амортизации.   |
|   исправление |   Строка  |   Описание элемента управления, какие представлены сведения о устранение. |
|   remediationImpact | Строка  |   Описание влияния на пользователей исправлению. |
|   actionUrl | Строка  |   URL-адрес, где элемент управления может быть actioned. |
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


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
