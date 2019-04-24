---
title: Удаление educationClass
description: Удаление класса из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 462ba0700a3070c5f01eb8ce9b507a6a3617c177
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457679"
---
# <a name="remove-educationclass"></a><span data-ttu-id="4c1ee-103">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="4c1ee-103">Remove educationClass</span></span>

<span data-ttu-id="4c1ee-104">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="4c1ee-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c1ee-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c1ee-105">Permissions</span></span>
<span data-ttu-id="4c1ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c1ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c1ee-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c1ee-108">Permission type</span></span>      | <span data-ttu-id="4c1ee-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c1ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c1ee-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c1ee-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c1ee-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c1ee-111">Not supported.</span></span>  |
|<span data-ttu-id="4c1ee-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c1ee-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4c1ee-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c1ee-113">Not supported.</span></span>  |
|<span data-ttu-id="4c1ee-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c1ee-114">Application</span></span> | <span data-ttu-id="4c1ee-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c1ee-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4c1ee-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c1ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4c1ee-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c1ee-117">Request headers</span></span>
| <span data-ttu-id="4c1ee-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c1ee-118">Header</span></span>       | <span data-ttu-id="4c1ee-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4c1ee-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4c1ee-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c1ee-120">Authorization</span></span>  | <span data-ttu-id="4c1ee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c1ee-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c1ee-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c1ee-123">Request body</span></span>
<span data-ttu-id="4c1ee-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c1ee-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4c1ee-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c1ee-125">Response</span></span>
<span data-ttu-id="4c1ee-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="4c1ee-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c1ee-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4c1ee-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c1ee-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c1ee-128">Request</span></span>
<span data-ttu-id="4c1ee-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c1ee-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="4c1ee-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c1ee-130">Response</span></span>
<span data-ttu-id="4c1ee-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c1ee-131">The following is an example of the response.</span></span> 

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
