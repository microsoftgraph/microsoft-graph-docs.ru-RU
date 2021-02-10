---
title: Тип ресурса tokenIssuancePolicy
description: Представляет политику для указания характеристик маркеров SAML, выдавляемой Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a74664438d7a7201f331c4dca1105d523478e3ae
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154728"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="d14ae-103">Тип ресурса tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="d14ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d14ae-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="d14ae-105">Представляет политику для указания характеристик маркеров SAML, выдавляемой Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d14ae-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="d14ae-106">Политики выдачи маркеров можно использовать для:</span><span class="sxs-lookup"><span data-stu-id="d14ae-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="d14ae-107">Настройка параметров подписи</span><span class="sxs-lookup"><span data-stu-id="d14ae-107">Set signing options</span></span>
- <span data-ttu-id="d14ae-108">Настройка алгоритма подписи</span><span class="sxs-lookup"><span data-stu-id="d14ae-108">Set signing algorithm</span></span>
- <span data-ttu-id="d14ae-109">Настройка версии маркера SAML</span><span class="sxs-lookup"><span data-stu-id="d14ae-109">Set SAML token version</span></span>

<span data-ttu-id="d14ae-110">Наследуется от [stsPolicy.](stsPolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d14ae-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d14ae-111">Методы</span><span class="sxs-lookup"><span data-stu-id="d14ae-111">Methods</span></span>

| <span data-ttu-id="d14ae-112">Метод</span><span class="sxs-lookup"><span data-stu-id="d14ae-112">Method</span></span>       | <span data-ttu-id="d14ae-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d14ae-113">Return Type</span></span> | <span data-ttu-id="d14ae-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d14ae-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d14ae-115">Список tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-115">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="d14ae-116">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="d14ae-117">Чтение свойств и связей объектов tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d14ae-117">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="d14ae-118">Создание tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-118">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="d14ae-119">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="d14ae-120">Создание объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d14ae-120">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="d14ae-121">Get tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-121">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="d14ae-122">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="d14ae-123">Чтение свойств и связей объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d14ae-123">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="d14ae-124">Обновление tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="d14ae-125">Нет</span><span class="sxs-lookup"><span data-stu-id="d14ae-125">None</span></span> | <span data-ttu-id="d14ae-126">Обновление объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d14ae-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="d14ae-127">Удаление tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="d14ae-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d14ae-128">None</span></span> | <span data-ttu-id="d14ae-129">Удаление объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d14ae-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="d14ae-130">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="d14ae-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="d14ae-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="d14ae-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="d14ae-132">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="d14ae-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="d14ae-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="d14ae-133">Properties</span></span>

| <span data-ttu-id="d14ae-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="d14ae-134">Property</span></span>     | <span data-ttu-id="d14ae-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d14ae-135">Type</span></span>        | <span data-ttu-id="d14ae-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d14ae-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d14ae-137">id</span><span class="sxs-lookup"><span data-stu-id="d14ae-137">id</span></span>|<span data-ttu-id="d14ae-138">String</span><span class="sxs-lookup"><span data-stu-id="d14ae-138">String</span></span>| <span data-ttu-id="d14ae-139">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d14ae-139">Unique identifier for this policy.</span></span> <span data-ttu-id="d14ae-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d14ae-140">Read-only.</span></span>|
|<span data-ttu-id="d14ae-141">definition</span><span class="sxs-lookup"><span data-stu-id="d14ae-141">definition</span></span>|<span data-ttu-id="d14ae-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d14ae-142">String collection</span></span>| <span data-ttu-id="d14ae-143">Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d14ae-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="d14ae-144">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="d14ae-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="d14ae-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d14ae-145">Required.</span></span>|
|<span data-ttu-id="d14ae-146">description</span><span class="sxs-lookup"><span data-stu-id="d14ae-146">description</span></span>|<span data-ttu-id="d14ae-147">String</span><span class="sxs-lookup"><span data-stu-id="d14ae-147">String</span></span>| <span data-ttu-id="d14ae-148">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="d14ae-148">Description for this policy.</span></span>|
|<span data-ttu-id="d14ae-149">displayName</span><span class="sxs-lookup"><span data-stu-id="d14ae-149">displayName</span></span>|<span data-ttu-id="d14ae-150">String</span><span class="sxs-lookup"><span data-stu-id="d14ae-150">String</span></span>| <span data-ttu-id="d14ae-151">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d14ae-151">Display name for this policy.</span></span> <span data-ttu-id="d14ae-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d14ae-152">Required.</span></span>|
|<span data-ttu-id="d14ae-153">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="d14ae-153">isOrganizationDefault</span></span>|<span data-ttu-id="d14ae-154">Логическое</span><span class="sxs-lookup"><span data-stu-id="d14ae-154">Boolean</span></span>|<span data-ttu-id="d14ae-155">Игнорируйте это свойство.</span><span class="sxs-lookup"><span data-stu-id="d14ae-155">Ignore this property.</span></span> <span data-ttu-id="d14ae-156">Политика выдачи маркеров может применяться только к тем или иным основным службам и не может быть установлена глобально для организации.</span><span class="sxs-lookup"><span data-stu-id="d14ae-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="d14ae-157">Свойства определения политики выдачи маркеров</span><span class="sxs-lookup"><span data-stu-id="d14ae-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="d14ae-158">Свойства формируют объект JSON, который представляет политику выдачи маркеров.</span><span class="sxs-lookup"><span data-stu-id="d14ae-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="d14ae-159">Этот объект JSON необходимо **преобразовать** в строку с escape-кавычками, чтобы вставить его в **свойство** определения.</span><span class="sxs-lookup"><span data-stu-id="d14ae-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="d14ae-160">Ниже приводится пример в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="d14ae-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="d14ae-161">Свойство</span><span class="sxs-lookup"><span data-stu-id="d14ae-161">Property</span></span>     | <span data-ttu-id="d14ae-162">Тип</span><span class="sxs-lookup"><span data-stu-id="d14ae-162">Type</span></span>   |<span data-ttu-id="d14ae-163">Описание</span><span class="sxs-lookup"><span data-stu-id="d14ae-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d14ae-164">TokenResponseSigningPolicy</span><span class="sxs-lookup"><span data-stu-id="d14ae-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="d14ae-165">String</span><span class="sxs-lookup"><span data-stu-id="d14ae-165">String</span></span>|<span data-ttu-id="d14ae-166">Представляет параметры подписи сертификатов, доступные в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d14ae-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="d14ae-167">Поддерживаемые значения: `ResponseOnly` , `TokenOnly` , `ResponseAndToken` .</span><span class="sxs-lookup"><span data-stu-id="d14ae-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="d14ae-168">SamlTokenVersion</span><span class="sxs-lookup"><span data-stu-id="d14ae-168">SamlTokenVersion</span></span>|<span data-ttu-id="d14ae-169">String</span><span class="sxs-lookup"><span data-stu-id="d14ae-169">String</span></span>|<span data-ttu-id="d14ae-170">Версия маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="d14ae-170">Version of the SAML token.</span></span> <span data-ttu-id="d14ae-171">Поддерживаемые значения: `1.1` , `2.0` .</span><span class="sxs-lookup"><span data-stu-id="d14ae-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="d14ae-172">SigningAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d14ae-172">SigningAlgorithm</span></span>|<span data-ttu-id="d14ae-173">String</span><span class="sxs-lookup"><span data-stu-id="d14ae-173">String</span></span>|<span data-ttu-id="d14ae-174">Алгоритм подписи, который azure AD использует для подписи маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="d14ae-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="d14ae-175">Поддерживаемые значения: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` , `http://www.w3.org/2000/09/xmldsig#rsa-sha1` .</span><span class="sxs-lookup"><span data-stu-id="d14ae-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="d14ae-176">Версия</span><span class="sxs-lookup"><span data-stu-id="d14ae-176">Version</span></span>|<span data-ttu-id="d14ae-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="d14ae-177">Integer</span></span>|<span data-ttu-id="d14ae-178">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="d14ae-178">Set value of 1.</span></span> <span data-ttu-id="d14ae-179">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d14ae-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d14ae-180">Связи</span><span class="sxs-lookup"><span data-stu-id="d14ae-180">Relationships</span></span>

| <span data-ttu-id="d14ae-181">Связь</span><span class="sxs-lookup"><span data-stu-id="d14ae-181">Relationship</span></span> | <span data-ttu-id="d14ae-182">Тип</span><span class="sxs-lookup"><span data-stu-id="d14ae-182">Type</span></span>        | <span data-ttu-id="d14ae-183">Описание</span><span class="sxs-lookup"><span data-stu-id="d14ae-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d14ae-184">appliesTo</span><span class="sxs-lookup"><span data-stu-id="d14ae-184">appliesTo</span></span>|<span data-ttu-id="d14ae-185">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="d14ae-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d14ae-186">Коллекция [directoryObject,](directoryObject.md) к которую применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="d14ae-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="d14ae-187">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d14ae-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d14ae-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d14ae-188">JSON representation</span></span>

<span data-ttu-id="d14ae-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d14ae-189">The following is a JSON representation of the resource.</span></span>

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

