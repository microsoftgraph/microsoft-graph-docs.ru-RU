---
title: Удаление преподавателя
description: Удаление преподавателя для курса.
ms.openlocfilehash: d0ae11901bf8e8cd05dd7705acad09a6604180fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027792"
---
# <a name="remove-teacher"></a><span data-ttu-id="4f280-103">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="4f280-103">Remove teacher</span></span>

<span data-ttu-id="4f280-104">Удаление преподавателя для курса.</span><span class="sxs-lookup"><span data-stu-id="4f280-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f280-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f280-105">Permissions</span></span>
<span data-ttu-id="4f280-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f280-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f280-108">Permission type</span></span>      | <span data-ttu-id="4f280-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f280-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f280-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f280-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4f280-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f280-111">Not supported.</span></span>  |
|<span data-ttu-id="4f280-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f280-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4f280-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f280-113">Not supported.</span></span>  |
|<span data-ttu-id="4f280-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f280-114">Application</span></span> | <span data-ttu-id="4f280-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f280-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4f280-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f280-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4f280-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f280-117">Request headers</span></span>
| <span data-ttu-id="4f280-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f280-118">Header</span></span>       | <span data-ttu-id="4f280-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4f280-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f280-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f280-120">Authorization</span></span>  | <span data-ttu-id="4f280-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f280-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f280-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f280-123">Request body</span></span>
<span data-ttu-id="4f280-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f280-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4f280-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f280-125">Response</span></span>
<span data-ttu-id="4f280-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="4f280-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f280-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4f280-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f280-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f280-128">Request</span></span>
<span data-ttu-id="4f280-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f280-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/{teacher-id}
```

##### <a name="response"></a><span data-ttu-id="4f280-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f280-130">Response</span></span>
<span data-ttu-id="4f280-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4f280-131">The following is an example of the response.</span></span> 
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
