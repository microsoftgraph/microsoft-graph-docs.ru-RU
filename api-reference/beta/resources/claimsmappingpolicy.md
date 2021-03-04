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
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="a489c-103">тип ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="a489c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a489c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a489c-105">Представляет политики сопоставления утверждений для протоколов WS-Fed, SAML, OAuth 2.0 и OpenID Connect для маркеров, выдаваемого конкретному приложению.</span><span class="sxs-lookup"><span data-stu-id="a489c-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="a489c-106">Политики сопоставления утверждений можно использовать для:</span><span class="sxs-lookup"><span data-stu-id="a489c-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="a489c-107">Выберите, какие утверждения включены в маркеры</span><span class="sxs-lookup"><span data-stu-id="a489c-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="a489c-108">Создание типов утверждений, которые еще не существуют</span><span class="sxs-lookup"><span data-stu-id="a489c-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="a489c-109">Выберите или измените источник данных, излучаемый в определенных утверждениях</span><span class="sxs-lookup"><span data-stu-id="a489c-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="a489c-110">Дополнительные сведения о сценарии и конфигурации см. в материале [How to: Customize claims emitted in tokens for a specific app in a tenant.](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties)</span><span class="sxs-lookup"><span data-stu-id="a489c-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="a489c-111">Наследует [от stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a489c-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a489c-112">Методы</span><span class="sxs-lookup"><span data-stu-id="a489c-112">Methods</span></span>

| <span data-ttu-id="a489c-113">Метод</span><span class="sxs-lookup"><span data-stu-id="a489c-113">Method</span></span>       | <span data-ttu-id="a489c-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a489c-114">Return Type</span></span> | <span data-ttu-id="a489c-115">Описание</span><span class="sxs-lookup"><span data-stu-id="a489c-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a489c-116">Создание claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="a489c-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="a489c-118">Создание объекта claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="a489c-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="a489c-119">Get claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="a489c-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="a489c-121">Чтение свойств и связей объекта claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="a489c-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="a489c-122">Перечисление типов ресурсов claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="a489c-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="a489c-124">Чтение свойств и связей объектов claimsMappingPolicies.</span><span class="sxs-lookup"><span data-stu-id="a489c-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="a489c-125">Обновление утвержденийMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="a489c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="a489c-126">None</span></span> | <span data-ttu-id="a489c-127">Обновление объекта claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="a489c-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="a489c-128">Удаление утвержденийMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="a489c-129">Нет</span><span class="sxs-lookup"><span data-stu-id="a489c-129">None</span></span> | <span data-ttu-id="a489c-130">Удаление объекта claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="a489c-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="a489c-131">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="a489c-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="a489c-132">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a489c-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="a489c-133">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="a489c-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="a489c-134">Назначение типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-134">Assign claimsMappingPolicy</span></span>](../api/serviceprincipal-post-claimsmappingpolicies.md) | <span data-ttu-id="a489c-135">Нет</span><span class="sxs-lookup"><span data-stu-id="a489c-135">None</span></span> | <span data-ttu-id="a489c-136">Назначьте объекту [servicePrincipal объект claimsMappingPolicy.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="a489c-136">Assign a claimsMappingPolicy to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="a489c-137">Список присвоенных утвержденийMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-137">List assigned claimsMappingPolicy</span></span>](../api/serviceprincipal-list-claimsmappingpolicies.md) | <span data-ttu-id="a489c-138">Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a489c-138">[claimsMappingPolicy](claimsmappingpolicy.md) collection</span></span> | <span data-ttu-id="a489c-139">Список объектов claimsMappingPolicy, которые назначены [объекту servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="a489c-139">List the claimsMappingPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="a489c-140">Удаление типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a489c-140">Remove claimsMappingPolicy</span></span>](../api/serviceprincipal-delete-claimsmappingpolicies.md) | <span data-ttu-id="a489c-141">Нет</span><span class="sxs-lookup"><span data-stu-id="a489c-141">None</span></span> | <span data-ttu-id="a489c-142">Удалите claimsMappingPolicy из [объекта servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="a489c-142">Remove a claimsMappingPolicy from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a489c-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="a489c-143">Properties</span></span>

| <span data-ttu-id="a489c-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="a489c-144">Property</span></span>     | <span data-ttu-id="a489c-145">Тип</span><span class="sxs-lookup"><span data-stu-id="a489c-145">Type</span></span>        | <span data-ttu-id="a489c-146">Описание</span><span class="sxs-lookup"><span data-stu-id="a489c-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a489c-147">id</span><span class="sxs-lookup"><span data-stu-id="a489c-147">id</span></span>|<span data-ttu-id="a489c-148">String</span><span class="sxs-lookup"><span data-stu-id="a489c-148">String</span></span>| <span data-ttu-id="a489c-149">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a489c-149">Unique identifier for this policy.</span></span> <span data-ttu-id="a489c-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a489c-150">Read-only.</span></span>|
|<span data-ttu-id="a489c-151">определение</span><span class="sxs-lookup"><span data-stu-id="a489c-151">definition</span></span>|<span data-ttu-id="a489c-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a489c-152">String collection</span></span>| <span data-ttu-id="a489c-153">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.</span><span class="sxs-lookup"><span data-stu-id="a489c-153">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="a489c-154">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="a489c-154">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="a489c-155">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a489c-155">Required.</span></span>|
|<span data-ttu-id="a489c-156">description</span><span class="sxs-lookup"><span data-stu-id="a489c-156">description</span></span>|<span data-ttu-id="a489c-157">String</span><span class="sxs-lookup"><span data-stu-id="a489c-157">String</span></span>| <span data-ttu-id="a489c-158">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="a489c-158">Description for this policy.</span></span>|
|<span data-ttu-id="a489c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a489c-159">displayName</span></span>|<span data-ttu-id="a489c-160">String</span><span class="sxs-lookup"><span data-stu-id="a489c-160">String</span></span>| <span data-ttu-id="a489c-161">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a489c-161">Display name for this policy.</span></span> <span data-ttu-id="a489c-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a489c-162">Required.</span></span>|
|<span data-ttu-id="a489c-163">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="a489c-163">isOrganizationDefault</span></span>|<span data-ttu-id="a489c-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="a489c-164">Boolean</span></span>|<span data-ttu-id="a489c-165">Игнорируйте это свойство.</span><span class="sxs-lookup"><span data-stu-id="a489c-165">Ignore this property.</span></span> <span data-ttu-id="a489c-166">Политика сопоставления утверждений может применяться только к директорам служб и не может быть установлена глобально для организации.</span><span class="sxs-lookup"><span data-stu-id="a489c-166">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="a489c-167">Свойства определения политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="a489c-167">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="a489c-168">Свойства, представленные ниже, формируют объект JSON, который представляет политику сопоставления утверждений.</span><span class="sxs-lookup"><span data-stu-id="a489c-168">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="a489c-169">Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.**</span><span class="sxs-lookup"><span data-stu-id="a489c-169">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="a489c-170">Ниже показано несколько примеров определения:</span><span class="sxs-lookup"><span data-stu-id="a489c-170">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="a489c-171">Пример: **определение** для того, чтобы включить EmployeeID и TenantCountry в качестве утверждений в маркерах</span><span class="sxs-lookup"><span data-stu-id="a489c-171">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="a489c-172">Пример: **определение,** использующее преобразование утверждений</span><span class="sxs-lookup"><span data-stu-id="a489c-172">Example: **definition** that uses a claims transformation</span></span>
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

| <span data-ttu-id="a489c-173">Свойство</span><span class="sxs-lookup"><span data-stu-id="a489c-173">Property</span></span>     | <span data-ttu-id="a489c-174">Тип</span><span class="sxs-lookup"><span data-stu-id="a489c-174">Type</span></span>   |<span data-ttu-id="a489c-175">Описание</span><span class="sxs-lookup"><span data-stu-id="a489c-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a489c-176">Версия</span><span class="sxs-lookup"><span data-stu-id="a489c-176">Version</span></span>|<span data-ttu-id="a489c-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="a489c-177">Integer</span></span>|<span data-ttu-id="a489c-178">Значение 1.</span><span class="sxs-lookup"><span data-stu-id="a489c-178">Set value of 1.</span></span> <span data-ttu-id="a489c-179">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a489c-179">Required.</span></span>|
|<span data-ttu-id="a489c-180">IncludeBasicClaimSet</span><span class="sxs-lookup"><span data-stu-id="a489c-180">IncludeBasicClaimSet</span></span>|<span data-ttu-id="a489c-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="a489c-181">Boolean</span></span>|<span data-ttu-id="a489c-182">Если установлено, что все утверждения в базовом наборе утверждений излучаются в маркерах, затронутых политикой.</span><span class="sxs-lookup"><span data-stu-id="a489c-182">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="a489c-183">Если установлено ложное, утверждения в базовом наборе утверждений не находятся в маркерах, если они не добавляются отдельно в свойстве ClaimsSchema той же политики.</span><span class="sxs-lookup"><span data-stu-id="a489c-183">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="a489c-184">ClaimsSchema</span><span class="sxs-lookup"><span data-stu-id="a489c-184">ClaimsSchema</span></span>|<span data-ttu-id="a489c-185">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="a489c-185">JSON object</span></span>|<span data-ttu-id="a489c-186">Определяет, какие утверждения присутствуют в маркерах, затронутых политикой, в дополнение к основному набору утверждений и набору основных утверждений.</span><span class="sxs-lookup"><span data-stu-id="a489c-186">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="a489c-187">Для каждой записи схемы утверждения, определенной в этом свойстве, требуется определенная информация.</span><span class="sxs-lookup"><span data-stu-id="a489c-187">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="a489c-188">Укажите, откуда приходят данные (пара Value или Source/ID) и какие утверждают, что данные излучаются как (Тип утверждения).</span><span class="sxs-lookup"><span data-stu-id="a489c-188">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="a489c-189">Дополнительные сведения доступны в [определении ClaimsSchema.](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema)</span><span class="sxs-lookup"><span data-stu-id="a489c-189">Further details are available in the [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="a489c-190">ClaimsTransformation</span><span class="sxs-lookup"><span data-stu-id="a489c-190">ClaimsTransformation</span></span>|<span data-ttu-id="a489c-191">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="a489c-191">JSON object</span></span>| <span data-ttu-id="a489c-192">Определяет общие преобразования, которые можно применить к исходным данным, для создания данных вывода для утверждений, указанных в ClaimsSchema.</span><span class="sxs-lookup"><span data-stu-id="a489c-192">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="a489c-193">Дополнительные сведения доступны в определении [ClaimsTransformation](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="a489c-193">Further details are available in the [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="a489c-194">Связи</span><span class="sxs-lookup"><span data-stu-id="a489c-194">Relationships</span></span>

| <span data-ttu-id="a489c-195">Связь</span><span class="sxs-lookup"><span data-stu-id="a489c-195">Relationship</span></span> | <span data-ttu-id="a489c-196">Тип</span><span class="sxs-lookup"><span data-stu-id="a489c-196">Type</span></span>        | <span data-ttu-id="a489c-197">Описание</span><span class="sxs-lookup"><span data-stu-id="a489c-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a489c-198">appliesTo</span><span class="sxs-lookup"><span data-stu-id="a489c-198">appliesTo</span></span>|<span data-ttu-id="a489c-199">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a489c-199">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="a489c-200">Коллекция [directoryObject,](directoryObject.md) к которую была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="a489c-200">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="a489c-201">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a489c-201">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a489c-202">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a489c-202">JSON representation</span></span>

<span data-ttu-id="a489c-203">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a489c-203">The following is a JSON representation of the resource.</span></span>

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
