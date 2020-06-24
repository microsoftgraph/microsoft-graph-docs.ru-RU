---
title: Тип ресурса Клаимсмаппингполици
description: Представляет политики сопоставления утверждений для протоколов WS — подача, SAML, OAuth 2,0 и OpenID Connect для маркеров, выданных определенным приложением.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a993043e9bfa8ec789316421066e16dd55f748af
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846322"
---
# <a name="claimsmappingpolicy-resource-type"></a>Тип ресурса Клаимсмаппингполици

Пространство имен: microsoft.graph

Представляет политики сопоставления утверждений для протоколов WS — подача, SAML, OAuth 2,0 и OpenID Connect для маркеров, выданных определенным приложением. Политики сопоставления утверждений можно использовать для:

- Выберите утверждения, включаемые в маркеры
- Создание типов утверждений, которые еще не существуют
- Выбор или изменение источника данных, выпущенных в определенных утверждениях  

Дополнительные сведения о сценариях и конфигурации [: Настройка утверждений, выпущенных в маркерах для определенного приложения в клиенте](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).

Наследуется от [стсполици](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание Клаимсмаппингполици](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [клаимсмаппингполици](claimsmappingpolicy.md) | Создание объекта Клаимсмаппингполици. |
| [Получение Клаимсмаппингполици](../api/claimsmappingpolicy-get.md) | [клаимсмаппингполици](claimsmappingpolicy.md) | Чтение свойств и связей объекта Клаимсмаппингполици. |
| [Перечисление типов ресурсов claimsMappingPolicy](../api/claimsmappingpolicy-list.md) | [клаимсмаппингполици](claimsmappingpolicy.md) | Чтение свойств и связей объектов КлаимсмаппингполиЦиес. |
| [Обновление Клаимсмаппингполици](../api/claimsmappingpolicy-update.md) | Нет | Обновление объекта Клаимсмаппингполици. |
| [Удаление Клаимсмаппингполици](../api/claimsmappingpolicy-delete.md) | Нет | Удаление объекта Клаимсмаппингполици. |
| [Список appliesTo](../api/claimsmappingpolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка Директорйобжектс, к которым применена эта политика. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|RDLC|Коллекция String| Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики. Ниже приведены дополнительные сведения о схеме JSON для этого свойства. Обязательный.|
|description|String| Описание для этой политики.|
|displayName|Строка| Отображаемое имя для этой политики. Обязательный элемент.|
|исорганизатиондефаулт|Boolean|Игнорировать это свойство. Политика сопоставления утверждений может применяться только к субъектам служб и не может быть настроена глобально для Организации.|

### <a name="properties-of-a-claims-mapping-policy-definition"></a>Свойства определения политики сопоставления утверждений

Свойства, приведенные ниже, формируют объект JSON, представляющий политику сопоставления утверждений. Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** . Ниже приведено несколько примеров определений.

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a>Пример: **Определение** для включения в маркеры кода EmployeeID и тенанткаунтри в качестве утверждений
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a>Пример: **Определение** , использующее преобразование утверждений
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
|Версия|Integer|Установите значение 1. Обязательный элемент.|
|инклудебасикклаимсет|Boolean|Если задано значение true, все утверждения в базовом наборе утверждений порождаются в маркерах, на которые влияет политика. Если задано значение false, утверждения в базовом наборе утверждений не входят в маркеры, если они не добавлены по отдельности в свойство Клаимссчема той же политики.|
|клаимссчема|Объект JSON|Определяет, какие утверждения присутствуют в маркерах, на которые влияет политика, а также базовый набор утверждений и основной набор утверждений. Для каждой записи схемы утверждений, определенной в этом свойстве, требуются определенные сведения. Укажите, откуда берутся данные (в виде значения или источника/идентификатора), и какие утверждения данные выдаются как (тип утверждения). Дополнительные сведения см. в статье [Определение клаимссчема](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).|
|клаимстрансформатион|Объект JSON| Определяет общие преобразования, которые можно применять к исходным данным для создания выходных данных для утверждений, указанных в Клаимссчема. Дополнительные сведения см. в статье [Определение клаимстрансформатион](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).|


## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Тег|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика. Только для чтения.|

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