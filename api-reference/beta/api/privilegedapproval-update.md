---
title: Обновление privilegedapproval
description: Обновление свойств объекта privilegedapproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e2782b4756ece02695049c4327b651a1796c77c7
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787392"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="c9c6e-103">Обновление privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="c9c6e-103">Update privilegedapproval</span></span>

<span data-ttu-id="c9c6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9c6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9c6e-105">Обновление свойств объекта privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-105">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9c6e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9c6e-106">Permissions</span></span>
<span data-ttu-id="c9c6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9c6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c9c6e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9c6e-109">Permission type</span></span>      | <span data-ttu-id="c9c6e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9c6e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9c6e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9c6e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9c6e-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c9c6e-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c9c6e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9c6e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9c6e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-114">Not supported.</span></span>    |
|<span data-ttu-id="c9c6e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9c6e-115">Application</span></span> | <span data-ttu-id="c9c6e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9c6e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9c6e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c9c6e-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9c6e-118">Optional request headers</span></span>
| <span data-ttu-id="c9c6e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c9c6e-119">Name</span></span>       | <span data-ttu-id="c9c6e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c9c6e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c9c6e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9c6e-121">Authorization</span></span>  | <span data-ttu-id="c9c6e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9c6e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9c6e-124">Request body</span></span>
<span data-ttu-id="c9c6e-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c9c6e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9c6e-128">Property</span></span>     | <span data-ttu-id="c9c6e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c9c6e-129">Type</span></span>   |<span data-ttu-id="c9c6e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c9c6e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9c6e-131">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="c9c6e-131">approvalDuration</span></span>|<span data-ttu-id="c9c6e-132">Длительность</span><span class="sxs-lookup"><span data-stu-id="c9c6e-132">Duration</span></span>||
|<span data-ttu-id="c9c6e-133">approvalState</span><span class="sxs-lookup"><span data-stu-id="c9c6e-133">approvalState</span></span>|<span data-ttu-id="c9c6e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c9c6e-134">string</span></span>| <span data-ttu-id="c9c6e-135">Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-135">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="c9c6e-136">approvalType</span><span class="sxs-lookup"><span data-stu-id="c9c6e-136">approvalType</span></span>|<span data-ttu-id="c9c6e-137">String</span><span class="sxs-lookup"><span data-stu-id="c9c6e-137">String</span></span>||
|<span data-ttu-id="c9c6e-138">approverReason</span><span class="sxs-lookup"><span data-stu-id="c9c6e-138">approverReason</span></span>|<span data-ttu-id="c9c6e-139">String</span><span class="sxs-lookup"><span data-stu-id="c9c6e-139">String</span></span>||
|<span data-ttu-id="c9c6e-140">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c9c6e-140">endDateTime</span></span>|<span data-ttu-id="c9c6e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9c6e-141">DateTimeOffset</span></span>||
|<span data-ttu-id="c9c6e-142">requestorReason</span><span class="sxs-lookup"><span data-stu-id="c9c6e-142">requestorReason</span></span>|<span data-ttu-id="c9c6e-143">String</span><span class="sxs-lookup"><span data-stu-id="c9c6e-143">String</span></span>||
|<span data-ttu-id="c9c6e-144">roleId</span><span class="sxs-lookup"><span data-stu-id="c9c6e-144">roleId</span></span>|<span data-ttu-id="c9c6e-145">String</span><span class="sxs-lookup"><span data-stu-id="c9c6e-145">String</span></span>||
|<span data-ttu-id="c9c6e-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c9c6e-146">startDateTime</span></span>|<span data-ttu-id="c9c6e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9c6e-147">DateTimeOffset</span></span>||
|<span data-ttu-id="c9c6e-148">userId</span><span class="sxs-lookup"><span data-stu-id="c9c6e-148">userId</span></span>|<span data-ttu-id="c9c6e-149">String</span><span class="sxs-lookup"><span data-stu-id="c9c6e-149">String</span></span>||

## <a name="response"></a><span data-ttu-id="c9c6e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9c6e-150">Response</span></span>

<span data-ttu-id="c9c6e-151">В случае успешной работы этот метод возвращает `204 No Content` код ответа</span><span class="sxs-lookup"><span data-stu-id="c9c6e-151">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="c9c6e-152">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c9c6e-153">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="c9c6e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="c9c6e-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9c6e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9c6e-155">Request</span></span>
<span data-ttu-id="c9c6e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9c6e-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9c6e-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval/{requestId}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c9c6e-158">C#</span><span class="sxs-lookup"><span data-stu-id="c9c6e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9c6e-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9c6e-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9c6e-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9c6e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9c6e-161">Java</span><span class="sxs-lookup"><span data-stu-id="c9c6e-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c9c6e-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9c6e-162">Response</span></span>
<span data-ttu-id="c9c6e-p105">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c9c6e-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


