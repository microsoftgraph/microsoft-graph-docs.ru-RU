---
title: Тип ресурса Клаимсмаппингполици
description: Представляет политику, которая может управлять временем существования маркера доступа, выданного Azure Active Directory (Azure AD).
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 09d68f6c9561ba0bf433c56abbba640b485a6fba
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405610"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="ff05e-103">Тип ресурса Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="ff05e-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="ff05e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff05e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff05e-105">Представляет политики сопоставления утверждений для протоколов WS — подача, SAML, OAuth 2,0 и OpenID Connect для маркеров, выданных определенным приложением.</span><span class="sxs-lookup"><span data-stu-id="ff05e-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="ff05e-106">Политики сопоставления утверждений можно использовать для:</span><span class="sxs-lookup"><span data-stu-id="ff05e-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="ff05e-107">Выберите утверждения, включаемые в маркеры</span><span class="sxs-lookup"><span data-stu-id="ff05e-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="ff05e-108">Создание типов утверждений, которые еще не существуют</span><span class="sxs-lookup"><span data-stu-id="ff05e-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="ff05e-109">Выбор или изменение источника данных, выпущенных в определенных утверждениях</span><span class="sxs-lookup"><span data-stu-id="ff05e-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="ff05e-110">Дополнительные сведения о сценариях и конфигурации [: Настройка утверждений, выпущенных в маркерах для определенного приложения в клиенте](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span><span class="sxs-lookup"><span data-stu-id="ff05e-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="ff05e-111">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ff05e-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ff05e-112">Методы</span><span class="sxs-lookup"><span data-stu-id="ff05e-112">Methods</span></span>

