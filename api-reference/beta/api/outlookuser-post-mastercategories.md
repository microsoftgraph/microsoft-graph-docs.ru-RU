---
title: Создание категории Outlook
description: Создание объекта outlookCategory в основном списке категорий пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9a0b13fdac001a168d2d43ea6e70e2c3651c0c47
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038021"
---
# <a name="create-outlook-category"></a><span data-ttu-id="321af-103">Создание категории Outlook</span><span class="sxs-lookup"><span data-stu-id="321af-103">Create Outlook category</span></span>

<span data-ttu-id="321af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="321af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="321af-105">Создание объекта [outlookCategory](../resources/outlookcategory.md) в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="321af-105">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="321af-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="321af-106">Permissions</span></span>
<span data-ttu-id="321af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="321af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="321af-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="321af-109">Permission type</span></span>      | <span data-ttu-id="321af-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="321af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="321af-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="321af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="321af-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="321af-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="321af-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="321af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="321af-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="321af-114">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="321af-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="321af-115">Application</span></span> | <span data-ttu-id="321af-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="321af-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="321af-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="321af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="321af-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="321af-118">Request headers</span></span>
| <span data-ttu-id="321af-119">Имя</span><span class="sxs-lookup"><span data-stu-id="321af-119">Name</span></span>       | <span data-ttu-id="321af-120">Описание</span><span class="sxs-lookup"><span data-stu-id="321af-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="321af-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="321af-121">Authorization</span></span>  | <span data-ttu-id="321af-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="321af-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="321af-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="321af-124">Request body</span></span>
<span data-ttu-id="321af-125">Включите в текст запроса описание объекта [outlookCategory](../resources/outlookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="321af-125">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="321af-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="321af-126">Response</span></span>

<span data-ttu-id="321af-127">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и новый объект [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="321af-127">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="321af-128">Пример</span><span class="sxs-lookup"><span data-stu-id="321af-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="321af-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="321af-129">Request</span></span>
<span data-ttu-id="321af-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="321af-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="321af-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="321af-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
# <a name="c"></a>[<span data-ttu-id="321af-132">C#</span><span class="sxs-lookup"><span data-stu-id="321af-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlookcategory-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="321af-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="321af-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlookcategory-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="321af-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="321af-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlookcategory-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="321af-135">Java</span><span class="sxs-lookup"><span data-stu-id="321af-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlookcategory-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="321af-136">Включите в текст запроса описание объекта [outlookCategory](../resources/outlookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="321af-136">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="321af-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="321af-137">Response</span></span>
<span data-ttu-id="321af-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="321af-138">Here is an example of the response.</span></span> <span data-ttu-id="321af-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="321af-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


