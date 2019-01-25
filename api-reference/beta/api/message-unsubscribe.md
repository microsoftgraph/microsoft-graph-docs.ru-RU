---
title: 'сообщение: отписаться'
description: Отправляет запрос электронной почты от имени пользователя, выполнившего вход Чтобы отписаться от список рассылки по электронной почте. Использует сведения, приведенные в `List-Unsubscribe` заголовка.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 69d14315fc0732ed12db357f9aa9a0c837f48f29
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508827"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="443fd-104">сообщение: отписаться</span><span class="sxs-lookup"><span data-stu-id="443fd-104">message: unsubscribe</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="443fd-105">Отправляет запрос электронной почты от имени пользователя, выполнившего вход Чтобы отписаться от список рассылки по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="443fd-105">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="443fd-106">Использует сведения, приведенные в `List-Unsubscribe` заголовка.</span><span class="sxs-lookup"><span data-stu-id="443fd-106">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="443fd-107">Отправители сообщений можно использовать списки рассылки понятным способом, включив параметр для получателей для отключить. Они могут делать это путем указания `List-Unsubscribe` верхнего колонтитула в каждое сообщение, выполнив [RFC 2369](https://www.faqs.org/rfcs/rfc2369.html).</span><span class="sxs-lookup"><span data-stu-id="443fd-107">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="443fd-108">**Примечание** В частности, для **отмены подписки** действия для работы отправителя необходимо указать `mailto:` и не на основе URL-адреса отписаться сведения.</span><span class="sxs-lookup"><span data-stu-id="443fd-108">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="443fd-109">Установка заголовок, также установить свойство **unsubscribeEnabled** экземпляра [сообщение](../resources/message.md) `true`и свойство **unsubscribeData** для данные заголовка.</span><span class="sxs-lookup"><span data-stu-id="443fd-109">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="443fd-110">Если свойство **unsubscribeEnabled** сообщения является `true`, можно использовать действие **отписаться** Чтобы отписаться пользователя из следующего последующих сообщений, которым осуществляется путем отправителя сообщения.</span><span class="sxs-lookup"><span data-stu-id="443fd-110">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="443fd-111">Успешные **отписаться** действие перемещает сообщение для папки « **Удаленные** ».</span><span class="sxs-lookup"><span data-stu-id="443fd-111">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="443fd-112">Фактические исключения пользователя из будущих почты распределения управляется отправителя.</span><span class="sxs-lookup"><span data-stu-id="443fd-112">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="443fd-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="443fd-113">Permissions</span></span>
<span data-ttu-id="443fd-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="443fd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="443fd-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="443fd-116">Permission type</span></span>      | <span data-ttu-id="443fd-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="443fd-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="443fd-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="443fd-118">Delegated (work or school account)</span></span> | <span data-ttu-id="443fd-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="443fd-119">Mail.Send</span></span>    |
|<span data-ttu-id="443fd-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="443fd-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="443fd-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="443fd-121">Mail.Send</span></span>    |
|<span data-ttu-id="443fd-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="443fd-122">Application</span></span> | <span data-ttu-id="443fd-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="443fd-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="443fd-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="443fd-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="443fd-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="443fd-125">Request headers</span></span>
| <span data-ttu-id="443fd-126">Имя</span><span class="sxs-lookup"><span data-stu-id="443fd-126">Name</span></span>       | <span data-ttu-id="443fd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="443fd-127">Type</span></span> | <span data-ttu-id="443fd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="443fd-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="443fd-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="443fd-129">Authorization</span></span>  | <span data-ttu-id="443fd-130">string</span><span class="sxs-lookup"><span data-stu-id="443fd-130">string</span></span>  | <span data-ttu-id="443fd-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="443fd-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="443fd-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="443fd-133">Request body</span></span>
<span data-ttu-id="443fd-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="443fd-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="443fd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="443fd-135">Response</span></span>

<span data-ttu-id="443fd-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="443fd-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="443fd-138">Пример</span><span class="sxs-lookup"><span data-stu-id="443fd-138">Example</span></span>
<span data-ttu-id="443fd-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="443fd-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="443fd-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="443fd-140">Request</span></span>
<span data-ttu-id="443fd-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="443fd-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="443fd-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="443fd-142">Response</span></span>
<span data-ttu-id="443fd-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="443fd-143">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/message-unsubscribe.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