| <span data-ttu-id="ff05e-113">Метод</span><span class="sxs-lookup"><span data-stu-id="ff05e-113">Method</span></span>       | <span data-ttu-id="ff05e-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff05e-114">Return Type</span></span> | <span data-ttu-id="ff05e-115">Описание</span><span class="sxs-lookup"><span data-stu-id="ff05e-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ff05e-116">Создание claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="ff05e-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="ff05e-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="ff05e-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="ff05e-118">Создание объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="ff05e-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="ff05e-119">Получение Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="ff05e-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="ff05e-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="ff05e-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="ff05e-121">Чтение свойств и связей объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="ff05e-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="ff05e-122">Перечисление типов ресурсов claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="ff05e-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="ff05e-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="ff05e-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="ff05e-124">Чтение свойств и связей объектов КлаимсмаппингполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="ff05e-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="ff05e-125">Обновление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="ff05e-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="ff05e-126">Нет</span><span class="sxs-lookup"><span data-stu-id="ff05e-126">None</span></span> | <span data-ttu-id="ff05e-127">Обновление объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="ff05e-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="ff05e-128">Удаление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="ff05e-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="ff05e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="ff05e-129">None</span></span> | <span data-ttu-id="ff05e-130">Удаление объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="ff05e-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="ff05e-131">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="ff05e-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="ff05e-132">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ff05e-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="ff05e-133">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="ff05e-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="ff05e-134">Назначение типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="ff05e-134">Assign claimsMappingPolicy</span></span>](../api/serviceprincipal-post-claimsmappingpolicies.md) | <span data-ttu-id="ff05e-135">Нет</span><span class="sxs-lookup"><span data-stu-id="ff05e-135">None</span></span> | <span data-ttu-id="ff05e-136">Назначьте Клаимсмаппингполици объекту [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ff05e-136">Assign a claimsMappingPolicy to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="ff05e-137">Список назначенных Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="ff05e-137">List assigned claimsMappingPolicy</span></span>](../api/serviceprincipal-list-claimsmappingpolicies.md) | <span data-ttu-id="ff05e-138">Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ff05e-138">[claimsMappingPolicy](claimsmappingpolicy.md) collection</span></span> | <span data-ttu-id="ff05e-139">Перечисление объектов Клаимсмаппингполици, назначенных объекту [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ff05e-139">List the claimsMappingPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="ff05e-140">Удаление типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="ff05e-140">Remove claimsMappingPolicy</span></span>](../api/serviceprincipal-delete-claimsmappingpolicies.md) | <span data-ttu-id="ff05e-141">Нет</span><span class="sxs-lookup"><span data-stu-id="ff05e-141">None</span></span> | <span data-ttu-id="ff05e-142">Удаление объекта Клаимсмаппингполици из объекта [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ff05e-142">Remove a claimsMappingPolicy from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff05e-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff05e-143">Properties</span></span>

| <span data-ttu-id="ff05e-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff05e-144">Property</span></span>     | <span data-ttu-id="ff05e-145">Тип</span><span class="sxs-lookup"><span data-stu-id="ff05e-145">Type</span></span>        | <span data-ttu-id="ff05e-146">Описание</span><span class="sxs-lookup"><span data-stu-id="ff05e-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff05e-147">id</span><span class="sxs-lookup"><span data-stu-id="ff05e-147">id</span></span>|<span data-ttu-id="ff05e-148">String</span><span class="sxs-lookup"><span data-stu-id="ff05e-148">String</span></span>| <span data-ttu-id="ff05e-149">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ff05e-149">Unique identifier for this policy.</span></span> <span data-ttu-id="ff05e-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff05e-150">Read-only.</span></span>|
|<span data-ttu-id="ff05e-151">RDLC</span><span class="sxs-lookup"><span data-stu-id="ff05e-151">definition</span></span>|<span data-ttu-id="ff05e-152">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ff05e-152">String collection</span></span>| <span data-ttu-id="ff05e-153">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ff05e-153">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="ff05e-154">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="ff05e-154">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="ff05e-155">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff05e-155">Required.</span></span>|
|<span data-ttu-id="ff05e-156">description</span><span class="sxs-lookup"><span data-stu-id="ff05e-156">description</span></span>|<span data-ttu-id="ff05e-157">String</span><span class="sxs-lookup"><span data-stu-id="ff05e-157">String</span></span>| <span data-ttu-id="ff05e-158">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ff05e-158">Description for this policy.</span></span>|
|<span data-ttu-id="ff05e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ff05e-159">displayName</span></span>|<span data-ttu-id="ff05e-160">String</span><span class="sxs-lookup"><span data-stu-id="ff05e-160">String</span></span>| <span data-ttu-id="ff05e-161">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ff05e-161">Display name for this policy.</span></span> <span data-ttu-id="ff05e-162">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ff05e-162">Required.</span></span>|
|<span data-ttu-id="ff05e-163">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="ff05e-163">isOrganizationDefault</span></span>|<span data-ttu-id="ff05e-164">Логический</span><span class="sxs-lookup"><span data-stu-id="ff05e-164">Boolean</span></span>|<span data-ttu-id="ff05e-165">Игнорировать это свойство.</span><span class="sxs-lookup"><span data-stu-id="ff05e-165">Ignore this property.</span></span> <span data-ttu-id="ff05e-166">Политика сопоставления утверждений может применяться только к субъектам служб и не может быть настроена глобально для Организации.</span><span class="sxs-lookup"><span data-stu-id="ff05e-166">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="ff05e-167">Свойства определения политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="ff05e-167">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="ff05e-168">Свойства, приведенные ниже, формируют объект JSON, представляющий политику сопоставления утверждений.</span><span class="sxs-lookup"><span data-stu-id="ff05e-168">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="ff05e-169">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="ff05e-169">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="ff05e-170">Ниже приведено несколько примеров определений.</span><span class="sxs-lookup"><span data-stu-id="ff05e-170">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="ff05e-171">Пример: **Определение** для включения в маркеры кода EmployeeID и тенанткаунтри в качестве утверждений</span><span class="sxs-lookup"><span data-stu-id="ff05e-171">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="ff05e-172">Пример: **Определение** , использующее преобразование утверждений</span><span class="sxs-lookup"><span data-stu-id="ff05e-172">Example: **definition** that uses a claims transformation</span></span>
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

| <span data-ttu-id="ff05e-173">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff05e-173">Property</span></span>     | <span data-ttu-id="ff05e-174">Тип</span><span class="sxs-lookup"><span data-stu-id="ff05e-174">Type</span></span>   |<span data-ttu-id="ff05e-175">Описание</span><span class="sxs-lookup"><span data-stu-id="ff05e-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff05e-176">Версия</span><span class="sxs-lookup"><span data-stu-id="ff05e-176">Version</span></span>|<span data-ttu-id="ff05e-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="ff05e-177">Integer</span></span>|<span data-ttu-id="ff05e-178">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="ff05e-178">Set value of 1.</span></span> <span data-ttu-id="ff05e-179">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ff05e-179">Required.</span></span>|
|<span data-ttu-id="ff05e-180">инклудебасикклаимсет</span><span class="sxs-lookup"><span data-stu-id="ff05e-180">IncludeBasicClaimSet</span></span>|<span data-ttu-id="ff05e-181">Логический</span><span class="sxs-lookup"><span data-stu-id="ff05e-181">Boolean</span></span>|<span data-ttu-id="ff05e-182">Если задано значение true, все утверждения в базовом наборе утверждений порождаются в маркерах, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="ff05e-182">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="ff05e-183">Если задано значение false, утверждения в базовом наборе утверждений не входят в маркеры, если они не добавлены по отдельности в свойство Клаимссчема той же политики.</span><span class="sxs-lookup"><span data-stu-id="ff05e-183">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="ff05e-184">клаимссчема</span><span class="sxs-lookup"><span data-stu-id="ff05e-184">ClaimsSchema</span></span>|<span data-ttu-id="ff05e-185">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="ff05e-185">JSON object</span></span>|<span data-ttu-id="ff05e-186">Определяет, какие утверждения присутствуют в маркерах, на которые влияет политика, а также базовый набор утверждений и основной набор утверждений.</span><span class="sxs-lookup"><span data-stu-id="ff05e-186">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="ff05e-187">Для каждой записи схемы утверждений, определенной в этом свойстве, требуются определенные сведения.</span><span class="sxs-lookup"><span data-stu-id="ff05e-187">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="ff05e-188">Укажите, откуда берутся данные (в виде значения или источника/идентификатора), и какие утверждения данные выдаются как (тип утверждения).</span><span class="sxs-lookup"><span data-stu-id="ff05e-188">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="ff05e-189">Дополнительные сведения можно найти в [определении клаимссчема](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span><span class="sxs-lookup"><span data-stu-id="ff05e-189">Further details are available in the [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="ff05e-190">клаимстрансформатион</span><span class="sxs-lookup"><span data-stu-id="ff05e-190">ClaimsTransformation</span></span>|<span data-ttu-id="ff05e-191">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="ff05e-191">JSON object</span></span>| <span data-ttu-id="ff05e-192">Определяет общие преобразования, которые можно применять к исходным данным для создания выходных данных для утверждений, указанных в Клаимссчема.</span><span class="sxs-lookup"><span data-stu-id="ff05e-192">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="ff05e-193">Дополнительные сведения можно найти в [определении клаимстрансформатион](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="ff05e-193">Further details are available in the [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="ff05e-194">Связи</span><span class="sxs-lookup"><span data-stu-id="ff05e-194">Relationships</span></span>

| <span data-ttu-id="ff05e-195">Связь</span><span class="sxs-lookup"><span data-stu-id="ff05e-195">Relationship</span></span> | <span data-ttu-id="ff05e-196">Тип</span><span class="sxs-lookup"><span data-stu-id="ff05e-196">Type</span></span>        | <span data-ttu-id="ff05e-197">Описание</span><span class="sxs-lookup"><span data-stu-id="ff05e-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff05e-198">Тег</span><span class="sxs-lookup"><span data-stu-id="ff05e-198">appliesTo</span></span>|<span data-ttu-id="ff05e-199">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ff05e-199">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="ff05e-200">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="ff05e-200">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="ff05e-201">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff05e-201">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff05e-202">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff05e-202">JSON representation</span></span>

<span data-ttu-id="ff05e-203">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff05e-203">The following is a JSON representation of the resource.</span></span>

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