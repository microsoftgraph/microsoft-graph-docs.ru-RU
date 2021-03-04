---
title: Создание privilegedApproval
description: Используйте этот API для создания нового привилегированногоApproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: ef3581fef523f14d5f84bb0f1859795860624c45
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442245"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="a54e9-103">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="a54e9-103">Create privilegedApproval</span></span>

<span data-ttu-id="a54e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a54e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a54e9-105">Используйте этот API для создания нового привилегированногоApproval.</span><span class="sxs-lookup"><span data-stu-id="a54e9-105">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="a54e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a54e9-106">Permissions</span></span>
<span data-ttu-id="a54e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a54e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a54e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a54e9-109">Permission type</span></span>      | <span data-ttu-id="a54e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a54e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a54e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a54e9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a54e9-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a54e9-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a54e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a54e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a54e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a54e9-114">Not supported.</span></span>    |
|<span data-ttu-id="a54e9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a54e9-115">Application</span></span> | <span data-ttu-id="a54e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a54e9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a54e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a54e9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="a54e9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a54e9-118">Request headers</span></span>
| <span data-ttu-id="a54e9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a54e9-119">Name</span></span>       | <span data-ttu-id="a54e9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a54e9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a54e9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a54e9-121">Authorization</span></span>  | <span data-ttu-id="a54e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a54e9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a54e9-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a54e9-124">Request body</span></span>
<span data-ttu-id="a54e9-125">В теле запроса поставляем представление JSON объекта [privilegedApproval.](../resources/privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="a54e9-125">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a54e9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a54e9-126">Response</span></span>

<span data-ttu-id="a54e9-127">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект privilegedApproval](../resources/privilegedapproval.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a54e9-127">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="a54e9-128">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="a54e9-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a54e9-129">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="a54e9-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="a54e9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a54e9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a54e9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a54e9-131">Request</span></span>
<span data-ttu-id="a54e9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a54e9-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a54e9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a54e9-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a54e9-134">C#</span><span class="sxs-lookup"><span data-stu-id="a54e9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a54e9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a54e9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a54e9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a54e9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a54e9-137">Java</span><span class="sxs-lookup"><span data-stu-id="a54e9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedapproval-from-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a54e9-138">В теле запроса поставляем представление JSON объекта [privilegedApproval.](../resources/privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="a54e9-138">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a54e9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a54e9-139">Response</span></span>
<span data-ttu-id="a54e9-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a54e9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


