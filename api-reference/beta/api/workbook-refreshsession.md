---
title: Refresh Session
description: 'Используйте этот API для обновления существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 288f0b4b41841a6393af837f1b6e5c048dfae77e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536112"
---
# <a name="refresh-session"></a><span data-ttu-id="3d58c-103">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="3d58c-103">Refresh Session</span></span>

<span data-ttu-id="3d58c-104">Используйте этот API для обновления существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="3d58c-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3d58c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d58c-105">Permissions</span></span>
<span data-ttu-id="3d58c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d58c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d58c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d58c-108">Permission type</span></span>      | <span data-ttu-id="3d58c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d58c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d58c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d58c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d58c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d58c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3d58c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d58c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d58c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d58c-113">Not supported.</span></span>    |
|<span data-ttu-id="3d58c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d58c-114">Application</span></span> | <span data-ttu-id="3d58c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d58c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d58c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d58c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="3d58c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d58c-117">Request headers</span></span>
| <span data-ttu-id="3d58c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3d58c-118">Name</span></span>       | <span data-ttu-id="3d58c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3d58c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3d58c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d58c-120">Authorization</span></span>  | <span data-ttu-id="3d58c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d58c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d58c-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="3d58c-123">workbook-session-id</span></span> | <span data-ttu-id="3d58c-124">Идентификатор сеанса для книги, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3d58c-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d58c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3d58c-125">Request body</span></span>
<span data-ttu-id="3d58c-126">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="3d58c-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="3d58c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d58c-127">Response</span></span>

<span data-ttu-id="3d58c-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3d58c-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3d58c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3d58c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d58c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d58c-130">Request</span></span>
<span data-ttu-id="3d58c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d58c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="3d58c-132">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="3d58c-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="3d58c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d58c-133">Response</span></span>
<span data-ttu-id="3d58c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3d58c-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
