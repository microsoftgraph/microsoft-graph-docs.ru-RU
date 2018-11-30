---
title: Удаление educationSchool
description: Удаление учебного заведения.
ms.openlocfilehash: 48516780c0132012b8b7f2d8aa9295af7ade0711
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027782"
---
# <a name="delete-educationschool"></a><span data-ttu-id="63a58-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="63a58-103">Delete educationSchool</span></span>

<span data-ttu-id="63a58-104">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="63a58-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="63a58-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63a58-105">Permissions</span></span>
<span data-ttu-id="63a58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63a58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63a58-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63a58-108">Permission type</span></span>      | <span data-ttu-id="63a58-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63a58-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63a58-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63a58-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="63a58-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63a58-111">Not supported.</span></span>  |
|<span data-ttu-id="63a58-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63a58-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="63a58-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63a58-113">Not supported.</span></span>  |
|<span data-ttu-id="63a58-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63a58-114">Application</span></span> | <span data-ttu-id="63a58-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a58-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="63a58-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63a58-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="63a58-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63a58-117">Request headers</span></span>
| <span data-ttu-id="63a58-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63a58-118">Header</span></span>       | <span data-ttu-id="63a58-119">Значение</span><span class="sxs-lookup"><span data-stu-id="63a58-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63a58-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63a58-120">Authorization</span></span>  | <span data-ttu-id="63a58-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63a58-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63a58-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63a58-123">Request body</span></span>
<span data-ttu-id="63a58-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63a58-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="63a58-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="63a58-125">Response</span></span>
<span data-ttu-id="63a58-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63a58-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63a58-128">Пример</span><span class="sxs-lookup"><span data-stu-id="63a58-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63a58-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="63a58-129">Request</span></span>
<span data-ttu-id="63a58-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63a58-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="63a58-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="63a58-131">Response</span></span>
<span data-ttu-id="63a58-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="63a58-132">The following is an example of the response.</span></span> 

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