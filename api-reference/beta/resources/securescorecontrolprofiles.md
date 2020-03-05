---
title: Тип ресурса Секурескореконтролпрофиле
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7dfca5eedebe7f2fe524c79cee52e5855af7f291
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520866"
---
# <a name="securescorecontrolprofile-resource-type"></a>Тип ресурса Секурескореконтролпрофиле

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | Коллекция [секурескореконтролпрофиле](securescorecontrolprofiles.md) |Получение коллекции объектов Секурескореконтролпрофиле.|


## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|   azureTenantId   |   String  |   Строка GUID для идентификатора клиента.  |
|   контролнаме |   String  |   Имя элемента управления. |
|   title   |   Строка  |   Название элемента управления.   |
| комплианцеинформатион | Коллекция [комплианцеинформатион](complianceinformation.md) | Коллекция сведений о соответствии, связанных с контролем безопасности по показателю |
|   контролкатегори |   String  |   Категория действий управления (учетная запись, данные, устройство, приложения, инфраструктура).  |
|   actionType  |   String  |   Тип действия управления (config, проверка, поведение). |
|   service |   String  |   Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD). |
|   максскоре |  String  |   Текущий полученный максимальный показатель на указанную дату.   |
|   медленно |  String  |   Уровень управления (ядро, Глубокая защита, расширенная)    |
|   усеримпакт |    String  | Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).    |
|   имплементатионкост |    String  |   Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая). |
|   rank |  Int32   |   Ранжирование стека для элемента управления корпорации Майкрософт.   |
|   угроз |   Коллекция String   |   Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, Датаексфилтратион,,, elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена). |
|   устаревшие |    Логический |   Флаг, указывающий, является ли элемент управления амортизировано.   |
|   исправления |   String  |   Описание того, что будет исправлено элементом управления. |
|   ремедиатионимпакт | String  |   Описание влияния на пользователей об исправлении. |
|   актионурл | String  |   URL-адрес, по которому можно выполнить действия с элементом управления. |
|   контролстатеупдатес | Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md) |    Флаг, указывающий, где клиент пометил элемент управления (Ignore, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofiles-update.md)). |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) |

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
