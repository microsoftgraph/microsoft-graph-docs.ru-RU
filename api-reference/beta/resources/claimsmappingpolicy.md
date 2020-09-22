---
title: Тип ресурса Клаимсмаппингполици
description: Представляет политику, которая может управлять временем существования маркера доступа, выданного Azure Active Directory (Azure AD).
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 83a3a0bb455e72796aac2fc27066f161b9a909ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040149"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="b6a49-103">Тип ресурса Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="b6a49-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="b6a49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6a49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6a49-105">Представляет политики сопоставления утверждений для протоколов WS — подача, SAML, OAuth 2,0 и OpenID Connect для маркеров, выданных определенным приложением.</span><span class="sxs-lookup"><span data-stu-id="b6a49-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="b6a49-106">Политики сопоставления утверждений можно использовать для:</span><span class="sxs-lookup"><span data-stu-id="b6a49-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="b6a49-107">Выберите утверждения, включаемые в маркеры</span><span class="sxs-lookup"><span data-stu-id="b6a49-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="b6a49-108">Создание типов утверждений, которые еще не существуют</span><span class="sxs-lookup"><span data-stu-id="b6a49-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="b6a49-109">Выбор или изменение источника данных, выпущенных в определенных утверждениях</span><span class="sxs-lookup"><span data-stu-id="b6a49-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="b6a49-110">Дополнительные сведения о сценариях и конфигурации [: Настройка утверждений, выпущенных в маркерах для определенного приложения в клиенте](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span><span class="sxs-lookup"><span data-stu-id="b6a49-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="b6a49-111">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6a49-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b6a49-112">Методы</span><span class="sxs-lookup"><span data-stu-id="b6a49-112">Methods</span></span>

| <span data-ttu-id="b6a49-113">Метод</span><span class="sxs-lookup"><span data-stu-id="b6a49-113">Method</span></span>       | <span data-ttu-id="b6a49-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b6a49-114">Return Type</span></span> | <span data-ttu-id="b6a49-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a49-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b6a49-116">Создание claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="b6a49-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="b6a49-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="b6a49-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="b6a49-118">Создание объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="b6a49-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="b6a49-119">Получение Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="b6a49-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="b6a49-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="b6a49-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="b6a49-121">Чтение свойств и связей объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="b6a49-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="b6a49-122">Перечисление типов ресурсов claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="b6a49-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="b6a49-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="b6a49-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="b6a49-124">Чтение свойств и связей объектов КлаимсмаппингполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="b6a49-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="b6a49-125">Обновление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="b6a49-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="b6a49-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b6a49-126">None</span></span> | <span data-ttu-id="b6a49-127">Обновление объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="b6a49-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="b6a49-128">Удаление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="b6a49-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="b6a49-129">Нет</span><span class="sxs-lookup"><span data-stu-id="b6a49-129">None</span></span> | <span data-ttu-id="b6a49-130">Удаление объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="b6a49-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="b6a49-131">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="b6a49-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="b6a49-132">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="b6a49-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b6a49-133">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="b6a49-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="b6a49-134">Назначение типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="b6a49-134">Assign claimsMappingPolicy</span></span>](../api/serviceprincipal-post-claimsmappingpolicies.md) | <span data-ttu-id="b6a49-135">Нет</span><span class="sxs-lookup"><span data-stu-id="b6a49-135">None</span></span> | <span data-ttu-id="b6a49-136">Назначьте Клаимсмаппингполици объекту [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="b6a49-136">Assign a claimsMappingPolicy to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="b6a49-137">Список назначенных Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="b6a49-137">List assigned claimsMappingPolicy</span></span>](../api/serviceprincipal-list-claimsmappingpolicies.md) | <span data-ttu-id="b6a49-138">Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6a49-138">[claimsMappingPolicy](claimsmappingpolicy.md) collection</span></span> | <span data-ttu-id="b6a49-139">Перечисление объектов Клаимсмаппингполици, назначенных объекту [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="b6a49-139">List the claimsMappingPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="b6a49-140">Удаление типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="b6a49-140">Remove claimsMappingPolicy</span></span>](../api/serviceprincipal-delete-claimsmappingpolicies.md) | <span data-ttu-id="b6a49-141">Нет</span><span class="sxs-lookup"><span data-stu-id="b6a49-141">None</span></span> | <span data-ttu-id="b6a49-142">Удаление объекта Клаимсмаппингполици из объекта [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="b6a49-142">Remove a claimsMappingPolicy from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6a49-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6a49-143">Properties</span></span>

