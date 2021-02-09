---
title: Тип ресурса tokenIssuancePolicy
description: Представляет политику для указания характеристик маркеров SAML, выдавляемой Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aae5bd4c252549f92d784b45eaf2d5af15a32db6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159880"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="32977-103">Тип ресурса tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="32977-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="32977-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32977-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32977-105">Представляет политику для указания характеристик маркеров SAML, выдавляемой Azure AD.</span><span class="sxs-lookup"><span data-stu-id="32977-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="32977-106">Политики выдачи маркеров можно использовать для:</span><span class="sxs-lookup"><span data-stu-id="32977-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="32977-107">Настройка параметров подписи</span><span class="sxs-lookup"><span data-stu-id="32977-107">Set signing options</span></span>
- <span data-ttu-id="32977-108">Настройка алгоритма подписи</span><span class="sxs-lookup"><span data-stu-id="32977-108">Set signing algorithm</span></span>
- <span data-ttu-id="32977-109">Настройка версии маркера SAML</span><span class="sxs-lookup"><span data-stu-id="32977-109">Set SAML token version</span></span>

<span data-ttu-id="32977-110">Наследуется от [stsPolicy.](stsPolicy.md)</span><span class="sxs-lookup"><span data-stu-id="32977-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="32977-111">Методы</span><span class="sxs-lookup"><span data-stu-id="32977-111">Methods</span></span>

| <span data-ttu-id="32977-112">Метод</span><span class="sxs-lookup"><span data-stu-id="32977-112">Method</span></span>       | <span data-ttu-id="32977-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="32977-113">Return Type</span></span> | <span data-ttu-id="32977-114">Описание</span><span class="sxs-lookup"><span data-stu-id="32977-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="32977-115">Создание tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="32977-115">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="32977-116">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="32977-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="32977-117">Создание объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="32977-117">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="32977-118">Get tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="32977-118">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="32977-119">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="32977-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="32977-120">Чтение свойств и связей объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="32977-120">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="32977-121">Список tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="32977-121">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="32977-122">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="32977-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="32977-123">Чтение свойств и связей объектов tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="32977-123">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="32977-124">Обновление tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="32977-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="32977-125">Нет</span><span class="sxs-lookup"><span data-stu-id="32977-125">None</span></span> | <span data-ttu-id="32977-126">Обновление объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="32977-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="32977-127">Удаление tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="32977-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="32977-128">Нет</span><span class="sxs-lookup"><span data-stu-id="32977-128">None</span></span> | <span data-ttu-id="32977-129">Удаление объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="32977-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="32977-130">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="32977-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="32977-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="32977-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="32977-132">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="32977-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="32977-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="32977-133">Properties</span></span>

