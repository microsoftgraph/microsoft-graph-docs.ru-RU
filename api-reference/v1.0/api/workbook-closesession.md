---
title: Close Session
description: 'Используйте этот API для закрытия существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 0e4d00b1ebf9ba90f6085f8dc7fc1005375efc0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818636"
---
# <a name="close-session"></a><span data-ttu-id="86bda-103">Close Session</span><span class="sxs-lookup"><span data-stu-id="86bda-103">Close Session</span></span>

<span data-ttu-id="86bda-104">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="86bda-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="86bda-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86bda-105">Permissions</span></span>
<span data-ttu-id="86bda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86bda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86bda-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86bda-108">Permission type</span></span>      | <span data-ttu-id="86bda-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86bda-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86bda-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86bda-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86bda-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86bda-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="86bda-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86bda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86bda-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86bda-113">Not supported.</span></span>    |
|<span data-ttu-id="86bda-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86bda-114">Application</span></span> | <span data-ttu-id="86bda-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86bda-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86bda-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86bda-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="86bda-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86bda-117">Request headers</span></span>
| <span data-ttu-id="86bda-118">Имя</span><span class="sxs-lookup"><span data-stu-id="86bda-118">Name</span></span>       | <span data-ttu-id="86bda-119">Описание</span><span class="sxs-lookup"><span data-stu-id="86bda-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="86bda-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86bda-120">Authorization</span></span>  | <span data-ttu-id="86bda-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86bda-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="86bda-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="86bda-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="86bda-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="86bda-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="86bda-126">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="86bda-126">workbook-session-id</span></span> | <span data-ttu-id="86bda-127">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="86bda-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="86bda-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86bda-128">Request body</span></span>
<span data-ttu-id="86bda-129">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="86bda-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="86bda-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="86bda-130">Response</span></span>

<span data-ttu-id="86bda-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="86bda-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="86bda-132">Пример</span><span class="sxs-lookup"><span data-stu-id="86bda-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86bda-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="86bda-133">Request</span></span>
<span data-ttu-id="86bda-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86bda-134">Here is an example of the request.</span></span>
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

<span data-ttu-id="86bda-135">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="86bda-135">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="86bda-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="86bda-136">Response</span></span>
<span data-ttu-id="86bda-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="86bda-137">Here is an example of the response.</span></span> 

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
