---
title: Создание privilegedApproval
description: Используйте этот API для создания нового Привилежедаппровал.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 05b8b7011f281ef371a49f0544c478f6736a8c1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455437"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="11b01-103">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="11b01-103">Create privilegedApproval</span></span>

<span data-ttu-id="11b01-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11b01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11b01-105">Используйте этот API для создания нового Привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="11b01-105">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="11b01-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11b01-106">Permissions</span></span>
<span data-ttu-id="11b01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11b01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="11b01-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11b01-109">Permission type</span></span>      | <span data-ttu-id="11b01-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11b01-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11b01-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11b01-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11b01-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11b01-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="11b01-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11b01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11b01-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b01-114">Not supported.</span></span>    |
|<span data-ttu-id="11b01-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11b01-115">Application</span></span> | <span data-ttu-id="11b01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b01-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11b01-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11b01-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="11b01-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11b01-118">Request headers</span></span>
| <span data-ttu-id="11b01-119">Имя</span><span class="sxs-lookup"><span data-stu-id="11b01-119">Name</span></span>       | <span data-ttu-id="11b01-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11b01-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11b01-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11b01-121">Authorization</span></span>  | <span data-ttu-id="11b01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11b01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11b01-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11b01-124">Request body</span></span>
<span data-ttu-id="11b01-125">В тексте запроса добавьте представление объекта [привилежедаппровал](../resources/privilegedapproval.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11b01-125">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="11b01-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b01-126">Response</span></span>

<span data-ttu-id="11b01-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11b01-127">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="11b01-128">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="11b01-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="11b01-129">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="11b01-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="11b01-130">Пример</span><span class="sxs-lookup"><span data-stu-id="11b01-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11b01-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b01-131">Request</span></span>
<span data-ttu-id="11b01-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11b01-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11b01-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="11b01-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="11b01-134">C#</span><span class="sxs-lookup"><span data-stu-id="11b01-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11b01-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11b01-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11b01-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11b01-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="11b01-137">В тексте запроса добавьте представление объекта [привилежедаппровал](../resources/privilegedapproval.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11b01-137">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="11b01-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b01-138">Response</span></span>
<span data-ttu-id="11b01-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11b01-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
