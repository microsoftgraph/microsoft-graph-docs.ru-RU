---
title: Удаление преподавателя
description: Удаление преподавателя для курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7fb693091cc0907b6eeb8ec293fea2bafbfa4295
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006873"
---
# <a name="remove-teacher"></a><span data-ttu-id="36f65-103">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="36f65-103">Remove teacher</span></span>

<span data-ttu-id="36f65-104">Удаление преподавателя для курса.</span><span class="sxs-lookup"><span data-stu-id="36f65-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="36f65-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36f65-105">Permissions</span></span>
<span data-ttu-id="36f65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36f65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36f65-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36f65-108">Permission type</span></span>      | <span data-ttu-id="36f65-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36f65-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36f65-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36f65-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="36f65-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36f65-111">Not supported.</span></span>  |
|<span data-ttu-id="36f65-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36f65-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="36f65-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36f65-113">Not supported.</span></span>  |
|<span data-ttu-id="36f65-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36f65-114">Application</span></span> | <span data-ttu-id="36f65-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f65-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36f65-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36f65-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="36f65-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36f65-117">Request headers</span></span>
| <span data-ttu-id="36f65-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36f65-118">Header</span></span>       | <span data-ttu-id="36f65-119">Значение</span><span class="sxs-lookup"><span data-stu-id="36f65-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36f65-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36f65-120">Authorization</span></span>  | <span data-ttu-id="36f65-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36f65-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36f65-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36f65-123">Request body</span></span>
<span data-ttu-id="36f65-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36f65-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="36f65-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="36f65-125">Response</span></span>
<span data-ttu-id="36f65-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="36f65-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="36f65-127">Пример</span><span class="sxs-lookup"><span data-stu-id="36f65-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36f65-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="36f65-128">Request</span></span>
<span data-ttu-id="36f65-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36f65-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/{teacher-id}
```

##### <a name="response"></a><span data-ttu-id="36f65-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="36f65-130">Response</span></span>
<span data-ttu-id="36f65-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36f65-131">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
