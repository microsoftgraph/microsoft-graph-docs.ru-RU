---
title: тип ресурса claimsMappingPolicy
description: Представляет политику, которая может контролировать срок службы маркера доступа, выданного Azure Active Directory (Azure AD).
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e15a99b5cc8d5f8a144cfc0cf438d146d442fd3a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444345"
---
# <a name="claimsmappingpolicy-resource-type"></a>тип ресурса claimsMappingPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политики сопоставления утверждений для протоколов WS-Fed, SAML, OAuth 2.0 и OpenID Connect для маркеров, выдаваемого конкретному приложению. Политики сопоставления утверждений можно использовать для:

- Выберите, какие утверждения включены в маркеры
- Создание типов утверждений, которые еще не существуют
- Выберите или измените источник данных, излучаемый в определенных утверждениях  

Дополнительные сведения о сценарии и конфигурации см. в материале [How to: Customize claims emitted in tokens for a specific app in a tenant.](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties)

Наследует [от stsPolicy](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание claimsMappingPolicy](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Создание объекта claimsMappingPolicy. |
| [Get claimsMappingPolicy](../api/claimsmappingpolicy-get.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Чтение свойств и связей объекта claimsMappingPolicy. |
| [Перечисление типов ресурсов claimsMappingPolicy](../api/claimsmappingpolicy-list.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Чтение свойств и связей объектов claimsMappingPolicies. |
| [Обновление утвержденийMappingPolicy](../api/claimsmappingpolicy-update.md) | Нет | Обновление объекта claimsMappingPolicy. |
| [Удаление утвержденийMappingPolicy](../api/claimsmappingpolicy-delete.md) | Нет | Удаление объекта claimsMappingPolicy. |
| [Список применяетсяTo](../api/claimsmappingpolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получите список directoryObjects, к которые была применена эта политика. |
| [Назначение типа ресурса claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md) | Нет | Назначьте объекту [servicePrincipal объект claimsMappingPolicy.](serviceprincipal.md) |
| [Список присвоенных утвержденийMappingPolicy](../api/serviceprincipal-list-claimsmappingpolicies.md) | Коллекция [claimsMappingPolicy](claimsmappingpolicy.md) | Список объектов claimsMappingPolicy, которые назначены [объекту servicePrincipal.](serviceprincipal.md) |
| [Удаление типа ресурса claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md) | Нет | Удалите claimsMappingPolicy из [объекта servicePrincipal.](serviceprincipal.md) |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|определение|Коллекция строк| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображение имени для этой политики. Обязательный.|
|isOrganizationDefault|Boolean|Игнорируйте это свойство. Политика сопоставления утверждений может применяться только к директорам служб и не может быть установлена глобально для организации.|

### <a name="properties-of-a-claims-mapping-policy-definition"></a>Свойства определения политики сопоставления утверждений

Свойства, представленные ниже, формируют объект JSON, который представляет политику сопоставления утверждений. Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.** Ниже показано несколько примеров определения:

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a>Пример: **определение** для того, чтобы включить EmployeeID и TenantCountry в качестве утверждений в маркерах
<!-- {
  "blockType": "ignored"
}-->
``` json
{
  "definition": [
    "{\"ClaimsMappingPolicy\":{
      \"Version\":1,
      \"IncludeBasicClaimSet\":\"true\", 
      \"ClaimsSchema\": [
        {\"Source\":\"user\",\"ID\":\"employeeid\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\",\"JwtClaimType\":\"name\"},{\"Source\":\"company\",\"ID\":\"tenantcountry\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/country\",\"JwtClaimType\":\"country\"}
        ]
      }
    }"
  ]
}
```

#### <a name="example-definition-that-uses-a-claims-transformation"></a>Пример: **определение,** использующее преобразование утверждений
<!-- {
  "blockType": "ignored"
}-->
``` json
{
  "definition": [
    "{\"ClaimsMappingPolicy\":{
      \"Version\":1,
      \"IncludeBasicClaimSet\":\"true\", 
      \"ClaimsSchema\":[
        {\"Source\":\"user\",\"ID\":\"extensionattribute1\"},{\"Source\":\"transformation\",\"ID\":\"DataJoin\",\"TransformationId\":\"JoinTheData\",\"JwtClaimType\":\"JoinedData\"}
        ],
      \"ClaimsTransformation\":[
        {\"ID\":\"JoinTheData\",\"TransformationMethod\":\"Join\",\"InputClaims\":[{\"ClaimTypeReferenceId\":\"extensionattribute1\",\"TransformationClaimType\":\"string1\"}], \"InputParameters\": [{\"ID\":\"string2\",\"Value\":\"sandbox\"},{\"ID\":\"separator\",\"Value\":\".\"}],\"OutputClaims\":[{\"ClaimTypeReferenceId\":\"DataJoin\",\"TransformationClaimType\":\"outputClaim\"}]}
        ]
      }
    }"
  ]
}
```

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Версия|Целое число|Значение 1. Обязательный.|
|IncludeBasicClaimSet|Boolean|Если установлено, что все утверждения в базовом наборе утверждений излучаются в маркерах, затронутых политикой. Если установлено ложное, утверждения в базовом наборе утверждений не находятся в маркерах, если они не добавляются отдельно в свойстве ClaimsSchema той же политики.|
|ClaimsSchema|Объект JSON|Определяет, какие утверждения присутствуют в маркерах, затронутых политикой, в дополнение к основному набору утверждений и набору основных утверждений. Для каждой записи схемы утверждения, определенной в этом свойстве, требуется определенная информация. Укажите, откуда приходят данные (пара Value или Source/ID) и какие утверждают, что данные излучаются как (Тип утверждения). Дополнительные сведения доступны в [определении ClaimsSchema.](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema)|
|ClaimsTransformation|Объект JSON| Определяет общие преобразования, которые можно применить к исходным данным, для создания данных вывода для утверждений, указанных в ClaimsSchema. Дополнительные сведения доступны в определении [ClaimsTransformation](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).|


## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|appliesTo|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject,](directoryObject.md) к которую была применена эта политика. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": false,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "claimsMappingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
