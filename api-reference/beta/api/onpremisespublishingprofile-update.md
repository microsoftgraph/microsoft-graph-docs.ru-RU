---
title: Обновление наPremisesPublishingProfile
description: Обновление свойств объекта onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8749ba414fc675fbdba4bed13a858b7d6512347d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963225"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="249f9-103">Обновление наPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="249f9-103">Update onPremisesPublishingProfile</span></span>

<span data-ttu-id="249f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="249f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="249f9-105">Обновление свойств объекта [onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="249f9-105">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="249f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="249f9-106">Permissions</span></span>

<span data-ttu-id="249f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="249f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="249f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="249f9-109">Permission type</span></span>                        | <span data-ttu-id="249f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="249f9-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="249f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="249f9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="249f9-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="249f9-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="249f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="249f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="249f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="249f9-114">Not supported.</span></span> |
| <span data-ttu-id="249f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="249f9-115">Application</span></span>                            | <span data-ttu-id="249f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="249f9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="249f9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="249f9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="249f9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="249f9-118">Request headers</span></span>

| <span data-ttu-id="249f9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="249f9-119">Name</span></span>       | <span data-ttu-id="249f9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="249f9-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="249f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="249f9-121">Authorization</span></span> | <span data-ttu-id="249f9-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="249f9-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="249f9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="249f9-123">Request body</span></span>

<span data-ttu-id="249f9-124">В теле запроса укажи значения для обновления соответствующих полей.</span><span class="sxs-lookup"><span data-stu-id="249f9-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="249f9-125">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="249f9-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="249f9-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="249f9-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="249f9-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="249f9-127">Property</span></span>     | <span data-ttu-id="249f9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="249f9-128">Type</span></span>        | <span data-ttu-id="249f9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="249f9-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="249f9-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="249f9-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="249f9-131">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="249f9-131">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="249f9-132">Представляет [гибридAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="249f9-132">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="249f9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="249f9-133">Response</span></span>

<span data-ttu-id="249f9-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="249f9-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="249f9-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="249f9-135">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="249f9-136">Пример 1. ОбновлениеWindow в hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="249f9-136">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="249f9-137">В следующем примере **обновляется обновлениеWindow** в **гибридеAgentUpdaterConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="249f9-137">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="249f9-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="249f9-138">Request</span></span>

<span data-ttu-id="249f9-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="249f9-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="249f9-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="249f9-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
   "updateWindow" :
{
      "updateWindowStartTime" : "0:00:00",
      "updateWindowEndTime" : "23:59:00"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="249f9-141">C#</span><span class="sxs-lookup"><span data-stu-id="249f9-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="249f9-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="249f9-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="249f9-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="249f9-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="249f9-144">Java</span><span class="sxs-lookup"><span data-stu-id="249f9-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisespublishingprofile-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="249f9-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="249f9-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="249f9-146">Пример 2. Обновление deferUpdate в гибридной версииAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="249f9-146">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="249f9-147">В следующем примере обновления **deferUpdate** в **гибридеAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="249f9-147">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="249f9-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="249f9-148">Request</span></span>

<span data-ttu-id="249f9-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="249f9-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="249f9-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="249f9-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "deferUpdate" : "2018-08-20T12:00"
}
```
# <a name="javascript"></a>[<span data-ttu-id="249f9-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="249f9-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="249f9-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="249f9-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="249f9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="249f9-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="249f9-154">Пример 3. Обновление allowUpdateConfigurationOverride в hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="249f9-154">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="249f9-155">В следующем примере обновления **позволяютUpdateConfigurationOverride в** **hybridAgentUpdaterConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="249f9-155">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="249f9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="249f9-156">Request</span></span>

<span data-ttu-id="249f9-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="249f9-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="249f9-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="249f9-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile_3"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "allowUpdateConfigurationOverride" : false
}
```
# <a name="c"></a>[<span data-ttu-id="249f9-159">C#</span><span class="sxs-lookup"><span data-stu-id="249f9-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="249f9-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="249f9-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="249f9-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="249f9-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="249f9-162">Java</span><span class="sxs-lookup"><span data-stu-id="249f9-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisespublishingprofile-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="249f9-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="249f9-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update onpremisespublishingprofile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



