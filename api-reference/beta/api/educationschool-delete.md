---
title: Удаление educationSchool
description: Удаление учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4fb4735a60303e252d75a8a4cebb39d2f4c252a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950587"
---
# <a name="delete-educationschool"></a><span data-ttu-id="91a12-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="91a12-103">Delete educationSchool</span></span>

> <span data-ttu-id="91a12-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91a12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91a12-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91a12-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91a12-106">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="91a12-106">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="91a12-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91a12-107">Permissions</span></span>
<span data-ttu-id="91a12-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91a12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91a12-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91a12-110">Permission type</span></span>      | <span data-ttu-id="91a12-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91a12-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91a12-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91a12-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="91a12-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91a12-113">Not supported.</span></span>  |
|<span data-ttu-id="91a12-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91a12-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="91a12-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91a12-115">Not supported.</span></span>  |
|<span data-ttu-id="91a12-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91a12-116">Application</span></span> | <span data-ttu-id="91a12-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91a12-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="91a12-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91a12-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="91a12-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91a12-119">Request headers</span></span>
| <span data-ttu-id="91a12-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91a12-120">Header</span></span>       | <span data-ttu-id="91a12-121">Значение</span><span class="sxs-lookup"><span data-stu-id="91a12-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91a12-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91a12-122">Authorization</span></span>  | <span data-ttu-id="91a12-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91a12-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91a12-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91a12-125">Request body</span></span>
<span data-ttu-id="91a12-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91a12-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="91a12-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="91a12-127">Response</span></span>
<span data-ttu-id="91a12-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91a12-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91a12-130">Пример</span><span class="sxs-lookup"><span data-stu-id="91a12-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91a12-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="91a12-131">Request</span></span>
<span data-ttu-id="91a12-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91a12-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
##### <a name="response"></a><span data-ttu-id="91a12-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="91a12-133">Response</span></span>
<span data-ttu-id="91a12-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91a12-134">The following is an example of the response.</span></span> 

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
