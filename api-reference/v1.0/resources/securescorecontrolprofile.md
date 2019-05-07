---
title: Тип ресурса Секурескореконтролпрофиле
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 7ea9550e7fc6417ac28e32acd1d95cb9178f7360
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629259"
---
# <a name="securescorecontrolprofile-resource-type"></a>Тип ресурса Секурескореконтролпрофиле

Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) | [Секурескореконтролпрофиле](securescorecontrolprofile.md) |Чтение свойств и метаданных объекта Секурескореконтролпрофилес.|
|[Получение Секурескореконтролпрофиле](../api/securescorecontrolprofile-get.md) | [секурескореконтролпрофиле](secureScoreControlProfile.md) |Чтение свойств и метаданных объекта Секурескореконтролпрофилес.|
|[Обновление секурескореконтролпрофиле](../api/securescorecontrolprofile-update.md) | [секурескореконтролпрофиле](securescorecontrolprofile.md) |Обновление объекта секурескореконтролпрофиле. |


## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|id|String|GUID или уникальный идентификатор, созданный поставщиком. Только для чтения. Обязательный атрибут.|
|azureTenantId|String|Строка GUID для идентификатора клиента.|
|actionType|String|Тип действия управления (config, проверка, поведение).|
|Актионурл|String|URL-адрес, по которому можно выполнить действия с элементом управления. |
|Контролкатегори|String|Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).|
|title|Строка|Название элемента управления.|
|устаревшие|Логический|Флаг, указывающий, является ли элемент управления амортизировано.|
|Имплементатионкост|String|Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения объекта профиля элемента управления. Тип timestamp представляет дату и время| 
|Максскоре|Двойное|максимальный достижимый показатель для элемента управления.|
|rank|Int32|Ранжирование стека для элемента управления корпорации Майкрософт.|
|исправления|String|Описание того, что будет исправлено элементом управления.|
|Ремедиатионимпакт|String|Описание влияния на пользователей об исправлении.|
|service|String|Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD).|
|угроз|Коллекция String|Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, удаление, Датаексфилтратион, удаление)
elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена).|
|медленно|String|Уровень управления (ядро, Глубокая защита, расширенная)   |
|Усеримпакт|String|Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).   |
|Комплианцеинформатион|Коллекция [комплианцеинформатион](complianceinformation.md)|Коллекция сведений о соответствии, связанных с контролем безопасности по показателю|
|Контролстатеупдатес|Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md)|Флаг, указывающий, где клиент пометил элемент управления (игнорируется, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofile-update.md)).|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий сведения о продукте, поставщике, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре). Обязательно.|

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
