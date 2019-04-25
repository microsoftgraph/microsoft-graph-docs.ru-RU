---
title: Удаление educationUser
description: Удаление пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: be2839a866474acbdd196c3b43503a5b69252c26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549987"
---
# <a name="delete-educationuser"></a><span data-ttu-id="decb0-103">Удаление educationUser</span><span class="sxs-lookup"><span data-stu-id="decb0-103">Delete educationUser</span></span>

<span data-ttu-id="decb0-104">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="decb0-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="decb0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="decb0-105">Permissions</span></span>
<span data-ttu-id="decb0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="decb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="decb0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="decb0-108">Permission type</span></span>      | <span data-ttu-id="decb0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="decb0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="decb0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="decb0-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="decb0-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="decb0-111">Not supported.</span></span>  |
|<span data-ttu-id="decb0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="decb0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="decb0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="decb0-113">Not supported.</span></span>  |
|<span data-ttu-id="decb0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="decb0-114">Application</span></span> | <span data-ttu-id="decb0-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="decb0-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="decb0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="decb0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="decb0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="decb0-117">Request headers</span></span>
| <span data-ttu-id="decb0-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="decb0-118">Header</span></span>       | <span data-ttu-id="decb0-119">Значение</span><span class="sxs-lookup"><span data-stu-id="decb0-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="decb0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="decb0-120">Authorization</span></span>  | <span data-ttu-id="decb0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="decb0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="decb0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="decb0-123">Request body</span></span>
<span data-ttu-id="decb0-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="decb0-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="decb0-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="decb0-125">Response</span></span>
<span data-ttu-id="decb0-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="decb0-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="decb0-128">Пример</span><span class="sxs-lookup"><span data-stu-id="decb0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="decb0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="decb0-129">Request</span></span>
<span data-ttu-id="decb0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="decb0-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="decb0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="decb0-131">Response</span></span>
<span data-ttu-id="decb0-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="decb0-132">The following is an example of the response.</span></span> 
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
