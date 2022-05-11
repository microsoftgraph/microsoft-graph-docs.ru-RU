---
title: Тип ресурса claimsMappingPolicy
description: Представляет политику, которая может управлять временем существования маркера доступа, выданного Azure Active Directory (Azure AD).
ms.localizationpriority: medium
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f25d4f252c3bda6331a982f26b82cf4764a4ec7c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314615"
---
# <a name="claimsmappingpolicy-resource-type"></a>Тип ресурса claimsMappingPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политики сопоставления утверждений для протоколов WS-Fed, SAML, OAuth 2.0 и OpenID Подключение для маркеров, выданных конкретному приложению. Политики сопоставления утверждений можно использовать для:

- Выбор утверждений, включенных в маркеры
- Создание типов утверждений, которые еще не существуют
- Выбор или изменение источника данных, выдаваемого в определенных утверждениях

Количество утверждений и преобразований, которые можно добавить в политику сопоставления утверждений, ограничено уменьшением размера маркера. Все записи схемы утверждений или преобразования, обнаруженные после предела, игнорируются и включаются в выданный токен. Дополнительные сведения об ограничениях см. в разделе ["Свойства определения политики сопоставления утверждений".](#properties-of-a-claims-mapping-policy-definition)

Дополнительные сведения о сценарии и конфигурации см. в разделах "Тип политики сопоставления утверждений" и "Практическое руководство. Настройка утверждений, создаваемых в маркерах для конкретного приложения [в клиенте"](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).[](/azure/active-directory/develop/reference-claims-mapping-policy-type)

Наследуется от [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание claimsMappingPolicy](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Создайте объект claimsMappingPolicy. |
| [Получение claimsMappingPolicy](../api/claimsmappingpolicy-get.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Чтение свойств и связей объекта claimsMappingPolicy. |
| [Перечисление типов ресурсов claimsMappingPolicy](../api/claimsmappingpolicy-list.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Чтение свойств и связей объектов claimsMappingPolicies. |
| [Обновление claimsMappingPolicy](../api/claimsmappingpolicy-update.md) | Нет | Обновление объекта claimsMappingPolicy. |
| [Удаление claimsMappingPolicy](../api/claimsmappingpolicy-delete.md) | Нет | Удаление объекта claimsMappingPolicy. |
| **Объекты каталога** |  |  |
| [List appliesTo](../api/claimsmappingpolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка объектов directoryObject, к которым применена эта политика. |
| [Назначение типа ресурса claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md) | Нет | Назначьте claimsMappingPolicy [объекту servicePrincipal](serviceprincipal.md) . |
| [Перечисление назначенных claimsMappingPolicy](../api/serviceprincipal-list-claimsmappingpolicies.md) | Коллекция [claimsMappingPolicy](claimsmappingpolicy.md) | Список объектов claimsMappingPolicy, назначенных [объекту servicePrincipal](serviceprincipal.md) . |
| [Удаление типа ресурса claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md) | Нет | Удалите claimsMappingPolicy из [объекта servicePrincipal](serviceprincipal.md) . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|Определение|Коллекция String| Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики. Дополнительные сведения о схеме JSON для этого свойства см. ниже. Обязательный.|
|description|String| Описание этой политики.|
|displayName|String| Отображаемое имя для этой политики. Обязательно.|
|isOrganizationDefault|Boolean|Игнорируйте это свойство. Политика сопоставления утверждений может применяться только к субъектам-службам и не может быть глобально задана для организации.|

### <a name="properties-of-a-claims-mapping-policy-definition"></a>Свойства определения политики сопоставления утверждений

Приведенные ниже свойства формируют объект JSON, представляющий политику сопоставления утверждений. Этот объект JSON необходимо преобразовать **в** строку с escape-кавычками, чтобы вставить его в **свойство** определения. Ниже приведено несколько примеров определения.

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a>Пример. **Определение для** включаемой EmployeeID и TenantCountry в качестве утверждений в маркеры

<!-- {
  "blockType": "ignored"
}-->
``` json
{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\",\"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"employeeid\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\",\"JwtClaimType\":\"name\"},{\"Source\":\"company\",\"ID\":\"tenantcountry\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/country\",\"JwtClaimType\":\"country\"}]}}"
    ],
    "displayName": "Test1234"
}
```

#### <a name="example-definition-that-uses-a-claims-transformation"></a>Пример: **определение,** использующее преобразование утверждений

<!-- {
  "blockType": "ignored"
}-->
``` json
{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\",\"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"},{\"Source\":\"user\",\"ID\":\"givenname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname\"},{\"Source\":\"user\",\"ID\":\"displayname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\"},{\"Source\":\"user\",\"ID\":\"surname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname\"},{\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\":\"username\"}],\"ClaimsTransformation\":[{\"ID\":\"CreateTermsOfService\",\"TransformationMethod\":\"CreateStringClaim\",\"InputParameters\": [{\"ID\":\"value\",\"DataType\":\"string\", \"Value\":\"sandbox\"}],\"OutputClaims\":[{\"ClaimTypeReferenceId\":\"TOS\",\"TransformationClaimType\":\"createdClaim\"}]}]}}"
    ],
    "displayName": "Test1234"
}
```

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Версия|Целое число|Задайте значение 1. Обязательно.|
|IncludeBasicClaimSet|Boolean|Если задано значение , `true`все утверждения в базовом наборе утверждений выдаются в маркерах, затронутых политикой. Если задано значение " `false`, утверждения в базовом наборе утверждений не находятся в маркерах, если они не добавляются отдельно в свойство ClaimsSchema той же политики.|
|ClaimsSchema|Объект JSON|Определяет, какие утверждения присутствуют в маркерах, затронутых политикой, в дополнение к базовому набору утверждений и набору основных утверждений. Для каждой записи схемы утверждения, определенной в этом свойстве, требуются определенные сведения. Укажите, откуда поступают данные (пара "Значение" или "Источник/идентификатор") и какое утверждение создает данные как (тип утверждения). Не более 50 утверждений включаются в маркер через объект ClaimsSchema. Все записи схемы утверждений, обнаруженные после достигнутого ограничения, будут игнорироваться и не будут отображаться в выданном токене. Дополнительные сведения доступны в [определении ClaimsSchema](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).|
|ClaimsTransformation|Объект JSON| Определяет общие преобразования, которые могут применяться к исходным данным для создания выходных данных для утверждений, указанных в ClaimsSchema. Не более 50 преобразований включаются в маркер через объект ClaimsTransformation. Все преобразования, которые возникают после предела, будут игнорироваться и не будут отображаться в выданном токене. Дополнительные сведения о ClaimsTransformation и поддерживаемых функциях см. в разделе ["Преобразование утверждений"](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).|


## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|appliesTo|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject](directoryObject.md) , к которой была применена эта политика. Только для чтения.|

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
