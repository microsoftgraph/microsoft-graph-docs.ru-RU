---
title: Создание проверки подлинностиContextClassReference
description: Создание новой проверки подлинностиContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4646e8a388800587c0aa73a736d591dc6b97c6fb
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663958"
---
# <a name="create-authenticationcontextclassreference"></a><span data-ttu-id="25ed4-103">Создание проверки подлинностиContextClassReference</span><span class="sxs-lookup"><span data-stu-id="25ed4-103">Create authenticationContextClassReference</span></span>

<span data-ttu-id="25ed4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25ed4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25ed4-105">Создание новой [проверки подлинностиContextClassReference](../resources/authenticationContextClassReference.md).</span><span class="sxs-lookup"><span data-stu-id="25ed4-105">Create a new [authenticationContextClassReference](../resources/authenticationContextClassReference.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="25ed4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25ed4-106">Permissions</span></span>

<span data-ttu-id="25ed4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25ed4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25ed4-109">Permission type</span></span>                        | <span data-ttu-id="25ed4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25ed4-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="25ed4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25ed4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="25ed4-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="25ed4-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="25ed4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25ed4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25ed4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25ed4-114">Not supported.</span></span> |
|<span data-ttu-id="25ed4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="25ed4-115">Application</span></span>                            | <span data-ttu-id="25ed4-116">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="25ed4-116">Policy.ReadWrite.ConditionalAccess</span></span> |

> [!NOTE]
> <span data-ttu-id="25ed4-117">Этот API имеет [известные проблемы, связанные](/graph/known-issues#permissions) с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="25ed4-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="25ed4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25ed4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/authenticationContextClassReferences
```

## <a name="request-headers"></a><span data-ttu-id="25ed4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25ed4-119">Request headers</span></span>

| <span data-ttu-id="25ed4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="25ed4-120">Name</span></span>          | <span data-ttu-id="25ed4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="25ed4-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="25ed4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25ed4-122">Authorization</span></span> | <span data-ttu-id="25ed4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25ed4-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="25ed4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25ed4-125">Content-Type</span></span>  | <span data-ttu-id="25ed4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25ed4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25ed4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25ed4-128">Request body</span></span>

<span data-ttu-id="25ed4-129">В тексте запроса поставляем представление JSON объекта [authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="25ed4-129">In the request body, supply a JSON representation of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="25ed4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="25ed4-130">Response</span></span>

<span data-ttu-id="25ed4-131">В случае успешной работы этот метод возвращает код ответа и новый объект `201 Created` [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="25ed4-131">If successful, this method returns a `201 Created` response code and a new [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25ed4-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="25ed4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25ed4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="25ed4-133">Request</span></span>
<span data-ttu-id="25ed4-134">В следующем примере показано создание новой проверки подлинности, которая доступна приложениям для использования.</span><span class="sxs-lookup"><span data-stu-id="25ed4-134">The following example shows creating a new authenticationcontextclassreference that is available for apps to use.</span></span>




# <a name="http"></a>[<span data-ttu-id="25ed4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="25ed4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_authenticationcontextclassreference"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
Content-type: application/json

{
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```
# <a name="c"></a>[<span data-ttu-id="25ed4-136">C#</span><span class="sxs-lookup"><span data-stu-id="25ed4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-authenticationcontextclassreference-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25ed4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25ed4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-authenticationcontextclassreference-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25ed4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25ed4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-authenticationcontextclassreference-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25ed4-139">Java</span><span class="sxs-lookup"><span data-stu-id="25ed4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-authenticationcontextclassreference-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="25ed4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="25ed4-140">Response</span></span>

<span data-ttu-id="25ed4-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="25ed4-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReference/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
