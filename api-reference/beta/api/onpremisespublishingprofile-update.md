---
title: Обновление Онпремисеспублишингпрофиле
description: Обновление свойств объекта Онпремисеспублишингпрофиле.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e08645e9e1f68b57eec4bfb0e33bdfaf7ac2d5d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456443"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="7afe4-103">Обновление Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="7afe4-103">Update onPremisesPublishingProfile</span></span>

<span data-ttu-id="7afe4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7afe4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7afe4-105">Обновление свойств объекта [онпремисеспублишингпрофиле](../resources/onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7afe4-105">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7afe4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7afe4-106">Permissions</span></span>

<span data-ttu-id="7afe4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7afe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7afe4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7afe4-109">Permission type</span></span>                        | <span data-ttu-id="7afe4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7afe4-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="7afe4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7afe4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7afe4-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7afe4-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="7afe4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7afe4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7afe4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7afe4-114">Not supported.</span></span> |
| <span data-ttu-id="7afe4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7afe4-115">Application</span></span>                            | <span data-ttu-id="7afe4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7afe4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7afe4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7afe4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="7afe4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7afe4-118">Request headers</span></span>

| <span data-ttu-id="7afe4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7afe4-119">Name</span></span>       | <span data-ttu-id="7afe4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7afe4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7afe4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7afe4-121">Authorization</span></span> | <span data-ttu-id="7afe4-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="7afe4-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7afe4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7afe4-123">Request body</span></span>

<span data-ttu-id="7afe4-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="7afe4-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="7afe4-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="7afe4-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7afe4-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7afe4-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7afe4-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="7afe4-127">Property</span></span>     | <span data-ttu-id="7afe4-128">Тип</span><span class="sxs-lookup"><span data-stu-id="7afe4-128">Type</span></span>        | <span data-ttu-id="7afe4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7afe4-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7afe4-130">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7afe4-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="7afe4-131">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7afe4-131">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="7afe4-132">Представляет [хибридажентупдатерконфигуратион](../resources/hybridagentupdaterconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7afe4-132">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="7afe4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7afe4-133">Response</span></span>

<span data-ttu-id="7afe4-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7afe4-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7afe4-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="7afe4-135">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="7afe4-136">Пример 1: обновление Упдатевиндов в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7afe4-136">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="7afe4-137">В следующем примере выполняется обновление **упдатевиндов** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="7afe4-137">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="7afe4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7afe4-138">Request</span></span>

<span data-ttu-id="7afe4-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7afe4-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7afe4-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="7afe4-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7afe4-141">C#</span><span class="sxs-lookup"><span data-stu-id="7afe4-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7afe4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7afe4-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7afe4-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7afe4-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7afe4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7afe4-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="7afe4-145">Пример 2: обновление Деферупдате в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7afe4-145">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="7afe4-146">В следующем примере показано, как обновить **деферупдате** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="7afe4-146">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="7afe4-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="7afe4-147">Request</span></span>

<span data-ttu-id="7afe4-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7afe4-148">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="7afe4-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="7afe4-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="7afe4-150">Пример 3: обновление Алловупдатеконфигуратионоверриде в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7afe4-150">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="7afe4-151">В следующем примере показано, как обновить **алловупдатеконфигуратионоверриде** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="7afe4-151">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="7afe4-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="7afe4-152">Request</span></span>

<span data-ttu-id="7afe4-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7afe4-153">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="7afe4-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7afe4-154">Response</span></span>

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
