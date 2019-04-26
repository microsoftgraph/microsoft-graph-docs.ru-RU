---
title: Close Session
description: 'Используйте этот API для закрытия существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9fbbaea28f93b757881550f36d76540fb6cfb388
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573566"
---
# <a name="close-session"></a><span data-ttu-id="e355e-103">Close Session</span><span class="sxs-lookup"><span data-stu-id="e355e-103">Close Session</span></span>

<span data-ttu-id="e355e-104">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="e355e-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e355e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e355e-105">Permissions</span></span>
<span data-ttu-id="e355e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e355e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e355e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e355e-108">Permission type</span></span>      | <span data-ttu-id="e355e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e355e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e355e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e355e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e355e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e355e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e355e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e355e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e355e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e355e-113">Not supported.</span></span>    |
|<span data-ttu-id="e355e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e355e-114">Application</span></span> | <span data-ttu-id="e355e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e355e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e355e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e355e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="e355e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e355e-117">Request headers</span></span>
| <span data-ttu-id="e355e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e355e-118">Name</span></span>       | <span data-ttu-id="e355e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e355e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e355e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e355e-120">Authorization</span></span>  | <span data-ttu-id="e355e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e355e-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="e355e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e355e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e355e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e355e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="e355e-126">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="e355e-126">workbook-session-id</span></span> | <span data-ttu-id="e355e-127">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="e355e-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="e355e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e355e-128">Request body</span></span>
<span data-ttu-id="e355e-129">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="e355e-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="e355e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e355e-130">Response</span></span>

<span data-ttu-id="e355e-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e355e-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e355e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e355e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e355e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e355e-133">Request</span></span>
<span data-ttu-id="e355e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e355e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="e355e-135">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e355e-135">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="e355e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e355e-136">Response</span></span>
<span data-ttu-id="e355e-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e355e-137">Here is an example of the response.</span></span> 

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
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
