---
title: Удаление educationUser
description: Удаление пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: edc9272d8b31804b170424a27123ca66b4611e28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464763"
---
# <a name="delete-educationuser"></a><span data-ttu-id="aa04d-103">Удаление educationUser</span><span class="sxs-lookup"><span data-stu-id="aa04d-103">Delete educationUser</span></span>

<span data-ttu-id="aa04d-104">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa04d-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="aa04d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa04d-105">Permissions</span></span>
<span data-ttu-id="aa04d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa04d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa04d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa04d-108">Permission type</span></span>      | <span data-ttu-id="aa04d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa04d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa04d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa04d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="aa04d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa04d-111">Not supported.</span></span>  |
|<span data-ttu-id="aa04d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa04d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="aa04d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa04d-113">Not supported.</span></span>  |
|<span data-ttu-id="aa04d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa04d-114">Application</span></span> | <span data-ttu-id="aa04d-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa04d-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa04d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa04d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="aa04d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa04d-117">Request headers</span></span>
| <span data-ttu-id="aa04d-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa04d-118">Header</span></span>       | <span data-ttu-id="aa04d-119">Значение</span><span class="sxs-lookup"><span data-stu-id="aa04d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa04d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa04d-120">Authorization</span></span>  | <span data-ttu-id="aa04d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa04d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa04d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa04d-123">Request body</span></span>
<span data-ttu-id="aa04d-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa04d-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="aa04d-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa04d-125">Response</span></span>
<span data-ttu-id="aa04d-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aa04d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa04d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="aa04d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa04d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa04d-129">Request</span></span>
<span data-ttu-id="aa04d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa04d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="aa04d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa04d-131">Response</span></span>
<span data-ttu-id="aa04d-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aa04d-132">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
