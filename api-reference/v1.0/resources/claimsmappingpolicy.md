---
title: Тип ресурса Клаимсмаппингполици
description: Представляет политики сопоставления утверждений для протоколов WS — подача, SAML, OAuth 2,0 и OpenID Connect для маркеров, выданных определенным приложением.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 360c2767d424f37ef120f7c2eab836569396e129
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086818"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="13ec3-103">Тип ресурса Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="13ec3-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="13ec3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13ec3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13ec3-105">Представляет политики сопоставления утверждений для протоколов WS — подача, SAML, OAuth 2,0 и OpenID Connect для маркеров, выданных определенным приложением.</span><span class="sxs-lookup"><span data-stu-id="13ec3-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="13ec3-106">Политики сопоставления утверждений можно использовать для:</span><span class="sxs-lookup"><span data-stu-id="13ec3-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="13ec3-107">Выберите утверждения, включаемые в маркеры</span><span class="sxs-lookup"><span data-stu-id="13ec3-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="13ec3-108">Создание типов утверждений, которые еще не существуют</span><span class="sxs-lookup"><span data-stu-id="13ec3-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="13ec3-109">Выбор или изменение источника данных, выпущенных в определенных утверждениях</span><span class="sxs-lookup"><span data-stu-id="13ec3-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="13ec3-110">Дополнительные сведения о сценариях и конфигурации [: Настройка утверждений, выпущенных в маркерах для определенного приложения в клиенте](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span><span class="sxs-lookup"><span data-stu-id="13ec3-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="13ec3-111">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="13ec3-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="13ec3-112">Методы</span><span class="sxs-lookup"><span data-stu-id="13ec3-112">Methods</span></span>

| <span data-ttu-id="13ec3-113">Метод</span><span class="sxs-lookup"><span data-stu-id="13ec3-113">Method</span></span>       | <span data-ttu-id="13ec3-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="13ec3-114">Return Type</span></span> | <span data-ttu-id="13ec3-115">Описание</span><span class="sxs-lookup"><span data-stu-id="13ec3-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="13ec3-116">Создание claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="13ec3-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="13ec3-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="13ec3-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="13ec3-118">Создание объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="13ec3-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="13ec3-119">Получение Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="13ec3-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="13ec3-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="13ec3-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="13ec3-121">Чтение свойств и связей объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="13ec3-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="13ec3-122">Перечисление типов ресурсов claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="13ec3-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="13ec3-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="13ec3-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="13ec3-124">Чтение свойств и связей объектов КлаимсмаппингполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="13ec3-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="13ec3-125">Обновление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="13ec3-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="13ec3-126">Нет</span><span class="sxs-lookup"><span data-stu-id="13ec3-126">None</span></span> | <span data-ttu-id="13ec3-127">Обновление объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="13ec3-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="13ec3-128">Удаление Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="13ec3-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="13ec3-129">Нет</span><span class="sxs-lookup"><span data-stu-id="13ec3-129">None</span></span> | <span data-ttu-id="13ec3-130">Удаление объекта Клаимсмаппингполици.</span><span class="sxs-lookup"><span data-stu-id="13ec3-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="13ec3-131">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="13ec3-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="13ec3-132">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="13ec3-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="13ec3-133">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="13ec3-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="13ec3-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="13ec3-134">Properties</span></span>

| <span data-ttu-id="13ec3-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="13ec3-135">Property</span></span>     | <span data-ttu-id="13ec3-136">Тип</span><span class="sxs-lookup"><span data-stu-id="13ec3-136">Type</span></span>        | <span data-ttu-id="13ec3-137">Описание</span><span class="sxs-lookup"><span data-stu-id="13ec3-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13ec3-138">id</span><span class="sxs-lookup"><span data-stu-id="13ec3-138">id</span></span>|<span data-ttu-id="13ec3-139">Строка</span><span class="sxs-lookup"><span data-stu-id="13ec3-139">String</span></span>| <span data-ttu-id="13ec3-140">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="13ec3-140">Unique identifier for this policy.</span></span> <span data-ttu-id="13ec3-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13ec3-141">Read-only.</span></span>|
|<span data-ttu-id="13ec3-142">RDLC</span><span class="sxs-lookup"><span data-stu-id="13ec3-142">definition</span></span>|<span data-ttu-id="13ec3-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="13ec3-143">String collection</span></span>| <span data-ttu-id="13ec3-144">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="13ec3-144">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="13ec3-145">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="13ec3-145">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="13ec3-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13ec3-146">Required.</span></span>|
|<span data-ttu-id="13ec3-147">description</span><span class="sxs-lookup"><span data-stu-id="13ec3-147">description</span></span>|<span data-ttu-id="13ec3-148">Строка</span><span class="sxs-lookup"><span data-stu-id="13ec3-148">String</span></span>| <span data-ttu-id="13ec3-149">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="13ec3-149">Description for this policy.</span></span>|
|<span data-ttu-id="13ec3-150">displayName</span><span class="sxs-lookup"><span data-stu-id="13ec3-150">displayName</span></span>|<span data-ttu-id="13ec3-151">Строка</span><span class="sxs-lookup"><span data-stu-id="13ec3-151">String</span></span>| <span data-ttu-id="13ec3-152">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="13ec3-152">Display name for this policy.</span></span> <span data-ttu-id="13ec3-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13ec3-153">Required.</span></span>|
|<span data-ttu-id="13ec3-154">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="13ec3-154">isOrganizationDefault</span></span>|<span data-ttu-id="13ec3-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="13ec3-155">Boolean</span></span>|<span data-ttu-id="13ec3-156">Игнорировать это свойство.</span><span class="sxs-lookup"><span data-stu-id="13ec3-156">Ignore this property.</span></span> <span data-ttu-id="13ec3-157">Политика сопоставления утверждений может применяться только к субъектам служб и не может быть настроена глобально для Организации.</span><span class="sxs-lookup"><span data-stu-id="13ec3-157">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="13ec3-158">Свойства определения политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="13ec3-158">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="13ec3-159">Свойства, приведенные ниже, формируют объект JSON, представляющий политику сопоставления утверждений.</span><span class="sxs-lookup"><span data-stu-id="13ec3-159">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="13ec3-160">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="13ec3-160">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="13ec3-161">Ниже приведено несколько примеров определений.</span><span class="sxs-lookup"><span data-stu-id="13ec3-161">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="13ec3-162">Пример: **Определение** для включения в маркеры кода EmployeeID и тенанткаунтри в качестве утверждений</span><span class="sxs-lookup"><span data-stu-id="13ec3-162">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="13ec3-163">Пример: **Определение** , использующее преобразование утверждений</span><span class="sxs-lookup"><span data-stu-id="13ec3-163">Example: **definition** that uses a claims transformation</span></span>
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

