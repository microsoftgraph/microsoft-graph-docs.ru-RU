---
title: Удаление administrativeUnit
description: Удаление administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6978c3046c9652068021141d0b5ec9aef5c8e8d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319036"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="9229b-103">Удаление administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="9229b-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9229b-104">Удаление [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="9229b-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9229b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9229b-105">Permissions</span></span>
<span data-ttu-id="9229b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9229b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9229b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9229b-108">Permission type</span></span>      | <span data-ttu-id="9229b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9229b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9229b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9229b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9229b-111">AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="9229b-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9229b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9229b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9229b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9229b-113">Not supported.</span></span>    |
|<span data-ttu-id="9229b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9229b-114">Application</span></span> | <span data-ttu-id="9229b-115">AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9229b-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9229b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9229b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9229b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9229b-117">Request headers</span></span>
| <span data-ttu-id="9229b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9229b-118">Name</span></span>       | <span data-ttu-id="9229b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9229b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9229b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9229b-120">Authorization</span></span>  | <span data-ttu-id="9229b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9229b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9229b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9229b-123">Request body</span></span>
<span data-ttu-id="9229b-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9229b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9229b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="9229b-125">Response</span></span>

<span data-ttu-id="9229b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9229b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9229b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="9229b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9229b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9229b-129">Request</span></span>
<span data-ttu-id="9229b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9229b-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9229b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9229b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9229b-132">C#</span><span class="sxs-lookup"><span data-stu-id="9229b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9229b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9229b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9229b-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9229b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9229b-135">Java</span><span class="sxs-lookup"><span data-stu-id="9229b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9229b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9229b-136">Response</span></span>
<span data-ttu-id="9229b-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9229b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
