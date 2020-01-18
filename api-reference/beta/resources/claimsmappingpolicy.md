---
title: Тип ресурса Клаимсмаппингполици
description: Представляет политику, которая может управлять временем существования маркера доступа, выданного Azure Active Directory (Azure AD).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8fe6ca32e606829f12400a03a70c9fb783f32f77
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234518"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="0c5cd-103">Тип ресурса Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="0c5cd-103">claimsMappingPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c5cd-104">Представляет политики сопоставления утверждений для протоколов WS — подача, SAML, OAuth 2,0 и OpenID Connect для маркеров, выданных определенным приложением.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-104">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="0c5cd-105">Политики сопоставления утверждений можно использовать для:</span><span class="sxs-lookup"><span data-stu-id="0c5cd-105">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="0c5cd-106">Выберите утверждения, включаемые в маркеры</span><span class="sxs-lookup"><span data-stu-id="0c5cd-106">Select which claims are included in tokens</span></span>
- <span data-ttu-id="0c5cd-107">Создание типов утверждений, которые еще не существуют</span><span class="sxs-lookup"><span data-stu-id="0c5cd-107">Create claim types that do not already exist</span></span>
- <span data-ttu-id="0c5cd-108">Выбор или изменение источника данных, выпущенных в определенных утверждениях</span><span class="sxs-lookup"><span data-stu-id="0c5cd-108">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="0c5cd-109">Дополнительные сведения о сценариях и конфигурации [: Настройка утверждений, выпущенных в маркерах для определенного приложения в клиенте](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span><span class="sxs-lookup"><span data-stu-id="0c5cd-109">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="0c5cd-110">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c5cd-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0c5cd-111">Методы</span><span class="sxs-lookup"><span data-stu-id="0c5cd-111">Methods</span></span>

| <span data-ttu-id="0c5cd-112">Метод</span><span class="sxs-lookup"><span data-stu-id="0c5cd-112">Method</span></span>       | <span data-ttu-id="0c5cd-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c5cd-113">Return Type</span></span> | <span data-ttu-id="0c5cd-114">Описание</span><span class="sxs-lookup"><span data-stu-id="0c5cd-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0c5cd-115">Создание Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="0c5cd-115">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="0c5cd-116">клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="0c5cd-116">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="0c5cd-117">Создание объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-117">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="0c5cd-118">Получение Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="0c5cd-118">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="0c5cd-119">клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="0c5cd-119">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="0c5cd-120">Чтение свойств и связей объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-120">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="0c5cd-121">Список КлаимсмаппингполиЦиес</span><span class="sxs-lookup"><span data-stu-id="0c5cd-121">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="0c5cd-122">клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="0c5cd-122">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="0c5cd-123">Чтение свойств и связей объектов КлаимсмаппингполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-123">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="0c5cd-124">Обновление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="0c5cd-124">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="0c5cd-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0c5cd-125">None</span></span> | <span data-ttu-id="0c5cd-126">Обновление объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-126">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="0c5cd-127">Удаление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="0c5cd-127">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="0c5cd-128">Нет</span><span class="sxs-lookup"><span data-stu-id="0c5cd-128">None</span></span> | <span data-ttu-id="0c5cd-129">Удаление объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-129">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="0c5cd-130">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="0c5cd-130">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="0c5cd-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="0c5cd-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="0c5cd-132">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="0c5cd-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c5cd-133">Properties</span></span>

| <span data-ttu-id="0c5cd-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c5cd-134">Property</span></span>     | <span data-ttu-id="0c5cd-135">Тип</span><span class="sxs-lookup"><span data-stu-id="0c5cd-135">Type</span></span>        | <span data-ttu-id="0c5cd-136">Описание</span><span class="sxs-lookup"><span data-stu-id="0c5cd-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c5cd-137">id</span><span class="sxs-lookup"><span data-stu-id="0c5cd-137">id</span></span>|<span data-ttu-id="0c5cd-138">String</span><span class="sxs-lookup"><span data-stu-id="0c5cd-138">String</span></span>| <span data-ttu-id="0c5cd-139">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-139">Unique identifier for this policy.</span></span> <span data-ttu-id="0c5cd-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-140">Read-only.</span></span>|
|<span data-ttu-id="0c5cd-141">RDLC</span><span class="sxs-lookup"><span data-stu-id="0c5cd-141">definition</span></span>|<span data-ttu-id="0c5cd-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0c5cd-142">String collection</span></span>| <span data-ttu-id="0c5cd-143">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="0c5cd-144">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="0c5cd-145">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-145">Required.</span></span>|
|<span data-ttu-id="0c5cd-146">description</span><span class="sxs-lookup"><span data-stu-id="0c5cd-146">description</span></span>|<span data-ttu-id="0c5cd-147">String</span><span class="sxs-lookup"><span data-stu-id="0c5cd-147">String</span></span>| <span data-ttu-id="0c5cd-148">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-148">Description for this policy.</span></span>|
|<span data-ttu-id="0c5cd-149">displayName</span><span class="sxs-lookup"><span data-stu-id="0c5cd-149">displayName</span></span>|<span data-ttu-id="0c5cd-150">Строка</span><span class="sxs-lookup"><span data-stu-id="0c5cd-150">String</span></span>| <span data-ttu-id="0c5cd-151">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-151">Display name for this policy.</span></span> <span data-ttu-id="0c5cd-152">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-152">Required.</span></span>|
|<span data-ttu-id="0c5cd-153">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="0c5cd-153">isOrganizationDefault</span></span>|<span data-ttu-id="0c5cd-154">Логический</span><span class="sxs-lookup"><span data-stu-id="0c5cd-154">Boolean</span></span>|<span data-ttu-id="0c5cd-155">Игнорировать это свойство.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-155">Ignore this property.</span></span> <span data-ttu-id="0c5cd-156">Политика сопоставления утверждений может применяться только к субъектам служб и не может быть настроена глобально для Организации.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-156">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="0c5cd-157">Свойства определения политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="0c5cd-157">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="0c5cd-158">Свойства, приведенные ниже, формируют объект JSON, представляющий политику сопоставления утверждений.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-158">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="0c5cd-159">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="0c5cd-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="0c5cd-160">Ниже приведено несколько примеров определений.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-160">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="0c5cd-161">Пример: **Определение** для включения в маркеры кода EmployeeID и тенанткаунтри в качестве утверждений</span><span class="sxs-lookup"><span data-stu-id="0c5cd-161">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="0c5cd-162">Пример: **Определение** , использующее преобразование утверждений</span><span class="sxs-lookup"><span data-stu-id="0c5cd-162">Example: **definition** that uses a claims transformation</span></span>
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

| <span data-ttu-id="0c5cd-163">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c5cd-163">Property</span></span>     | <span data-ttu-id="0c5cd-164">Тип</span><span class="sxs-lookup"><span data-stu-id="0c5cd-164">Type</span></span>   |<span data-ttu-id="0c5cd-165">Описание</span><span class="sxs-lookup"><span data-stu-id="0c5cd-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c5cd-166">Версия</span><span class="sxs-lookup"><span data-stu-id="0c5cd-166">Version</span></span>|<span data-ttu-id="0c5cd-167">Целое число</span><span class="sxs-lookup"><span data-stu-id="0c5cd-167">Integer</span></span>|<span data-ttu-id="0c5cd-168">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-168">Set value of 1.</span></span> <span data-ttu-id="0c5cd-169">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-169">Required.</span></span>|
|<span data-ttu-id="0c5cd-170">инклудебасикклаимсет</span><span class="sxs-lookup"><span data-stu-id="0c5cd-170">IncludeBasicClaimSet</span></span>|<span data-ttu-id="0c5cd-171">Логический</span><span class="sxs-lookup"><span data-stu-id="0c5cd-171">Boolean</span></span>|<span data-ttu-id="0c5cd-172">Если задано значение true, все утверждения в базовом наборе утверждений порождаются в маркерах, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-172">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="0c5cd-173">Если задано значение false, утверждения в базовом наборе утверждений не входят в маркеры, если они не добавлены по отдельности в свойство Клаимссчема той же политики.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-173">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="0c5cd-174">клаимссчема</span><span class="sxs-lookup"><span data-stu-id="0c5cd-174">ClaimsSchema</span></span>|<span data-ttu-id="0c5cd-175">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="0c5cd-175">JSON object</span></span>|<span data-ttu-id="0c5cd-176">Определяет, какие утверждения присутствуют в маркерах, на которые влияет политика, а также базовый набор утверждений и основной набор утверждений.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-176">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="0c5cd-177">Для каждой записи схемы утверждений, определенной в этом свойстве, требуются определенные сведения.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-177">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="0c5cd-178">Укажите, откуда берутся данные (в виде значения или источника/идентификатора), и какие утверждения данные выдаются как (тип утверждения).</span><span class="sxs-lookup"><span data-stu-id="0c5cd-178">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="0c5cd-179">Дополнительные сведения можно найти в [определении клаимссчема](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span><span class="sxs-lookup"><span data-stu-id="0c5cd-179">Further details are available in the [ClaimsSchema definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="0c5cd-180">клаимстрансформатион</span><span class="sxs-lookup"><span data-stu-id="0c5cd-180">ClaimsTransformation</span></span>|<span data-ttu-id="0c5cd-181">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="0c5cd-181">JSON object</span></span>| <span data-ttu-id="0c5cd-182">Определяет общие преобразования, которые можно применять к исходным данным для создания выходных данных для утверждений, указанных в Клаимссчема.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-182">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="0c5cd-183">Дополнительные сведения можно найти в [определении клаимстрансформатион](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="0c5cd-183">Further details are available in the [ClaimsTransformation definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="0c5cd-184">Связи</span><span class="sxs-lookup"><span data-stu-id="0c5cd-184">Relationships</span></span>

| <span data-ttu-id="0c5cd-185">Связь</span><span class="sxs-lookup"><span data-stu-id="0c5cd-185">Relationship</span></span> | <span data-ttu-id="0c5cd-186">Тип</span><span class="sxs-lookup"><span data-stu-id="0c5cd-186">Type</span></span>        | <span data-ttu-id="0c5cd-187">Описание</span><span class="sxs-lookup"><span data-stu-id="0c5cd-187">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c5cd-188">Тег</span><span class="sxs-lookup"><span data-stu-id="0c5cd-188">appliesTo</span></span>|<span data-ttu-id="0c5cd-189">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="0c5cd-189">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="0c5cd-190">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-190">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="0c5cd-191">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-191">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c5cd-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c5cd-192">JSON representation</span></span>

<span data-ttu-id="0c5cd-193">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c5cd-193">The following is a JSON representation of the resource.</span></span>

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