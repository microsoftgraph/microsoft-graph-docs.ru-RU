---
title: Создание privilegedApproval
description: Используйте этот API для создания нового Привилежедаппровал.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 271590a1526fca37a385471a0efcdbb2956b341f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412847"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="baf85-103">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="baf85-103">Create privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baf85-104">Используйте этот API для создания нового Привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="baf85-104">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="baf85-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="baf85-105">Permissions</span></span>
<span data-ttu-id="baf85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baf85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="baf85-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="baf85-108">Permission type</span></span>      | <span data-ttu-id="baf85-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="baf85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baf85-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="baf85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="baf85-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="baf85-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="baf85-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="baf85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baf85-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baf85-113">Not supported.</span></span>    |
|<span data-ttu-id="baf85-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="baf85-114">Application</span></span> | <span data-ttu-id="baf85-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baf85-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="baf85-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="baf85-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="baf85-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="baf85-117">Request headers</span></span>
| <span data-ttu-id="baf85-118">Имя</span><span class="sxs-lookup"><span data-stu-id="baf85-118">Name</span></span>       | <span data-ttu-id="baf85-119">Описание</span><span class="sxs-lookup"><span data-stu-id="baf85-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="baf85-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="baf85-120">Authorization</span></span>  | <span data-ttu-id="baf85-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baf85-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="baf85-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="baf85-123">Request body</span></span>
<span data-ttu-id="baf85-124">В тексте запроса добавьте представление объекта [привилежедаппровал](../resources/privilegedapproval.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baf85-124">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="baf85-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="baf85-125">Response</span></span>

<span data-ttu-id="baf85-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="baf85-126">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="baf85-127">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="baf85-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="baf85-128">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="baf85-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="baf85-129">Пример</span><span class="sxs-lookup"><span data-stu-id="baf85-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="baf85-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="baf85-130">Request</span></span>
<span data-ttu-id="baf85-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="baf85-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="baf85-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="baf85-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="baf85-133">C#</span><span class="sxs-lookup"><span data-stu-id="baf85-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="baf85-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="baf85-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="baf85-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="baf85-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="baf85-136">В тексте запроса добавьте представление объекта [привилежедаппровал](../resources/privilegedapproval.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baf85-136">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="baf85-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="baf85-137">Response</span></span>
<span data-ttu-id="baf85-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="baf85-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