| <span data-ttu-id="32977-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="32977-134">Property</span></span>     | <span data-ttu-id="32977-135">Тип</span><span class="sxs-lookup"><span data-stu-id="32977-135">Type</span></span>        | <span data-ttu-id="32977-136">Описание</span><span class="sxs-lookup"><span data-stu-id="32977-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="32977-137">id</span><span class="sxs-lookup"><span data-stu-id="32977-137">id</span></span>|<span data-ttu-id="32977-138">String</span><span class="sxs-lookup"><span data-stu-id="32977-138">String</span></span>| <span data-ttu-id="32977-139">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="32977-139">Unique identifier for this policy.</span></span> <span data-ttu-id="32977-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32977-140">Read-only.</span></span>|
|<span data-ttu-id="32977-141">definition</span><span class="sxs-lookup"><span data-stu-id="32977-141">definition</span></span>|<span data-ttu-id="32977-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="32977-142">String collection</span></span>| <span data-ttu-id="32977-143">Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="32977-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="32977-144">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="32977-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="32977-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32977-145">Required.</span></span>|
|<span data-ttu-id="32977-146">description</span><span class="sxs-lookup"><span data-stu-id="32977-146">description</span></span>|<span data-ttu-id="32977-147">String</span><span class="sxs-lookup"><span data-stu-id="32977-147">String</span></span>| <span data-ttu-id="32977-148">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="32977-148">Description for this policy.</span></span>|
|<span data-ttu-id="32977-149">displayName</span><span class="sxs-lookup"><span data-stu-id="32977-149">displayName</span></span>|<span data-ttu-id="32977-150">String</span><span class="sxs-lookup"><span data-stu-id="32977-150">String</span></span>| <span data-ttu-id="32977-151">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="32977-151">Display name for this policy.</span></span> <span data-ttu-id="32977-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="32977-152">Required.</span></span>|
|<span data-ttu-id="32977-153">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="32977-153">isOrganizationDefault</span></span>|<span data-ttu-id="32977-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="32977-154">Boolean</span></span>|<span data-ttu-id="32977-155">Игнорируйте это свойство.</span><span class="sxs-lookup"><span data-stu-id="32977-155">Ignore this property.</span></span> <span data-ttu-id="32977-156">Политика выдачи маркеров может применяться только к тем или иным основным службам и не может быть установлена глобально для организации.</span><span class="sxs-lookup"><span data-stu-id="32977-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="32977-157">Свойства определения политики выдачи маркеров</span><span class="sxs-lookup"><span data-stu-id="32977-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="32977-158">Свойства формируют объект JSON, который представляет политику выдачи маркеров.</span><span class="sxs-lookup"><span data-stu-id="32977-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="32977-159">Этот объект JSON необходимо **преобразовать** в строку с escape-кавычками, чтобы вставить его в **свойство** определения.</span><span class="sxs-lookup"><span data-stu-id="32977-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="32977-160">Ниже приводится пример в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="32977-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="32977-161">Свойство</span><span class="sxs-lookup"><span data-stu-id="32977-161">Property</span></span>     | <span data-ttu-id="32977-162">Тип</span><span class="sxs-lookup"><span data-stu-id="32977-162">Type</span></span>   |<span data-ttu-id="32977-163">Описание</span><span class="sxs-lookup"><span data-stu-id="32977-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32977-164">TokenResponseSigningPolicy</span><span class="sxs-lookup"><span data-stu-id="32977-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="32977-165">String</span><span class="sxs-lookup"><span data-stu-id="32977-165">String</span></span>|<span data-ttu-id="32977-166">Представляет параметры подписи сертификатов, доступные в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="32977-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="32977-167">Поддерживаемые значения: `ResponseOnly` , `TokenOnly` , `ResponseAndToken` .</span><span class="sxs-lookup"><span data-stu-id="32977-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="32977-168">SamlTokenVersion</span><span class="sxs-lookup"><span data-stu-id="32977-168">SamlTokenVersion</span></span>|<span data-ttu-id="32977-169">String</span><span class="sxs-lookup"><span data-stu-id="32977-169">String</span></span>|<span data-ttu-id="32977-170">Версия маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="32977-170">Version of the SAML token.</span></span> <span data-ttu-id="32977-171">Поддерживаемые значения: `1.1` , `2.0` .</span><span class="sxs-lookup"><span data-stu-id="32977-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="32977-172">SigningAlgorithm</span><span class="sxs-lookup"><span data-stu-id="32977-172">SigningAlgorithm</span></span>|<span data-ttu-id="32977-173">String</span><span class="sxs-lookup"><span data-stu-id="32977-173">String</span></span>|<span data-ttu-id="32977-174">Алгоритм подписи, который Azure AD использует для подписи маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="32977-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="32977-175">Поддерживаемые значения: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` , `http://www.w3.org/2000/09/xmldsig#rsa-sha1` .</span><span class="sxs-lookup"><span data-stu-id="32977-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="32977-176">Версия</span><span class="sxs-lookup"><span data-stu-id="32977-176">Version</span></span>|<span data-ttu-id="32977-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="32977-177">Integer</span></span>|<span data-ttu-id="32977-178">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="32977-178">Set value of 1.</span></span> <span data-ttu-id="32977-179">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32977-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="32977-180">Связи</span><span class="sxs-lookup"><span data-stu-id="32977-180">Relationships</span></span>

| <span data-ttu-id="32977-181">Связь</span><span class="sxs-lookup"><span data-stu-id="32977-181">Relationship</span></span> | <span data-ttu-id="32977-182">Тип</span><span class="sxs-lookup"><span data-stu-id="32977-182">Type</span></span>        | <span data-ttu-id="32977-183">Описание</span><span class="sxs-lookup"><span data-stu-id="32977-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="32977-184">appliesTo</span><span class="sxs-lookup"><span data-stu-id="32977-184">appliesTo</span></span>|<span data-ttu-id="32977-185">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="32977-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="32977-186">Коллекция [directoryObject,](directoryObject.md) к которую применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="32977-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="32977-187">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32977-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32977-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32977-188">JSON representation</span></span>

<span data-ttu-id="32977-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32977-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenIssuancePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