| <span data-ttu-id="b6a49-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6a49-144">Property</span></span>     | <span data-ttu-id="b6a49-145">Тип</span><span class="sxs-lookup"><span data-stu-id="b6a49-145">Type</span></span>        | <span data-ttu-id="b6a49-146">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a49-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6a49-147">id</span><span class="sxs-lookup"><span data-stu-id="b6a49-147">id</span></span>|<span data-ttu-id="b6a49-148">String</span><span class="sxs-lookup"><span data-stu-id="b6a49-148">String</span></span>| <span data-ttu-id="b6a49-149">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b6a49-149">Unique identifier for this policy.</span></span> <span data-ttu-id="b6a49-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6a49-150">Read-only.</span></span>|
|<span data-ttu-id="b6a49-151">RDLC</span><span class="sxs-lookup"><span data-stu-id="b6a49-151">definition</span></span>|<span data-ttu-id="b6a49-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b6a49-152">String collection</span></span>| <span data-ttu-id="b6a49-153">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b6a49-153">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="b6a49-154">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="b6a49-154">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="b6a49-155">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a49-155">Required.</span></span>|
|<span data-ttu-id="b6a49-156">description</span><span class="sxs-lookup"><span data-stu-id="b6a49-156">description</span></span>|<span data-ttu-id="b6a49-157">String</span><span class="sxs-lookup"><span data-stu-id="b6a49-157">String</span></span>| <span data-ttu-id="b6a49-158">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b6a49-158">Description for this policy.</span></span>|
|<span data-ttu-id="b6a49-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b6a49-159">displayName</span></span>|<span data-ttu-id="b6a49-160">String</span><span class="sxs-lookup"><span data-stu-id="b6a49-160">String</span></span>| <span data-ttu-id="b6a49-161">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b6a49-161">Display name for this policy.</span></span> <span data-ttu-id="b6a49-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a49-162">Required.</span></span>|
|<span data-ttu-id="b6a49-163">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="b6a49-163">isOrganizationDefault</span></span>|<span data-ttu-id="b6a49-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6a49-164">Boolean</span></span>|<span data-ttu-id="b6a49-165">Игнорировать это свойство.</span><span class="sxs-lookup"><span data-stu-id="b6a49-165">Ignore this property.</span></span> <span data-ttu-id="b6a49-166">Политика сопоставления утверждений может применяться только к субъектам служб и не может быть настроена глобально для Организации.</span><span class="sxs-lookup"><span data-stu-id="b6a49-166">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="b6a49-167">Свойства определения политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="b6a49-167">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="b6a49-168">Свойства, приведенные ниже, формируют объект JSON, представляющий политику сопоставления утверждений.</span><span class="sxs-lookup"><span data-stu-id="b6a49-168">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="b6a49-169">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="b6a49-169">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="b6a49-170">Ниже приведено несколько примеров определений.</span><span class="sxs-lookup"><span data-stu-id="b6a49-170">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="b6a49-171">Пример: **Определение** для включения в маркеры кода EmployeeID и тенанткаунтри в качестве утверждений</span><span class="sxs-lookup"><span data-stu-id="b6a49-171">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="b6a49-172">Пример: **Определение** , использующее преобразование утверждений</span><span class="sxs-lookup"><span data-stu-id="b6a49-172">Example: **definition** that uses a claims transformation</span></span>
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

