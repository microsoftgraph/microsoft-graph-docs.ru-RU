---
title: Обновление onPremisesPublishingProfile
description: Обновление свойств объекта onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e1200e66da53b564e21396bbf347959a3223fd3a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132794"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="ba130-103">Обновление onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="ba130-103">Update onPremisesPublishingProfile</span></span>

<span data-ttu-id="ba130-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba130-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba130-105">Обновление свойств объекта [onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba130-105">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba130-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba130-106">Permissions</span></span>

<span data-ttu-id="ba130-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba130-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba130-109">Permission type</span></span>                        | <span data-ttu-id="ba130-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba130-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="ba130-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba130-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba130-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba130-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="ba130-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba130-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba130-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba130-114">Not supported.</span></span> |
| <span data-ttu-id="ba130-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba130-115">Application</span></span>                            | <span data-ttu-id="ba130-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba130-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba130-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba130-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="ba130-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba130-118">Request headers</span></span>

| <span data-ttu-id="ba130-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ba130-119">Name</span></span>       | <span data-ttu-id="ba130-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ba130-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ba130-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba130-121">Authorization</span></span> | <span data-ttu-id="ba130-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ba130-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba130-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba130-123">Request body</span></span>

<span data-ttu-id="ba130-124">В теле запроса укавите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ba130-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="ba130-125">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="ba130-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ba130-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ba130-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ba130-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba130-127">Property</span></span>     | <span data-ttu-id="ba130-128">Тип</span><span class="sxs-lookup"><span data-stu-id="ba130-128">Type</span></span>        | <span data-ttu-id="ba130-129">Описание</span><span class="sxs-lookup"><span data-stu-id="ba130-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba130-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba130-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="ba130-131">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba130-131">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="ba130-132">Представляет [hybridAgentUpdaterConfiguration.](../resources/hybridagentupdaterconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba130-132">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ba130-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba130-133">Response</span></span>

<span data-ttu-id="ba130-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba130-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ba130-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba130-135">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="ba130-136">Пример 1. Обновление updateWindow в гибридной версииAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba130-136">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="ba130-137">В следующем примере **обновляется updateWindow** в **гибридной версииAgentUpdaterConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="ba130-137">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="ba130-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba130-138">Request</span></span>

<span data-ttu-id="ba130-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba130-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba130-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba130-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
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
# <a name="c"></a>[<span data-ttu-id="ba130-141">C#</span><span class="sxs-lookup"><span data-stu-id="ba130-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba130-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba130-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba130-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba130-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba130-144">Java</span><span class="sxs-lookup"><span data-stu-id="ba130-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ba130-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba130-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="ba130-146">Пример 2. Обновление deferUpdate в гибридной версииAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba130-146">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="ba130-147">В следующем примере обновления **deferUpdate** в **гибридной версииAgentUpdaterConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="ba130-147">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="ba130-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba130-148">Request</span></span>

<span data-ttu-id="ba130-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba130-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "deferUpdate" : "2018-08-20T12:00"
}
```

#### <a name="response"></a><span data-ttu-id="ba130-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba130-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="ba130-151">Пример 3. Обновление allowUpdateConfigurationOverride в гибридной версииAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba130-151">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="ba130-152">В следующем примере **обновляется allowUpdateConfigurationOverride в** **гибридной версииAgentUpdaterConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="ba130-152">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="ba130-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba130-153">Request</span></span>

<span data-ttu-id="ba130-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba130-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "allowUpdateConfigurationOverride" : false
}
```

#### <a name="response"></a><span data-ttu-id="ba130-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba130-155">Response</span></span>

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



