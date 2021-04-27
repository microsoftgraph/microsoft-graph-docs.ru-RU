---
title: Создание privilegedApproval
description: Используйте этот API для создания нового привилегированногоApproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 3b85324bc8468f0fd6c3c5963ab417ba8c6a9acb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055290"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="beffc-103">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="beffc-103">Create privilegedApproval</span></span>

<span data-ttu-id="beffc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beffc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beffc-105">Используйте этот API для создания нового привилегированногоApproval.</span><span class="sxs-lookup"><span data-stu-id="beffc-105">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="beffc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="beffc-106">Permissions</span></span>
<span data-ttu-id="beffc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="beffc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beffc-109">Permission type</span></span>      | <span data-ttu-id="beffc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="beffc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beffc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beffc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="beffc-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="beffc-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="beffc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beffc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beffc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beffc-114">Not supported.</span></span>    |
|<span data-ttu-id="beffc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="beffc-115">Application</span></span> | <span data-ttu-id="beffc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beffc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="beffc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beffc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="beffc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beffc-118">Request headers</span></span>
| <span data-ttu-id="beffc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="beffc-119">Name</span></span>       | <span data-ttu-id="beffc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="beffc-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="beffc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="beffc-121">Authorization</span></span>  | <span data-ttu-id="beffc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beffc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="beffc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beffc-124">Request body</span></span>
<span data-ttu-id="beffc-125">В теле запроса поставляем представление JSON объекта [privilegedApproval.](../resources/privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="beffc-125">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="beffc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="beffc-126">Response</span></span>

<span data-ttu-id="beffc-127">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект privilegedApproval](../resources/privilegedapproval.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="beffc-127">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="beffc-128">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="beffc-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="beffc-129">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="beffc-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="beffc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="beffc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="beffc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="beffc-131">Request</span></span>
<span data-ttu-id="beffc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beffc-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="beffc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="beffc-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="beffc-134">C#</span><span class="sxs-lookup"><span data-stu-id="beffc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="beffc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="beffc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="beffc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="beffc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="beffc-137">Java</span><span class="sxs-lookup"><span data-stu-id="beffc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedapproval-from-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="beffc-138">В теле запроса поставляем представление JSON объекта [privilegedApproval.](../resources/privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="beffc-138">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="beffc-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="beffc-139">Response</span></span>
<span data-ttu-id="beffc-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="beffc-140">Here is an example of the response.</span></span> <span data-ttu-id="beffc-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="beffc-141">Note: The response object shown here might be shortened for readability.</span></span>
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


