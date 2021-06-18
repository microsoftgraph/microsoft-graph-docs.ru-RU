---
title: Удаление educationRubric
description: Удаление объекта educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 15d455e665026c3e0c86f7ef162a5602772d84aa
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991194"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="8066f-103">Удаление educationRubric</span><span class="sxs-lookup"><span data-stu-id="8066f-103">Delete educationRubric</span></span>

<span data-ttu-id="8066f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8066f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8066f-105">Удаление [объекта educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="8066f-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8066f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8066f-106">Permissions</span></span>

<span data-ttu-id="8066f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8066f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8066f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8066f-109">Permission type</span></span>                        | <span data-ttu-id="8066f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8066f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8066f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8066f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8066f-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8066f-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8066f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8066f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8066f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8066f-114">Not supported.</span></span> |
| <span data-ttu-id="8066f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8066f-115">Application</span></span>                            | <span data-ttu-id="8066f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8066f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8066f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8066f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

## <a name="request-headers"></a><span data-ttu-id="8066f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8066f-118">Request headers</span></span>

| <span data-ttu-id="8066f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8066f-119">Name</span></span>          | <span data-ttu-id="8066f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8066f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8066f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8066f-121">Authorization</span></span> | <span data-ttu-id="8066f-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8066f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8066f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8066f-123">Request body</span></span>

<span data-ttu-id="8066f-124">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8066f-124">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8066f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8066f-125">Response</span></span>

<span data-ttu-id="8066f-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8066f-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8066f-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8066f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8066f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8066f-129">Request</span></span>

<span data-ttu-id="8066f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8066f-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8066f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8066f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```
# <a name="c"></a>[<span data-ttu-id="8066f-132">C#</span><span class="sxs-lookup"><span data-stu-id="8066f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8066f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8066f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8066f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8066f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8066f-135">Java</span><span class="sxs-lookup"><span data-stu-id="8066f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationrubric-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8066f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8066f-136">Response</span></span>

<span data-ttu-id="8066f-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8066f-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


