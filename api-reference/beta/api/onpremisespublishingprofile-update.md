---
title: Обновление Онпремисеспублишингпрофиле
description: Обновление свойств объекта Онпремисеспублишингпрофиле.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b4d2eac82b47549633b03c39465e4107e4fcd8b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414506"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="8e8d1-103">Обновление Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="8e8d1-103">Update onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e8d1-104">Обновление свойств объекта [онпремисеспублишингпрофиле](../resources/onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8e8d1-104">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e8d1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e8d1-105">Permissions</span></span>

<span data-ttu-id="8e8d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e8d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e8d1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e8d1-108">Permission type</span></span>                        | <span data-ttu-id="8e8d1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e8d1-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="8e8d1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e8d1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e8d1-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8e8d1-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="8e8d1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e8d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e8d1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-113">Not supported.</span></span> |
| <span data-ttu-id="8e8d1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e8d1-114">Application</span></span>                            | <span data-ttu-id="8e8d1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e8d1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e8d1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="8e8d1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e8d1-117">Request headers</span></span>

| <span data-ttu-id="8e8d1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8e8d1-118">Name</span></span>       | <span data-ttu-id="8e8d1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8e8d1-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8e8d1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e8d1-120">Authorization</span></span> | <span data-ttu-id="8e8d1-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8e8d1-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e8d1-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e8d1-122">Request body</span></span>

<span data-ttu-id="8e8d1-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="8e8d1-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8e8d1-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8e8d1-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e8d1-126">Property</span></span>     | <span data-ttu-id="8e8d1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8e8d1-127">Type</span></span>        | <span data-ttu-id="8e8d1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8e8d1-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e8d1-129">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8e8d1-129">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="8e8d1-130">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8e8d1-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="8e8d1-131">Представляет [хибридажентупдатерконфигуратион](../resources/hybridagentupdaterconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e8d1-131">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="8e8d1-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e8d1-132">Response</span></span>

<span data-ttu-id="8e8d1-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8e8d1-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="8e8d1-134">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="8e8d1-135">Пример 1: обновление Упдатевиндов в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8e8d1-135">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="8e8d1-136">В следующем примере выполняется обновление **упдатевиндов** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-136">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="8e8d1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e8d1-137">Request</span></span>

<span data-ttu-id="8e8d1-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8e8d1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e8d1-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e8d1-140">C#</span><span class="sxs-lookup"><span data-stu-id="8e8d1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e8d1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e8d1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e8d1-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8e8d1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e8d1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e8d1-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="8e8d1-144">Пример 2: обновление Деферупдате в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8e8d1-144">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="8e8d1-145">В следующем примере показано, как обновить **деферупдате** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-145">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="8e8d1-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e8d1-146">Request</span></span>

<span data-ttu-id="8e8d1-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-147">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="8e8d1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e8d1-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="8e8d1-149">Пример 3: обновление Алловупдатеконфигуратионоверриде в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8e8d1-149">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="8e8d1-150">В следующем примере показано, как обновить **алловупдатеконфигуратионоверриде** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-150">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="8e8d1-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e8d1-151">Request</span></span>

<span data-ttu-id="8e8d1-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e8d1-152">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="8e8d1-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e8d1-153">Response</span></span>

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
