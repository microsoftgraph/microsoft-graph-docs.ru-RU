---
title: Обновление Онпремисеспублишингпрофиле
description: Обновление свойств объекта Онпремисеспублишингпрофиле.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: adb963d1f9b3ee2e0c6625a786e35a77682f6d4d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878289"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="63988-103">Обновление Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="63988-103">Update onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63988-104">Обновление свойств объекта [онпремисеспублишингпрофиле](../resources/onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="63988-104">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63988-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63988-105">Permissions</span></span>

<span data-ttu-id="63988-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63988-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63988-108">Permission type</span></span>                        | <span data-ttu-id="63988-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63988-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="63988-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63988-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="63988-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="63988-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="63988-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63988-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63988-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63988-113">Not supported.</span></span> |
| <span data-ttu-id="63988-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63988-114">Application</span></span>                            | <span data-ttu-id="63988-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63988-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63988-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63988-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="63988-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63988-117">Request headers</span></span>

| <span data-ttu-id="63988-118">Имя</span><span class="sxs-lookup"><span data-stu-id="63988-118">Name</span></span>       | <span data-ttu-id="63988-119">Описание</span><span class="sxs-lookup"><span data-stu-id="63988-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="63988-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63988-120">Authorization</span></span> | <span data-ttu-id="63988-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="63988-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="63988-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="63988-122">Request body</span></span>

<span data-ttu-id="63988-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="63988-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="63988-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="63988-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="63988-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="63988-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="63988-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="63988-126">Property</span></span>     | <span data-ttu-id="63988-127">Тип</span><span class="sxs-lookup"><span data-stu-id="63988-127">Type</span></span>        | <span data-ttu-id="63988-128">Описание</span><span class="sxs-lookup"><span data-stu-id="63988-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63988-129">Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="63988-129">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="63988-130">Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="63988-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="63988-131">Представляет [хибридажентупдатерконфигуратион](../resources/hybridagentupdaterconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63988-131">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="63988-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="63988-132">Response</span></span>

<span data-ttu-id="63988-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="63988-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="63988-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="63988-134">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="63988-135">Пример 1: обновление Упдатевиндов в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="63988-135">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="63988-136">В следующем примере выполняется обновление **упдатевиндов** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="63988-136">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="63988-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="63988-137">Request</span></span>

<span data-ttu-id="63988-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63988-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63988-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="63988-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="63988-140">C#</span><span class="sxs-lookup"><span data-stu-id="63988-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63988-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="63988-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63988-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="63988-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="63988-143">Java</span><span class="sxs-lookup"><span data-stu-id="63988-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="63988-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="63988-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="63988-145">Пример 2: обновление Деферупдате в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="63988-145">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="63988-146">В следующем примере показано, как обновить **деферупдате** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="63988-146">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="63988-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="63988-147">Request</span></span>

<span data-ttu-id="63988-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63988-148">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="63988-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="63988-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="63988-150">Пример 3: обновление Алловупдатеконфигуратионоверриде в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="63988-150">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="63988-151">В следующем примере показано, как обновить **алловупдатеконфигуратионоверриде** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="63988-151">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="63988-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="63988-152">Request</span></span>

<span data-ttu-id="63988-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63988-153">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="63988-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="63988-154">Response</span></span>

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
