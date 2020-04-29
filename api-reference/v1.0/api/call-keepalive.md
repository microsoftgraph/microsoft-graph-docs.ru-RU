---
title: 'Call: keepAlive'
description: Сделайте запрос к этому API каждые 15 – 45 минут, чтобы убедиться в том, что текущий вызов остается активным.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 37af131e5e51f1bb0388bc002465aef71a8059a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518716"
---
# <a name="call-keepalive"></a><span data-ttu-id="67954-103">Call: keepAlive</span><span class="sxs-lookup"><span data-stu-id="67954-103">call: keepAlive</span></span>

<span data-ttu-id="67954-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67954-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67954-105">Сделайте запрос к этому API каждые 15 – 45 минут, чтобы убедиться, что текущий вызов остается активным.</span><span class="sxs-lookup"><span data-stu-id="67954-105">Make a request to this API every 15 to 45 minutes to ensure that an ongoing call remains active.</span></span> <span data-ttu-id="67954-106">Вызов, не получающий этот запрос в течение 45 минут, считается неактивным и позднее завершается.</span><span class="sxs-lookup"><span data-stu-id="67954-106">A call that does not receive this request within 45 minutes is considered inactive and will subsequently end.</span></span>

<span data-ttu-id="67954-107">По крайней мере один успешный запрос должен быть выполнен в течение 45 минут предыдущего запроса или с начала вызова.</span><span class="sxs-lookup"><span data-stu-id="67954-107">At least one successful request must be made within 45 minutes of the previous request, or the start of the call.</span></span>

<span data-ttu-id="67954-108">Мы рекомендуем отправлять запрос через более короткие интервалы времени (каждые 15 минут).</span><span class="sxs-lookup"><span data-stu-id="67954-108">We recommend that you send a request in shorter time intervals (every 15 minutes).</span></span> <span data-ttu-id="67954-109">Убедитесь, что эти запросы выполнены успешно, чтобы предотвратить истечение времени и завершения вызова.</span><span class="sxs-lookup"><span data-stu-id="67954-109">Make sure that these requests are successful to prevent the call from timing out and ending.</span></span>

<span data-ttu-id="67954-110">Попытка отправить запрос на уже завершенный вызов приведет к `404 Not-Found` ошибке.</span><span class="sxs-lookup"><span data-stu-id="67954-110">Attempting to send a request to a call that has already ended will result in a `404 Not-Found` error.</span></span> <span data-ttu-id="67954-111">Ресурсы, связанные с вызовом, необходимо очистить на стороне приложения.</span><span class="sxs-lookup"><span data-stu-id="67954-111">The resources related to the call should be cleaned up on the application side.</span></span>

## <a name="permissions"></a><span data-ttu-id="67954-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67954-112">Permissions</span></span>
<span data-ttu-id="67954-113">Для вызова этого API может потребоваться одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="67954-113">One of the following permissions may be required to call this API.</span></span> <span data-ttu-id="67954-114">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67954-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67954-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67954-115">Permission type</span></span> | <span data-ttu-id="67954-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67954-116">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="67954-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67954-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="67954-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="67954-118">Not Supported</span></span>        |
| <span data-ttu-id="67954-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67954-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67954-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="67954-120">Not Supported</span></span>        |
| <span data-ttu-id="67954-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67954-121">Application</span></span>     | <span data-ttu-id="67954-122">Нет</span><span class="sxs-lookup"><span data-stu-id="67954-122">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="67954-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67954-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a><span data-ttu-id="67954-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67954-124">Request headers</span></span>
| <span data-ttu-id="67954-125">Имя</span><span class="sxs-lookup"><span data-stu-id="67954-125">Name</span></span>          | <span data-ttu-id="67954-126">Описание</span><span class="sxs-lookup"><span data-stu-id="67954-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="67954-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67954-127">Authorization</span></span> | <span data-ttu-id="67954-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67954-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67954-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67954-130">Request body</span></span>
<span data-ttu-id="67954-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67954-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67954-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="67954-132">Response</span></span>
<span data-ttu-id="67954-133">Этот метод возвращает код `200 OK` отклика.</span><span class="sxs-lookup"><span data-stu-id="67954-133">This method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="67954-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="67954-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="67954-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="67954-135">Request</span></span>
<span data-ttu-id="67954-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67954-136">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67954-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="67954-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```
# <a name="c"></a>[<span data-ttu-id="67954-138">C#</span><span class="sxs-lookup"><span data-stu-id="67954-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/keep-alive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67954-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67954-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/keep-alive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67954-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67954-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/keep-alive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67954-141">Java</span><span class="sxs-lookup"><span data-stu-id="67954-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/keep-alive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="67954-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="67954-142">Response</span></span>
<span data-ttu-id="67954-143">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67954-143">The following example shows the response.</span></span>

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
