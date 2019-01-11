---
title: Refresh Session
description: 'Используйте этот API для обновления существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 686325dd106af01d1f8f3fcf94b5bdb9ad4b000f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831222"
---
# <a name="refresh-session"></a><span data-ttu-id="9441b-103">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="9441b-103">Refresh Session</span></span>

<span data-ttu-id="9441b-104">Используйте этот API для обновления существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="9441b-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9441b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9441b-105">Permissions</span></span>
<span data-ttu-id="9441b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9441b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9441b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9441b-108">Permission type</span></span>      | <span data-ttu-id="9441b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9441b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9441b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9441b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9441b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9441b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9441b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9441b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9441b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9441b-113">Not supported.</span></span>    |
|<span data-ttu-id="9441b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9441b-114">Application</span></span> | <span data-ttu-id="9441b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9441b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9441b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9441b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="9441b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9441b-117">Request headers</span></span>
| <span data-ttu-id="9441b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9441b-118">Name</span></span>       | <span data-ttu-id="9441b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9441b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9441b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9441b-120">Authorization</span></span>  | <span data-ttu-id="9441b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9441b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9441b-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="9441b-123">workbook-session-id</span></span> | <span data-ttu-id="9441b-124">Идентификатор сеанса для книги, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9441b-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="9441b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9441b-125">Request body</span></span>
<span data-ttu-id="9441b-126">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="9441b-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="9441b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9441b-127">Response</span></span>

<span data-ttu-id="9441b-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9441b-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9441b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9441b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9441b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9441b-130">Request</span></span>
<span data-ttu-id="9441b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9441b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="9441b-132">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="9441b-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="9441b-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9441b-133">Response</span></span>
<span data-ttu-id="9441b-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9441b-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: refresh_excel_session//api-reference/v1.0/api/workbook-refreshsession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
