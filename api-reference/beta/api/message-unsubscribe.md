---
title: 'сообщение: отписаться'
description: Отправляет запрос электронной почты от имени пользователя, выполнившего вход Чтобы отписаться от список рассылки по электронной почте. Использует сведения, приведенные в `List-Unsubscribe` заголовка.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f66c24e2900ca4c881d08a402698dacbaf5af5f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877688"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="80fe8-104">сообщение: отписаться</span><span class="sxs-lookup"><span data-stu-id="80fe8-104">message: unsubscribe</span></span>

> <span data-ttu-id="80fe8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="80fe8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80fe8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80fe8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80fe8-107">Отправляет запрос электронной почты от имени пользователя, выполнившего вход Чтобы отписаться от список рассылки по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="80fe8-107">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="80fe8-108">Использует сведения, приведенные в `List-Unsubscribe` заголовка.</span><span class="sxs-lookup"><span data-stu-id="80fe8-108">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="80fe8-109">Отправители сообщений можно использовать списки рассылки понятным способом, включив параметр для получателей для отключить. Они могут делать это путем указания `List-Unsubscribe` верхнего колонтитула в каждое сообщение, выполнив [RFC 2369](https://www.faqs.org/rfcs/rfc2369.html).</span><span class="sxs-lookup"><span data-stu-id="80fe8-109">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="80fe8-110">**Примечание** В частности, для **отмены подписки** действия для работы отправителя необходимо указать `mailto:` и не на основе URL-адреса отписаться сведения.</span><span class="sxs-lookup"><span data-stu-id="80fe8-110">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="80fe8-111">Установка заголовок, также установить свойство **unsubscribeEnabled** экземпляра [сообщение](../resources/message.md) `true`и свойство **unsubscribeData** для данные заголовка.</span><span class="sxs-lookup"><span data-stu-id="80fe8-111">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="80fe8-112">Если свойство **unsubscribeEnabled** сообщения является `true`, можно использовать действие **отписаться** Чтобы отписаться пользователя из следующего последующих сообщений, которым осуществляется путем отправителя сообщения.</span><span class="sxs-lookup"><span data-stu-id="80fe8-112">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="80fe8-113">Успешные **отписаться** действие перемещает сообщение для папки « **Удаленные** ».</span><span class="sxs-lookup"><span data-stu-id="80fe8-113">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="80fe8-114">Фактические исключения пользователя из будущих почты распределения управляется отправителя.</span><span class="sxs-lookup"><span data-stu-id="80fe8-114">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="80fe8-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80fe8-115">Permissions</span></span>
<span data-ttu-id="80fe8-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80fe8-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80fe8-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80fe8-118">Permission type</span></span>      | <span data-ttu-id="80fe8-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80fe8-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80fe8-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80fe8-120">Delegated (work or school account)</span></span> | <span data-ttu-id="80fe8-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="80fe8-121">Mail.Send</span></span>    |
|<span data-ttu-id="80fe8-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80fe8-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80fe8-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="80fe8-123">Mail.Send</span></span>    |
|<span data-ttu-id="80fe8-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80fe8-124">Application</span></span> | <span data-ttu-id="80fe8-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="80fe8-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="80fe8-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80fe8-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="80fe8-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80fe8-127">Request headers</span></span>
| <span data-ttu-id="80fe8-128">Имя</span><span class="sxs-lookup"><span data-stu-id="80fe8-128">Name</span></span>       | <span data-ttu-id="80fe8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="80fe8-129">Type</span></span> | <span data-ttu-id="80fe8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="80fe8-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80fe8-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="80fe8-131">Authorization</span></span>  | <span data-ttu-id="80fe8-132">string</span><span class="sxs-lookup"><span data-stu-id="80fe8-132">string</span></span>  | <span data-ttu-id="80fe8-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80fe8-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80fe8-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80fe8-135">Request body</span></span>
<span data-ttu-id="80fe8-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80fe8-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80fe8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="80fe8-137">Response</span></span>

<span data-ttu-id="80fe8-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="80fe8-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80fe8-140">Пример</span><span class="sxs-lookup"><span data-stu-id="80fe8-140">Example</span></span>
<span data-ttu-id="80fe8-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="80fe8-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80fe8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="80fe8-142">Request</span></span>
<span data-ttu-id="80fe8-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80fe8-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="80fe8-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="80fe8-144">Response</span></span>
<span data-ttu-id="80fe8-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80fe8-145">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
