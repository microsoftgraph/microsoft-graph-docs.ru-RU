---
title: тип ресурса tokenIssuancePolicy
description: Представляет политику, определяемую характеристиками маркеров SAML, выданных Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 761e1d7e45f2d6a2cb11513cd3484a88a080888e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444324"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="04f78-103">тип ресурса tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="04f78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04f78-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="04f78-105">Представляет политику, определяемую характеристиками маркеров SAML, выданных Azure AD.</span><span class="sxs-lookup"><span data-stu-id="04f78-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="04f78-106">Политики выдачи маркеров можно использовать для:</span><span class="sxs-lookup"><span data-stu-id="04f78-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="04f78-107">Настройка параметров подписи</span><span class="sxs-lookup"><span data-stu-id="04f78-107">Set signing options</span></span>
- <span data-ttu-id="04f78-108">Настройка алгоритма подписи</span><span class="sxs-lookup"><span data-stu-id="04f78-108">Set signing algorithm</span></span>
- <span data-ttu-id="04f78-109">Установите версию маркера SAML</span><span class="sxs-lookup"><span data-stu-id="04f78-109">Set SAML token version</span></span>

<span data-ttu-id="04f78-110">Наследует [от stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="04f78-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="04f78-111">Методы</span><span class="sxs-lookup"><span data-stu-id="04f78-111">Methods</span></span>

| <span data-ttu-id="04f78-112">Метод</span><span class="sxs-lookup"><span data-stu-id="04f78-112">Method</span></span>       | <span data-ttu-id="04f78-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="04f78-113">Return Type</span></span> | <span data-ttu-id="04f78-114">Описание</span><span class="sxs-lookup"><span data-stu-id="04f78-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="04f78-115">List tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-115">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="04f78-116">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="04f78-117">Чтение свойств и связей объектов tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="04f78-117">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="04f78-118">Создание tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-118">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="04f78-119">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="04f78-120">Создание объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="04f78-120">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="04f78-121">Get tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-121">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="04f78-122">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="04f78-123">Чтение свойств и связей объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="04f78-123">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="04f78-124">Обновление tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="04f78-125">Нет</span><span class="sxs-lookup"><span data-stu-id="04f78-125">None</span></span> | <span data-ttu-id="04f78-126">Обновление объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="04f78-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="04f78-127">Удаление tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="04f78-128">Нет</span><span class="sxs-lookup"><span data-stu-id="04f78-128">None</span></span> | <span data-ttu-id="04f78-129">Удаление объекта tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="04f78-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="04f78-130">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="04f78-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="04f78-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="04f78-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="04f78-132">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="04f78-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="04f78-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="04f78-133">Properties</span></span>

| <span data-ttu-id="04f78-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="04f78-134">Property</span></span>     | <span data-ttu-id="04f78-135">Тип</span><span class="sxs-lookup"><span data-stu-id="04f78-135">Type</span></span>        | <span data-ttu-id="04f78-136">Описание</span><span class="sxs-lookup"><span data-stu-id="04f78-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04f78-137">id</span><span class="sxs-lookup"><span data-stu-id="04f78-137">id</span></span>|<span data-ttu-id="04f78-138">String</span><span class="sxs-lookup"><span data-stu-id="04f78-138">String</span></span>| <span data-ttu-id="04f78-139">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="04f78-139">Unique identifier for this policy.</span></span> <span data-ttu-id="04f78-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04f78-140">Read-only.</span></span>|
|<span data-ttu-id="04f78-141">определение</span><span class="sxs-lookup"><span data-stu-id="04f78-141">definition</span></span>|<span data-ttu-id="04f78-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="04f78-142">String collection</span></span>| <span data-ttu-id="04f78-143">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.</span><span class="sxs-lookup"><span data-stu-id="04f78-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="04f78-144">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="04f78-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="04f78-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04f78-145">Required.</span></span>|
|<span data-ttu-id="04f78-146">description</span><span class="sxs-lookup"><span data-stu-id="04f78-146">description</span></span>|<span data-ttu-id="04f78-147">String</span><span class="sxs-lookup"><span data-stu-id="04f78-147">String</span></span>| <span data-ttu-id="04f78-148">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="04f78-148">Description for this policy.</span></span>|
|<span data-ttu-id="04f78-149">displayName</span><span class="sxs-lookup"><span data-stu-id="04f78-149">displayName</span></span>|<span data-ttu-id="04f78-150">String</span><span class="sxs-lookup"><span data-stu-id="04f78-150">String</span></span>| <span data-ttu-id="04f78-151">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="04f78-151">Display name for this policy.</span></span> <span data-ttu-id="04f78-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="04f78-152">Required.</span></span>|
|<span data-ttu-id="04f78-153">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="04f78-153">isOrganizationDefault</span></span>|<span data-ttu-id="04f78-154">Логический</span><span class="sxs-lookup"><span data-stu-id="04f78-154">Boolean</span></span>|<span data-ttu-id="04f78-155">Игнорируйте это свойство.</span><span class="sxs-lookup"><span data-stu-id="04f78-155">Ignore this property.</span></span> <span data-ttu-id="04f78-156">Политика выдачи маркеров может применяться только к директорам служб и не может быть установлена глобально для организации.</span><span class="sxs-lookup"><span data-stu-id="04f78-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="04f78-157">Свойства определения политики выдачи маркеров</span><span class="sxs-lookup"><span data-stu-id="04f78-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="04f78-158">Свойства формируют объект JSON, который представляет политику выдачи маркеров.</span><span class="sxs-lookup"><span data-stu-id="04f78-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="04f78-159">Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.**</span><span class="sxs-lookup"><span data-stu-id="04f78-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="04f78-160">Ниже приводится пример в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="04f78-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="04f78-161">Свойство</span><span class="sxs-lookup"><span data-stu-id="04f78-161">Property</span></span>     | <span data-ttu-id="04f78-162">Тип</span><span class="sxs-lookup"><span data-stu-id="04f78-162">Type</span></span>   |<span data-ttu-id="04f78-163">Описание</span><span class="sxs-lookup"><span data-stu-id="04f78-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04f78-164">TokenResponseSigningPolicy</span><span class="sxs-lookup"><span data-stu-id="04f78-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="04f78-165">String</span><span class="sxs-lookup"><span data-stu-id="04f78-165">String</span></span>|<span data-ttu-id="04f78-166">Представляет параметры подписи сертификатов, доступные в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="04f78-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="04f78-167">Поддерживаемые значения: `ResponseOnly` `TokenOnly` , `ResponseAndToken` .</span><span class="sxs-lookup"><span data-stu-id="04f78-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="04f78-168">SamlTokenVersion</span><span class="sxs-lookup"><span data-stu-id="04f78-168">SamlTokenVersion</span></span>|<span data-ttu-id="04f78-169">String</span><span class="sxs-lookup"><span data-stu-id="04f78-169">String</span></span>|<span data-ttu-id="04f78-170">Версия маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="04f78-170">Version of the SAML token.</span></span> <span data-ttu-id="04f78-171">Поддерживаемые значения: `1.1` , `2.0` .</span><span class="sxs-lookup"><span data-stu-id="04f78-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="04f78-172">SigningAlgorithm</span><span class="sxs-lookup"><span data-stu-id="04f78-172">SigningAlgorithm</span></span>|<span data-ttu-id="04f78-173">String</span><span class="sxs-lookup"><span data-stu-id="04f78-173">String</span></span>|<span data-ttu-id="04f78-174">Использование алгоритма подписи в Azure AD для подписи маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="04f78-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="04f78-175">Поддерживаемые значения: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` , `http://www.w3.org/2000/09/xmldsig#rsa-sha1` .</span><span class="sxs-lookup"><span data-stu-id="04f78-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="04f78-176">Версия</span><span class="sxs-lookup"><span data-stu-id="04f78-176">Version</span></span>|<span data-ttu-id="04f78-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="04f78-177">Integer</span></span>|<span data-ttu-id="04f78-178">Значение 1.</span><span class="sxs-lookup"><span data-stu-id="04f78-178">Set value of 1.</span></span> <span data-ttu-id="04f78-179">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04f78-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="04f78-180">Связи</span><span class="sxs-lookup"><span data-stu-id="04f78-180">Relationships</span></span>

| <span data-ttu-id="04f78-181">Связь</span><span class="sxs-lookup"><span data-stu-id="04f78-181">Relationship</span></span> | <span data-ttu-id="04f78-182">Тип</span><span class="sxs-lookup"><span data-stu-id="04f78-182">Type</span></span>        | <span data-ttu-id="04f78-183">Описание</span><span class="sxs-lookup"><span data-stu-id="04f78-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04f78-184">appliesTo</span><span class="sxs-lookup"><span data-stu-id="04f78-184">appliesTo</span></span>|<span data-ttu-id="04f78-185">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="04f78-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="04f78-186">Коллекция [directoryObject,](directoryObject.md) к которую была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="04f78-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="04f78-187">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04f78-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04f78-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04f78-188">JSON representation</span></span>

<span data-ttu-id="04f78-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04f78-189">The following is a JSON representation of the resource.</span></span>

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