| <span data-ttu-id="13ec3-164">Свойство</span><span class="sxs-lookup"><span data-stu-id="13ec3-164">Property</span></span>     | <span data-ttu-id="13ec3-165">Тип</span><span class="sxs-lookup"><span data-stu-id="13ec3-165">Type</span></span>   |<span data-ttu-id="13ec3-166">Описание</span><span class="sxs-lookup"><span data-stu-id="13ec3-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13ec3-167">Версия</span><span class="sxs-lookup"><span data-stu-id="13ec3-167">Version</span></span>|<span data-ttu-id="13ec3-168">Целое число</span><span class="sxs-lookup"><span data-stu-id="13ec3-168">Integer</span></span>|<span data-ttu-id="13ec3-169">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="13ec3-169">Set value of 1.</span></span> <span data-ttu-id="13ec3-170">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13ec3-170">Required.</span></span>|
|<span data-ttu-id="13ec3-171">инклудебасикклаимсет</span><span class="sxs-lookup"><span data-stu-id="13ec3-171">IncludeBasicClaimSet</span></span>|<span data-ttu-id="13ec3-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="13ec3-172">Boolean</span></span>|<span data-ttu-id="13ec3-173">Если задано значение true, все утверждения в базовом наборе утверждений порождаются в маркерах, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="13ec3-173">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="13ec3-174">Если задано значение false, утверждения в базовом наборе утверждений не входят в маркеры, если они не добавлены по отдельности в свойство Клаимссчема той же политики.</span><span class="sxs-lookup"><span data-stu-id="13ec3-174">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="13ec3-175">клаимссчема</span><span class="sxs-lookup"><span data-stu-id="13ec3-175">ClaimsSchema</span></span>|<span data-ttu-id="13ec3-176">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="13ec3-176">JSON object</span></span>|<span data-ttu-id="13ec3-177">Определяет, какие утверждения присутствуют в маркерах, на которые влияет политика, а также базовый набор утверждений и основной набор утверждений.</span><span class="sxs-lookup"><span data-stu-id="13ec3-177">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="13ec3-178">Для каждой записи схемы утверждений, определенной в этом свойстве, требуются определенные сведения.</span><span class="sxs-lookup"><span data-stu-id="13ec3-178">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="13ec3-179">Укажите, откуда берутся данные (в виде значения или источника/идентификатора), и какие утверждения данные выдаются как (тип утверждения).</span><span class="sxs-lookup"><span data-stu-id="13ec3-179">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="13ec3-180">Дополнительные сведения см. в статье [Определение клаимссчема](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span><span class="sxs-lookup"><span data-stu-id="13ec3-180">For more information, see [ClaimsSchema definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="13ec3-181">клаимстрансформатион</span><span class="sxs-lookup"><span data-stu-id="13ec3-181">ClaimsTransformation</span></span>|<span data-ttu-id="13ec3-182">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="13ec3-182">JSON object</span></span>| <span data-ttu-id="13ec3-183">Определяет общие преобразования, которые можно применять к исходным данным для создания выходных данных для утверждений, указанных в Клаимссчема.</span><span class="sxs-lookup"><span data-stu-id="13ec3-183">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="13ec3-184">Дополнительные сведения см. в статье [Определение клаимстрансформатион](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="13ec3-184">For more information, see [ClaimsTransformation definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="13ec3-185">Связи</span><span class="sxs-lookup"><span data-stu-id="13ec3-185">Relationships</span></span>

| <span data-ttu-id="13ec3-186">Связь</span><span class="sxs-lookup"><span data-stu-id="13ec3-186">Relationship</span></span> | <span data-ttu-id="13ec3-187">Тип</span><span class="sxs-lookup"><span data-stu-id="13ec3-187">Type</span></span>        | <span data-ttu-id="13ec3-188">Описание</span><span class="sxs-lookup"><span data-stu-id="13ec3-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13ec3-189">Тег</span><span class="sxs-lookup"><span data-stu-id="13ec3-189">appliesTo</span></span>|<span data-ttu-id="13ec3-190">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="13ec3-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="13ec3-191">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="13ec3-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="13ec3-192">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13ec3-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13ec3-193">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13ec3-193">JSON representation</span></span>

<span data-ttu-id="13ec3-194">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13ec3-194">The following is a JSON representation of the resource.</span></span>

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
