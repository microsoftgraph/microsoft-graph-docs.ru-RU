---
title: Close Session
description: 'Используйте этот API для закрытия существующего сеанса книги. '
author: lumine2008
ms.openlocfilehash: b44e708616bd6f115c166f5c66d74a54fb3734b0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324964"
---
# <a name="close-session"></a><span data-ttu-id="88d4a-103">Close Session</span><span class="sxs-lookup"><span data-stu-id="88d4a-103">Close Session</span></span>

<span data-ttu-id="88d4a-104">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="88d4a-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="88d4a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88d4a-105">Permissions</span></span>
<span data-ttu-id="88d4a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88d4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88d4a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88d4a-108">Permission type</span></span>      | <span data-ttu-id="88d4a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88d4a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88d4a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88d4a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88d4a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88d4a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="88d4a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88d4a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88d4a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88d4a-113">Not supported.</span></span>    |
|<span data-ttu-id="88d4a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88d4a-114">Application</span></span> | <span data-ttu-id="88d4a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88d4a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88d4a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88d4a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="88d4a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88d4a-117">Request headers</span></span>
| <span data-ttu-id="88d4a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="88d4a-118">Name</span></span>       | <span data-ttu-id="88d4a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="88d4a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="88d4a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88d4a-120">Authorization</span></span>  | <span data-ttu-id="88d4a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88d4a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88d4a-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="88d4a-123">workbook-session-id</span></span> | <span data-ttu-id="88d4a-124">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="88d4a-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="88d4a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88d4a-125">Request body</span></span>
<span data-ttu-id="88d4a-126">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="88d4a-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="88d4a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="88d4a-127">Response</span></span>

<span data-ttu-id="88d4a-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="88d4a-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88d4a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="88d4a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88d4a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="88d4a-130">Request</span></span>
<span data-ttu-id="88d4a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88d4a-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="88d4a-132">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="88d4a-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="88d4a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="88d4a-133">Response</span></span>
<span data-ttu-id="88d4a-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="88d4a-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```