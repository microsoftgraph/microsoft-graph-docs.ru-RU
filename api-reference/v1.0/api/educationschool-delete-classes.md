---
title: Удаление educationClass
description: Удаление класса из учебного заведения.
author: mmast-msft
ms.openlocfilehash: 6f917946e0fc24a34c5560e5b01a2bd4acca030d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331579"
---
# <a name="remove-educationclass"></a><span data-ttu-id="3b186-103">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="3b186-103">Remove educationClass</span></span>

<span data-ttu-id="3b186-104">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="3b186-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b186-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b186-105">Permissions</span></span>
<span data-ttu-id="3b186-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b186-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b186-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b186-108">Permission type</span></span>      | <span data-ttu-id="3b186-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b186-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b186-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b186-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3b186-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b186-111">Not supported.</span></span>  |
|<span data-ttu-id="3b186-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b186-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3b186-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b186-113">Not supported.</span></span>  |
|<span data-ttu-id="3b186-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b186-114">Application</span></span> | <span data-ttu-id="3b186-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b186-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3b186-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b186-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="3b186-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b186-117">Request headers</span></span>
| <span data-ttu-id="3b186-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b186-118">Header</span></span>       | <span data-ttu-id="3b186-119">Значение</span><span class="sxs-lookup"><span data-stu-id="3b186-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b186-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b186-120">Authorization</span></span>  | <span data-ttu-id="3b186-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b186-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b186-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b186-123">Request body</span></span>
<span data-ttu-id="3b186-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b186-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3b186-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b186-125">Response</span></span>
<span data-ttu-id="3b186-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="3b186-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b186-127">Пример</span><span class="sxs-lookup"><span data-stu-id="3b186-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b186-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b186-128">Request</span></span>
<span data-ttu-id="3b186-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b186-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="3b186-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b186-130">Response</span></span>
<span data-ttu-id="3b186-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3b186-131">The following is an example of the response.</span></span> 

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