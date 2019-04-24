---
title: Удаление преподавателя
description: Удаление преподавателя для курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bf6860e515d1b8e1fa52b633b88740e62c6992e4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457937"
---
# <a name="remove-teacher"></a><span data-ttu-id="6d024-103">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="6d024-103">Remove teacher</span></span>

<span data-ttu-id="6d024-104">Удаление преподавателя для курса.</span><span class="sxs-lookup"><span data-stu-id="6d024-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d024-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d024-105">Permissions</span></span>
<span data-ttu-id="6d024-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d024-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d024-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d024-108">Permission type</span></span>      | <span data-ttu-id="6d024-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d024-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d024-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d024-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6d024-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d024-111">Not supported.</span></span>  |
|<span data-ttu-id="6d024-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d024-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6d024-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d024-113">Not supported.</span></span>  |
|<span data-ttu-id="6d024-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d024-114">Application</span></span> | <span data-ttu-id="6d024-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d024-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6d024-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d024-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6d024-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d024-117">Request headers</span></span>
| <span data-ttu-id="6d024-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d024-118">Header</span></span>       | <span data-ttu-id="6d024-119">Значение</span><span class="sxs-lookup"><span data-stu-id="6d024-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d024-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d024-120">Authorization</span></span>  | <span data-ttu-id="6d024-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d024-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d024-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d024-123">Request body</span></span>
<span data-ttu-id="6d024-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d024-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6d024-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d024-125">Response</span></span>
<span data-ttu-id="6d024-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="6d024-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d024-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6d024-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d024-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d024-128">Request</span></span>
<span data-ttu-id="6d024-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d024-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/{teacher-id}
```

##### <a name="response"></a><span data-ttu-id="6d024-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d024-130">Response</span></span>
<span data-ttu-id="6d024-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6d024-131">The following is an example of the response.</span></span> 
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
