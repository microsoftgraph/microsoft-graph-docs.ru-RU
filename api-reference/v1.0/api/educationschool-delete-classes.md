---
title: Удаление educationClass
description: Удаление класса из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1a0deef07b733153b939eba13b5d0987b106208a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002904"
---
# <a name="remove-educationclass"></a><span data-ttu-id="4a76a-103">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="4a76a-103">Remove educationClass</span></span>

<span data-ttu-id="4a76a-104">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="4a76a-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a76a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a76a-105">Permissions</span></span>
<span data-ttu-id="4a76a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a76a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a76a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a76a-108">Permission type</span></span>      | <span data-ttu-id="4a76a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a76a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a76a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a76a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4a76a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a76a-111">Not supported.</span></span>  |
|<span data-ttu-id="4a76a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a76a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4a76a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a76a-113">Not supported.</span></span>  |
|<span data-ttu-id="4a76a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a76a-114">Application</span></span> | <span data-ttu-id="4a76a-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a76a-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4a76a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a76a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4a76a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a76a-117">Request headers</span></span>
| <span data-ttu-id="4a76a-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a76a-118">Header</span></span>       | <span data-ttu-id="4a76a-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4a76a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a76a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a76a-120">Authorization</span></span>  | <span data-ttu-id="4a76a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a76a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a76a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a76a-123">Request body</span></span>
<span data-ttu-id="4a76a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a76a-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4a76a-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a76a-125">Response</span></span>
<span data-ttu-id="4a76a-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="4a76a-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a76a-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4a76a-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a76a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a76a-128">Request</span></span>
<span data-ttu-id="4a76a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a76a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="4a76a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a76a-130">Response</span></span>
<span data-ttu-id="4a76a-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4a76a-131">The following is an example of the response.</span></span> 

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
