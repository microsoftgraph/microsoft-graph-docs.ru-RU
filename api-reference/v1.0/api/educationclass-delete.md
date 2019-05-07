---
title: Удаление educationClass
description: Удаление класса. Так как класс также является универсальной группой, удаление класса приводит к удалению группы.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1e12201386ab3e14155f04f4408c364334e0b0d5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616077"
---
# <a name="delete-educationclass"></a><span data-ttu-id="68e6a-104">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="68e6a-104">Delete educationClass</span></span>

<span data-ttu-id="68e6a-105">Удаление класса.</span><span class="sxs-lookup"><span data-stu-id="68e6a-105">Delete a class.</span></span> <span data-ttu-id="68e6a-106">Так как класс также является универсальной группой, удаление класса приводит к удалению группы.</span><span class="sxs-lookup"><span data-stu-id="68e6a-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="68e6a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68e6a-107">Permissions</span></span>
<span data-ttu-id="68e6a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68e6a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e6a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68e6a-110">Permission type</span></span>      | <span data-ttu-id="68e6a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68e6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68e6a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68e6a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="68e6a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68e6a-113">Not supported.</span></span>  |
|<span data-ttu-id="68e6a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68e6a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="68e6a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68e6a-115">Not supported.</span></span>  |
|<span data-ttu-id="68e6a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68e6a-116">Application</span></span> | <span data-ttu-id="68e6a-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68e6a-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="68e6a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68e6a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="68e6a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68e6a-119">Request headers</span></span>
| <span data-ttu-id="68e6a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68e6a-120">Header</span></span>       | <span data-ttu-id="68e6a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="68e6a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68e6a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68e6a-122">Authorization</span></span>  | <span data-ttu-id="68e6a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68e6a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68e6a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68e6a-125">Request body</span></span>
<span data-ttu-id="68e6a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68e6a-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="68e6a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="68e6a-127">Response</span></span>
<span data-ttu-id="68e6a-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="68e6a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68e6a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="68e6a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68e6a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="68e6a-131">Request</span></span>
<span data-ttu-id="68e6a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68e6a-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="68e6a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="68e6a-133">Response</span></span>
<span data-ttu-id="68e6a-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68e6a-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="68e6a-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="68e6a-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="68e6a-136">Языках</span><span class="sxs-lookup"><span data-stu-id="68e6a-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationclass-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68e6a-137">Язык</span><span class="sxs-lookup"><span data-stu-id="68e6a-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationclass-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
