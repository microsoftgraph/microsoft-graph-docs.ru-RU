---
title: 'сообщение: отказ от подписки'
description: Отправка запроса электронной почты от имени вошедшего пользователя для отказа от подписки на список рассылки электронной почты. Использует информацию в `List-Unsubscribe` заголовке.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e3f3378f813bce61f5ecef5b6003fb10fc680d59
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456873"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="0282c-104">сообщение: отказ от подписки</span><span class="sxs-lookup"><span data-stu-id="0282c-104">message: unsubscribe</span></span>

<span data-ttu-id="0282c-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0282c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0282c-106">Отправка запроса электронной почты от имени вошедшего пользователя для отказа от подписки на список рассылки электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0282c-106">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="0282c-107">Использует информацию в `List-Unsubscribe` заголовке.</span><span class="sxs-lookup"><span data-stu-id="0282c-107">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="0282c-108">Отправители сообщений могут использовать списки рассылки в удобном для пользователя виде, включая возможность отказаться от получателей. Это можно сделать, указав `List-Unsubscribe` заголовок в каждом сообщении, описанном в [документе RFC – 2369](https://www.faqs.org/rfcs/rfc2369.html).</span><span class="sxs-lookup"><span data-stu-id="0282c-108">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="0282c-109">**Note (Примечание** ) В частности, чтобы действие **отмены подписки** работало, отправителю необходимо указать и не `mailto:` указывать сведения об отмене подписки на основе URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="0282c-109">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="0282c-110">При задании этого заголовка `true`для свойства **unsubscribeEnabled** экземпляра [Message](../resources/message.md) также будет задано значение, а свойству **unsubscribeData** — данные заголовка.</span><span class="sxs-lookup"><span data-stu-id="0282c-110">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="0282c-111">Если свойство **unsubscribeEnabled** сообщения имеет `true`значение, можно использовать действие **Отменить подписку** , чтобы отменить подписку на пользователя из похожих будущих сообщений, которыми управляет отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="0282c-111">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="0282c-112">При успешном завершении операции **отмены подписки** сообщение перемещается в папку " **Удаленные** ".</span><span class="sxs-lookup"><span data-stu-id="0282c-112">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="0282c-113">Фактическим исключением пользователя из будущей рассылки почты управляет отправитель.</span><span class="sxs-lookup"><span data-stu-id="0282c-113">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="0282c-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0282c-114">Permissions</span></span>
<span data-ttu-id="0282c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0282c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0282c-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0282c-117">Permission type</span></span>      | <span data-ttu-id="0282c-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0282c-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0282c-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0282c-119">Delegated (work or school account)</span></span> | <span data-ttu-id="0282c-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0282c-120">Mail.Send</span></span>    |
|<span data-ttu-id="0282c-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0282c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0282c-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0282c-122">Mail.Send</span></span>    |
|<span data-ttu-id="0282c-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0282c-123">Application</span></span> | <span data-ttu-id="0282c-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0282c-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="0282c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0282c-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="0282c-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0282c-126">Request headers</span></span>
| <span data-ttu-id="0282c-127">Имя</span><span class="sxs-lookup"><span data-stu-id="0282c-127">Name</span></span>       | <span data-ttu-id="0282c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="0282c-128">Type</span></span> | <span data-ttu-id="0282c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0282c-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0282c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0282c-130">Authorization</span></span>  | <span data-ttu-id="0282c-131">string</span><span class="sxs-lookup"><span data-stu-id="0282c-131">string</span></span>  | <span data-ttu-id="0282c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0282c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0282c-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0282c-134">Request body</span></span>
<span data-ttu-id="0282c-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0282c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0282c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0282c-136">Response</span></span>

<span data-ttu-id="0282c-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0282c-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0282c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0282c-139">Example</span></span>
<span data-ttu-id="0282c-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0282c-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0282c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0282c-141">Request</span></span>
<span data-ttu-id="0282c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0282c-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0282c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0282c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```
# <a name="c"></a>[<span data-ttu-id="0282c-144">C#</span><span class="sxs-lookup"><span data-stu-id="0282c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-unsubscribe-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0282c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0282c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-unsubscribe-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0282c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0282c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-unsubscribe-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0282c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0282c-147">Response</span></span>
<span data-ttu-id="0282c-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0282c-148">Here is an example of the response.</span></span> 
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
