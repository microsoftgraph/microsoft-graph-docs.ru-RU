---
title: Удаление Тимеоффрекуест
description: Удаление объекта Тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 89ec693d533e39075bde89992eaba55ebd8656e4
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215887"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="b1d24-103">Удаление Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="b1d24-103">Delete timeOffRequest</span></span>

<span data-ttu-id="b1d24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1d24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1d24-105">Удаление объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="b1d24-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1d24-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1d24-106">Permissions</span></span>

<span data-ttu-id="b1d24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1d24-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1d24-109">Permission type</span></span>                        | <span data-ttu-id="b1d24-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1d24-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="b1d24-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1d24-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b1d24-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b1d24-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1d24-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1d24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1d24-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1d24-114">Not supported.</span></span>    |
|<span data-ttu-id="b1d24-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="b1d24-115">Application</span></span> | <span data-ttu-id="b1d24-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1d24-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="b1d24-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b1d24-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b1d24-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="b1d24-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b1d24-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1d24-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="b1d24-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1d24-120">Request headers</span></span>

| <span data-ttu-id="b1d24-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b1d24-121">Name</span></span>          | <span data-ttu-id="b1d24-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b1d24-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b1d24-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1d24-123">Authorization</span></span> | <span data-ttu-id="b1d24-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1d24-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1d24-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1d24-126">Request body</span></span>

<span data-ttu-id="b1d24-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1d24-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1d24-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1d24-128">Response</span></span>

<span data-ttu-id="b1d24-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1d24-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1d24-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b1d24-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1d24-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1d24-132">Request</span></span>

<span data-ttu-id="b1d24-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1d24-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b1d24-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1d24-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="b1d24-135">C#</span><span class="sxs-lookup"><span data-stu-id="b1d24-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1d24-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1d24-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1d24-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1d24-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1d24-138">Java</span><span class="sxs-lookup"><span data-stu-id="b1d24-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-timeoffrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="b1d24-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1d24-139">Response</span></span>

<span data-ttu-id="b1d24-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b1d24-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
