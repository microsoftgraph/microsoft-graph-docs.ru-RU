---
title: Удаление educationClass
description: Удаление класса из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: ac626310fb61fd0d0a73e86d5c52ad0b37e1dd32
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866684"
---
# <a name="remove-educationclass"></a><span data-ttu-id="9164a-103">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="9164a-103">Remove educationClass</span></span>

> <span data-ttu-id="9164a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9164a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9164a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9164a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9164a-106">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="9164a-106">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="9164a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9164a-107">Permissions</span></span>
<span data-ttu-id="9164a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9164a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9164a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9164a-110">Permission type</span></span>      | <span data-ttu-id="9164a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9164a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9164a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9164a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="9164a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9164a-113">Not supported.</span></span>  |
|<span data-ttu-id="9164a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9164a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9164a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9164a-115">Not supported.</span></span>  |
|<span data-ttu-id="9164a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9164a-116">Application</span></span> | <span data-ttu-id="9164a-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9164a-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9164a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9164a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9164a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9164a-119">Request headers</span></span>
| <span data-ttu-id="9164a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9164a-120">Header</span></span>       | <span data-ttu-id="9164a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9164a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9164a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9164a-122">Authorization</span></span>  | <span data-ttu-id="9164a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9164a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9164a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9164a-125">Request body</span></span>
<span data-ttu-id="9164a-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9164a-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9164a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9164a-127">Response</span></span>
<span data-ttu-id="9164a-128">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="9164a-128">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="9164a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9164a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9164a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9164a-130">Request</span></span>
<span data-ttu-id="9164a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9164a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="9164a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="9164a-132">Response</span></span>
<span data-ttu-id="9164a-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9164a-133">The following is an example of the response.</span></span> 

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
