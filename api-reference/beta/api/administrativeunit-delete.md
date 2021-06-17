---
title: Удаление administrativeUnit
description: Удаление администратораUnit.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6b9f2c9813e56475280109ad8fd66ee4680ea663
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992053"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="bd513-103">Удаление administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="bd513-103">Delete administrativeUnit</span></span>

<span data-ttu-id="bd513-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd513-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd513-105">Удаление [администратораUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="bd513-105">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd513-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd513-106">Permissions</span></span>
<span data-ttu-id="bd513-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bd513-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd513-109">Permission type</span></span>      | <span data-ttu-id="bd513-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd513-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd513-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd513-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bd513-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd513-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bd513-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd513-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd513-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd513-114">Not supported.</span></span>    |
|<span data-ttu-id="bd513-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="bd513-115">Application</span></span> | <span data-ttu-id="bd513-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd513-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd513-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd513-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="bd513-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd513-118">Request headers</span></span>
| <span data-ttu-id="bd513-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bd513-119">Name</span></span>       | <span data-ttu-id="bd513-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bd513-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bd513-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd513-121">Authorization</span></span>  | <span data-ttu-id="bd513-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd513-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd513-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd513-124">Request body</span></span>
<span data-ttu-id="bd513-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd513-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd513-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd513-126">Response</span></span>

<span data-ttu-id="bd513-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bd513-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd513-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bd513-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd513-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd513-130">Request</span></span>
<span data-ttu-id="bd513-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd513-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd513-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd513-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="bd513-133">C#</span><span class="sxs-lookup"><span data-stu-id="bd513-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd513-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd513-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd513-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd513-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd513-136">Java</span><span class="sxs-lookup"><span data-stu-id="bd513-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bd513-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd513-137">Response</span></span>
<span data-ttu-id="bd513-p104">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd513-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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


