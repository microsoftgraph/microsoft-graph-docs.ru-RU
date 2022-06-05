---
title: Тип ресурса secureScoreControlProfile
description: Представляет оценку безопасности клиента для каждого контрольного данных. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6c54901018dcb6eccf36be2f6f4b0fc1c7d9da8d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899836"
---
# <a name="securescorecontrolprofile-resource-type"></a>Тип ресурса secureScoreControlProfile

Пространство имен: microsoft.graph

Представляет оценку безопасности клиента для каждого контрольного данных. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.


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
|azureTenantId|String|Строка GUID для идентификатора клиента.|
|actionType|String|Тип действия элемента управления (Config, Review, Behavior).|
|actionUrl|Строка|URL-адрес, по которому можно выполнить действие элемента управления. |
|controlCategory|Строка|Категория действий управления (удостоверение, данные, устройство, приложения, инфраструктура).|
|title|Строка|Заголовок элемента управления.|
|Устаревшие|Boolean|Флаг, указывающий, является ли элемент управления нерекомендуемым.|
|implementationCost|Строка|Затраты на ресурсы для управления имлемментациями (низкая, средняя, высокая).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения сущности профиля элемента управления. Тип метки времени представляет дату и время| 
|maxScore|Двойное с плавающей точкой|максимальная достижимая оценка для элемента управления.|
|rank|Int32|Рейтинг элементов управления в стеке корпорации Майкрософт.|
|Исправления|Строка|Описание того, что поможет устранить элемент управления.|
|remediationImpact|Строка|Описание влияния на пользователей исправления.|
|service|String|Служба, владеющую элементом управления (Exchange, Sharepoint, Azure AD).|
|Угроз|Коллекция объектов string|Список угроз, которые устраняет элемент управления (accountBreach, dataDeletion, dataExfiltration, dataSpillage,
elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling, spoofing).|
|Уровня|Строка|Уровень управления (Core, Глубина защиты, Дополнительно.)   |
|userImpact|Строка|Влияние пользователя на реализацию контроля (низкий, средний, высокий).   |
|complianceInformation|[Коллекция complianceInformation](complianceinformation.md)|Коллекция сведений о соответствии требованиям, связанных с управлением оценкой безопасности|
|controlStateUpdates|[Коллекция secureScoreControlStateUpdate](securescorecontrolstateupdate.md)|Флаг, указывающий, где клиент помечал элемент управления (игнорируется, thirdParty, reviewed) (поддерживает [обновление](../api/securescorecontrolprofile-update.md)).|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий сведения о поставщике продукта или службы безопасности, поставщике и субпроидере (например, vendor=Microsoft; provider=SecureScore). Обязательный.|

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

