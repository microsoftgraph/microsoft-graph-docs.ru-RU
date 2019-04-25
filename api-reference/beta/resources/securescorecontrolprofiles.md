---
title: Тип ресурса Секурескореконтролпрофилес
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549176"
---
# <a name="securescorecontrolprofiles-resource-type"></a>Тип ресурса Секурескореконтролпрофилес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |Чтение свойств и метаданных объекта Секурескореконтролпрофилес.|


## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|   Азуретенантид   |   String  |   Строка GUID для идентификатора клиента.  |
|   Контролнаме |   String  |   Имя элемента управления. |
|   title   |   Строка  |   Название элемента управления.   |
| Комплианцеинформатион | Коллекция [комплианцеинформатион](complianceinformation.md) | Коллекция сведений о соответствии, связанных с контролем безопасности по показателю |
|   Контролкатегори |   String  |   Категория действий управления (учетная запись, данные, устройство, приложения, инфраструктура).  |
|   actionType  |   String  |   Тип действия управления (config, проверка, поведение). |
|   service |   String  |   Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD). |
|   Максскоре |  String  |   Текущий полученный максимальный показатель на указанную дату.   |
|   медленно |  String  |   Уровень управления (ядро, Глубокая защита, расширенная)    |
|   Усеримпакт |    String  | Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).    |
|   Имплементатионкост |    String  |   Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая). |
|   rank |  Int32   |   Ранжирование стека для элемента управления корпорации Майкрософт.   |
|   угроз |   Коллекция String   |   Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, Датаексфилтратион,,, elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена). |
|   устаревшие |    Логический |   Флаг, указывающий, является ли элемент управления амортизировано.   |
|   исправления |   String  |   Описание того, что будет исправлено элементом управления. |
|   Ремедиатионимпакт | String  |   Описание влияния на пользователей об исправлении. |
|   Актионурл | String  |   URL-адрес, по которому можно выполнить действия с элементом управления. |
|   Контролстатеупдатес |   Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md) |    Флаг, указывающий, где клиент пометил элемент управления (Ignore, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofiles-update.md)). |

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
