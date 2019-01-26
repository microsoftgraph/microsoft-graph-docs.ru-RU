---
title: Тип ресурса secureScoreControlProfiles
description: Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576061"
---
# <a name="securescorecontrolprofiles-resource-type"></a>Тип ресурса secureScoreControlProfiles

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfile](securescorecontrolprofiles.md) |Чтение свойства и метаданные объекта secureScoreControlProfiles.|


## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|   azureTenantId   |   Строка  |   Идентификатор GUID строки для клиента.  |
|   ИмяЭлементаУправления |   Строка  |   Имя элемента управления. |
|   title   |   Строка  |   Заголовок элемента управления.   |
|   controlCategory |   Строка  |   Категория действие элемента управления (учетная запись, данные, устройства, приложения, инфраструктуры).  |
|   actionType  |   String  |   Действие типа (Config, просмотр, поведение) элемента управления. |
|   service |   String  |   Службы, которому принадлежит элемент управления (Exchange, Sharepoint, Azure AD). |
|   maxScore |  Double  |   Текущая платформа получить максимальный показатель на указанной даты.   |
|   уровень |  Строка  |   Уровень элемента управления (Core, защите подробно, Дополнительно.)    |
|   userImpact |    Строка  | Влияние пользователей реализации управления (низкий, средний, высокий).    |
|   implementationCost |    Строка  |   Стоимость ресурса элемента управления implemmentating (низкий, средний, высокий). |
|   rank |  Int32   |   Стек корпорации Майкрософт ранжирования элемента управления.   |
|   угрозы безопасности |   Коллекция строк   |   Список управления устраняет угрозы (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, спуфинг). |
|   устаревшие |    Boolean |   Флаг, указывающий, если элемент управления амортизации.   |
|   исправление |   Строка  |   Описание элемента управления, какие представлены сведения о устранение. |
|   remediationImpact | Строка  |   Описание влияния на пользователей исправлению. |
|   actionUrl | Строка  |   URL-адрес, где элемент управления может быть actioned. |
|   lastModifiedDateTime |  String (DateTimeOffset) |   Дата последнего изменения |
|   controlStateUpdates |   [secureScoreControlStateUpdate](securescorecontrolstateupdate.md) коллекции |  Флаг, указывающий, где клиент отметил элемента управления (игнорировать, сторонних анализа) (поддерживает [обновление](../api/securescorecontrolprofiles-update.md)). |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).|

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
    "title": "String", 
    "azureTenantId": "String (identifier)", 
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