| <span data-ttu-id="b6a49-173">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6a49-173">Property</span></span>     | <span data-ttu-id="b6a49-174">Тип</span><span class="sxs-lookup"><span data-stu-id="b6a49-174">Type</span></span>   |<span data-ttu-id="b6a49-175">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a49-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6a49-176">Версия</span><span class="sxs-lookup"><span data-stu-id="b6a49-176">Version</span></span>|<span data-ttu-id="b6a49-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="b6a49-177">Integer</span></span>|<span data-ttu-id="b6a49-178">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="b6a49-178">Set value of 1.</span></span> <span data-ttu-id="b6a49-179">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a49-179">Required.</span></span>|
|<span data-ttu-id="b6a49-180">инклудебасикклаимсет</span><span class="sxs-lookup"><span data-stu-id="b6a49-180">IncludeBasicClaimSet</span></span>|<span data-ttu-id="b6a49-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6a49-181">Boolean</span></span>|<span data-ttu-id="b6a49-182">Если задано значение true, все утверждения в базовом наборе утверждений порождаются в маркерах, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="b6a49-182">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="b6a49-183">Если задано значение false, утверждения в базовом наборе утверждений не входят в маркеры, если они не добавлены по отдельности в свойство Клаимссчема той же политики.</span><span class="sxs-lookup"><span data-stu-id="b6a49-183">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="b6a49-184">клаимссчема</span><span class="sxs-lookup"><span data-stu-id="b6a49-184">ClaimsSchema</span></span>|<span data-ttu-id="b6a49-185">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="b6a49-185">JSON object</span></span>|<span data-ttu-id="b6a49-186">Определяет, какие утверждения присутствуют в маркерах, на которые влияет политика, а также базовый набор утверждений и основной набор утверждений.</span><span class="sxs-lookup"><span data-stu-id="b6a49-186">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="b6a49-187">Для каждой записи схемы утверждений, определенной в этом свойстве, требуются определенные сведения.</span><span class="sxs-lookup"><span data-stu-id="b6a49-187">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="b6a49-188">Укажите, откуда берутся данные (в виде значения или источника/идентификатора), и какие утверждения данные выдаются как (тип утверждения).</span><span class="sxs-lookup"><span data-stu-id="b6a49-188">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="b6a49-189">Дополнительные сведения можно найти в [определении клаимссчема](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span><span class="sxs-lookup"><span data-stu-id="b6a49-189">Further details are available in the [ClaimsSchema definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="b6a49-190">клаимстрансформатион</span><span class="sxs-lookup"><span data-stu-id="b6a49-190">ClaimsTransformation</span></span>|<span data-ttu-id="b6a49-191">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="b6a49-191">JSON object</span></span>| <span data-ttu-id="b6a49-192">Определяет общие преобразования, которые можно применять к исходным данным для создания выходных данных для утверждений, указанных в Клаимссчема.</span><span class="sxs-lookup"><span data-stu-id="b6a49-192">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="b6a49-193">Дополнительные сведения можно найти в [определении клаимстрансформатион](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="b6a49-193">Further details are available in the [ClaimsTransformation definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="b6a49-194">Отношения</span><span class="sxs-lookup"><span data-stu-id="b6a49-194">Relationships</span></span>

| <span data-ttu-id="b6a49-195">Связь</span><span class="sxs-lookup"><span data-stu-id="b6a49-195">Relationship</span></span> | <span data-ttu-id="b6a49-196">Тип</span><span class="sxs-lookup"><span data-stu-id="b6a49-196">Type</span></span>        | <span data-ttu-id="b6a49-197">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a49-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6a49-198">Тег</span><span class="sxs-lookup"><span data-stu-id="b6a49-198">appliesTo</span></span>|<span data-ttu-id="b6a49-199">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="b6a49-199">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b6a49-200">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="b6a49-200">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="b6a49-201">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6a49-201">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6a49-202">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6a49-202">JSON representation</span></span>

<span data-ttu-id="b6a49-203">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6a49-203">The following is a JSON representation of the resource.</span></span>

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

