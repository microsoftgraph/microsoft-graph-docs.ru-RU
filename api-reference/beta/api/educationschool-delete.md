---
title: Удаление educationSchool
description: Удаление учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bdf1d3faa41e12ee911796d36c6da76fc4b0f753
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324937"
---
# <a name="delete-educationschool"></a><span data-ttu-id="fd1ab-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="fd1ab-103">Delete educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd1ab-104">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="fd1ab-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd1ab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd1ab-105">Permissions</span></span>
<span data-ttu-id="fd1ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd1ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd1ab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd1ab-108">Permission type</span></span>      | <span data-ttu-id="fd1ab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd1ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd1ab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd1ab-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fd1ab-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd1ab-111">Not supported.</span></span>  |
|<span data-ttu-id="fd1ab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd1ab-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fd1ab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd1ab-113">Not supported.</span></span>  |
|<span data-ttu-id="fd1ab-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="fd1ab-114">Application</span></span> | <span data-ttu-id="fd1ab-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd1ab-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fd1ab-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd1ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fd1ab-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd1ab-117">Request headers</span></span>
| <span data-ttu-id="fd1ab-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd1ab-118">Header</span></span>       | <span data-ttu-id="fd1ab-119">Значение</span><span class="sxs-lookup"><span data-stu-id="fd1ab-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd1ab-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd1ab-120">Authorization</span></span>  | <span data-ttu-id="fd1ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd1ab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd1ab-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd1ab-123">Request body</span></span>
<span data-ttu-id="fd1ab-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd1ab-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fd1ab-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd1ab-125">Response</span></span>
<span data-ttu-id="fd1ab-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd1ab-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd1ab-128">Пример</span><span class="sxs-lookup"><span data-stu-id="fd1ab-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd1ab-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd1ab-129">Request</span></span>
<span data-ttu-id="fd1ab-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd1ab-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
##### <a name="response"></a><span data-ttu-id="fd1ab-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd1ab-131">Response</span></span>
<span data-ttu-id="fd1ab-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd1ab-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
