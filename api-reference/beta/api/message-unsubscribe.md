---
title: 'message: unsubscribe'
description: Отправка запроса электронной почты от имени во включенного пользователя, чтобы отписаться от списка рассылки электронной почты. Использует сведения в `List-Unsubscribe` заголке.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7bf800fe385c75c6d472f9cee40f55ec81633640
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131108"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="6e706-104">message: unsubscribe</span><span class="sxs-lookup"><span data-stu-id="6e706-104">message: unsubscribe</span></span>

<span data-ttu-id="6e706-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e706-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e706-106">Отправка запроса электронной почты от имени во включенного пользователя, чтобы отписаться от списка рассылки электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6e706-106">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="6e706-107">Использует сведения в `List-Unsubscribe` заголке.</span><span class="sxs-lookup"><span data-stu-id="6e706-107">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="6e706-108">Отправителю сообщений удобно использовать списки рассылки, включив для получателей возможность отказаться от них. Это можно сделать, указав заголок в каждом сообщении после `List-Unsubscribe` [RFC-2369.](https://www.faqs.org/rfcs/rfc2369.html)</span><span class="sxs-lookup"><span data-stu-id="6e706-108">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="6e706-109">**Примечание** В частности,  чтобы действие отписки работало, отправитель должен указать информацию, основанную на URL-адресе, а не `mailto:` отписаться от нее.</span><span class="sxs-lookup"><span data-stu-id="6e706-109">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="6e706-110">При установке этого загона свойству **unsubscribeEnabled** экземпляра сообщения будет задано свойство [](../resources/message.md) `true` **unsubscribeData, а свойству unsubscribeData** для данных загона.</span><span class="sxs-lookup"><span data-stu-id="6e706-110">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="6e706-111">Если свойство **unsubscribeEnabled** сообщения, вы можете использовать действие отписаться, чтобы отписать пользователя от похожих будущих сообщений, управляемых отправителям `true` сообщений. </span><span class="sxs-lookup"><span data-stu-id="6e706-111">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="6e706-112">Успешное **действие отписаться** перемещает сообщение в папку **"Удаленные".**</span><span class="sxs-lookup"><span data-stu-id="6e706-112">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="6e706-113">Фактическое исключение пользователя из дальнейшего распространения почты управляется отправителями.</span><span class="sxs-lookup"><span data-stu-id="6e706-113">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e706-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e706-114">Permissions</span></span>
<span data-ttu-id="6e706-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e706-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e706-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e706-117">Permission type</span></span>      | <span data-ttu-id="6e706-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e706-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e706-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e706-119">Delegated (work or school account)</span></span> | <span data-ttu-id="6e706-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6e706-120">Mail.Send</span></span>    |
|<span data-ttu-id="6e706-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e706-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e706-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6e706-122">Mail.Send</span></span>    |
|<span data-ttu-id="6e706-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e706-123">Application</span></span> | <span data-ttu-id="6e706-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6e706-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e706-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e706-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="6e706-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e706-126">Request headers</span></span>
| <span data-ttu-id="6e706-127">Имя</span><span class="sxs-lookup"><span data-stu-id="6e706-127">Name</span></span>       | <span data-ttu-id="6e706-128">Тип</span><span class="sxs-lookup"><span data-stu-id="6e706-128">Type</span></span> | <span data-ttu-id="6e706-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6e706-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6e706-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e706-130">Authorization</span></span>  | <span data-ttu-id="6e706-131">string</span><span class="sxs-lookup"><span data-stu-id="6e706-131">string</span></span>  | <span data-ttu-id="6e706-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e706-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e706-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e706-134">Request body</span></span>
<span data-ttu-id="6e706-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e706-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e706-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e706-136">Response</span></span>

<span data-ttu-id="6e706-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6e706-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e706-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6e706-139">Example</span></span>
<span data-ttu-id="6e706-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6e706-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e706-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e706-141">Request</span></span>
<span data-ttu-id="6e706-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e706-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e706-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e706-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```
# <a name="c"></a>[<span data-ttu-id="6e706-144">C#</span><span class="sxs-lookup"><span data-stu-id="6e706-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-unsubscribe-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e706-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e706-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-unsubscribe-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e706-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e706-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-unsubscribe-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e706-147">Java</span><span class="sxs-lookup"><span data-stu-id="6e706-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-unsubscribe-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6e706-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e706-148">Response</span></span>
<span data-ttu-id="6e706-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6e706-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


