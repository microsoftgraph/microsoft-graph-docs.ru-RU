---
title: Удаление educationSchool
description: Удаление учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bb865ef12d0ad8eb0f18b5f9c7c9631346921e17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923847"
---
# <a name="delete-educationschool"></a><span data-ttu-id="f7e74-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="f7e74-103">Delete educationSchool</span></span>

<span data-ttu-id="f7e74-104">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f7e74-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7e74-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e74-105">Permissions</span></span>
<span data-ttu-id="f7e74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7e74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e74-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e74-108">Permission type</span></span>      | <span data-ttu-id="f7e74-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7e74-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7e74-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7e74-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f7e74-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e74-111">Not supported.</span></span>  |
|<span data-ttu-id="f7e74-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7e74-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f7e74-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e74-113">Not supported.</span></span>  |
|<span data-ttu-id="f7e74-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7e74-114">Application</span></span> | <span data-ttu-id="f7e74-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e74-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f7e74-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7e74-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f7e74-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7e74-117">Request headers</span></span>
| <span data-ttu-id="f7e74-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7e74-118">Header</span></span>       | <span data-ttu-id="f7e74-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f7e74-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7e74-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7e74-120">Authorization</span></span>  | <span data-ttu-id="f7e74-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7e74-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7e74-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7e74-123">Request body</span></span>
<span data-ttu-id="f7e74-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7e74-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f7e74-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e74-125">Response</span></span>
<span data-ttu-id="f7e74-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e74-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e74-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f7e74-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7e74-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7e74-129">Request</span></span>
<span data-ttu-id="f7e74-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7e74-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="f7e74-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7e74-131">Response</span></span>
<span data-ttu-id="f7e74-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f7e74-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
