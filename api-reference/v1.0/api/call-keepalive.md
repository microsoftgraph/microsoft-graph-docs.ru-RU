---
title: 'Call: keepAlive'
description: Сделайте запрос к этому API каждые 15 – 45 минут, чтобы убедиться в том, что текущий вызов остается активным.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 32de1b3a24c6b37640376cdf7b60289ced5f90f3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866344"
---
# <a name="call-keepalive"></a><span data-ttu-id="1030b-103">Call: keepAlive</span><span class="sxs-lookup"><span data-stu-id="1030b-103">call: keepAlive</span></span>

<span data-ttu-id="1030b-104">Сделайте запрос к этому API каждые 15 – 45 минут, чтобы убедиться, что текущий вызов остается активным.</span><span class="sxs-lookup"><span data-stu-id="1030b-104">Make a request to this API every 15 to 45 minutes to ensure that an ongoing call remains active.</span></span> <span data-ttu-id="1030b-105">Вызов, не получающий этот запрос в течение 45 минут, считается неактивным и позднее завершается.</span><span class="sxs-lookup"><span data-stu-id="1030b-105">A call that does not receive this request within 45 minutes is considered inactive and will subsequently end.</span></span>

<span data-ttu-id="1030b-106">По крайней мере один успешный запрос должен быть выполнен в течение 45 минут предыдущего запроса или с начала вызова.</span><span class="sxs-lookup"><span data-stu-id="1030b-106">At least one successful request must be made within 45 minutes of the previous request, or the start of the call.</span></span>

<span data-ttu-id="1030b-107">Мы рекомендуем отправлять запрос через более короткие интервалы времени (каждые 15 минут).</span><span class="sxs-lookup"><span data-stu-id="1030b-107">We recommend that you send a request in shorter time intervals (every 15 minutes).</span></span> <span data-ttu-id="1030b-108">Убедитесь, что эти запросы выполнены успешно, чтобы предотвратить истечение времени и завершения вызова.</span><span class="sxs-lookup"><span data-stu-id="1030b-108">Make sure that these requests are successful to prevent the call from timing out and ending.</span></span>

<span data-ttu-id="1030b-109">Попытка отправить запрос на уже завершенный вызов приведет к `404 Not-Found` ошибке.</span><span class="sxs-lookup"><span data-stu-id="1030b-109">Attempting to send a request to a call that has already ended will result in a `404 Not-Found` error.</span></span> <span data-ttu-id="1030b-110">Ресурсы, связанные с вызовом, необходимо очистить на стороне приложения.</span><span class="sxs-lookup"><span data-stu-id="1030b-110">The resources related to the call should be cleaned up on the application side.</span></span>

## <a name="permissions"></a><span data-ttu-id="1030b-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="1030b-111">Permissions</span></span>
<span data-ttu-id="1030b-112">Для вызова этого API может потребоваться одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="1030b-112">One of the following permissions may be required to call this API.</span></span> <span data-ttu-id="1030b-113">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1030b-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1030b-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1030b-114">Permission type</span></span> | <span data-ttu-id="1030b-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1030b-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="1030b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1030b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="1030b-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1030b-117">Not Supported</span></span>        |
| <span data-ttu-id="1030b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1030b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1030b-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1030b-119">Not Supported</span></span>        |
| <span data-ttu-id="1030b-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="1030b-120">Application</span></span>     | <span data-ttu-id="1030b-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="1030b-121">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="1030b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1030b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a><span data-ttu-id="1030b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1030b-123">Request headers</span></span>
| <span data-ttu-id="1030b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1030b-124">Name</span></span>          | <span data-ttu-id="1030b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1030b-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1030b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1030b-126">Authorization</span></span> | <span data-ttu-id="1030b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1030b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1030b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1030b-129">Request body</span></span>
<span data-ttu-id="1030b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1030b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1030b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1030b-131">Response</span></span>
<span data-ttu-id="1030b-132">Этот метод возвращает код `200 OK` отклика.</span><span class="sxs-lookup"><span data-stu-id="1030b-132">This method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1030b-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="1030b-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1030b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1030b-134">Request</span></span>
<span data-ttu-id="1030b-135">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1030b-135">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1030b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1030b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1030b-137">C#</span><span class="sxs-lookup"><span data-stu-id="1030b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/keep-alive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1030b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1030b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/keep-alive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1030b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1030b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/keep-alive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1030b-140">Java</span><span class="sxs-lookup"><span data-stu-id="1030b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/keep-alive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1030b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1030b-141">Response</span></span>
<span data-ttu-id="1030b-142">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1030b-142">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "keep-alive",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 200 OK
```


<!--
{
  "type": "#page.annotation",
  "description": "call: keepAlive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
