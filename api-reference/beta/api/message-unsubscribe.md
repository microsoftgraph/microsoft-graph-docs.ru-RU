---
title: 'сообщение: отказ от подписки'
description: Отправка запроса электронной почты от имени вошедшего пользователя для отказа от подписки на список рассылки электронной почты. Использует информацию в `List-Unsubscribe` заголовке.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 69d14315fc0732ed12db357f9aa9a0c837f48f29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540380"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="4d17e-104">сообщение: отказ от подписки</span><span class="sxs-lookup"><span data-stu-id="4d17e-104">message: unsubscribe</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d17e-105">Отправка запроса электронной почты от имени вошедшего пользователя для отказа от подписки на список рассылки электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4d17e-105">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="4d17e-106">Использует информацию в `List-Unsubscribe` заголовке.</span><span class="sxs-lookup"><span data-stu-id="4d17e-106">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="4d17e-107">Отправители сообщений могут использовать списки рассылки в удобном для пользователя виде, включая возможность отказаться от получателей. Это можно сделать, указав `List-Unsubscribe` заголовок в каждом сообщении, описанном в [документе RFC – 2369](https://www.faqs.org/rfcs/rfc2369.html).</span><span class="sxs-lookup"><span data-stu-id="4d17e-107">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="4d17e-108">**Note (Примечание** ) В частности, чтобы действие **отмены подписки** работало, отправителю необходимо указать и не `mailto:` указывать сведения об отмене подписки на основе URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="4d17e-108">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="4d17e-109">При задании этого заголовка `true`для свойства **unsubscribeEnabled** экземпляра [Message](../resources/message.md) также будет задано значение, а свойству **unsubscribeData** — данные заголовка.</span><span class="sxs-lookup"><span data-stu-id="4d17e-109">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="4d17e-110">Если свойство **unsubscribeEnabled** сообщения имеет `true`значение, можно использовать действие **Отменить подписку** , чтобы отменить подписку на пользователя из похожих будущих сообщений, которыми управляет отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="4d17e-110">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="4d17e-111">При успешном завершении операции **отмены подписки** сообщение перемещается в папку " **Удаленные** ".</span><span class="sxs-lookup"><span data-stu-id="4d17e-111">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="4d17e-112">Фактическим исключением пользователя из будущей рассылки почты управляет отправитель.</span><span class="sxs-lookup"><span data-stu-id="4d17e-112">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d17e-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d17e-113">Permissions</span></span>
<span data-ttu-id="4d17e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d17e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d17e-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d17e-116">Permission type</span></span>      | <span data-ttu-id="4d17e-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d17e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d17e-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d17e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="4d17e-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4d17e-119">Mail.Send</span></span>    |
|<span data-ttu-id="4d17e-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d17e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d17e-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4d17e-121">Mail.Send</span></span>    |
|<span data-ttu-id="4d17e-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d17e-122">Application</span></span> | <span data-ttu-id="4d17e-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4d17e-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d17e-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d17e-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="4d17e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d17e-125">Request headers</span></span>
| <span data-ttu-id="4d17e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="4d17e-126">Name</span></span>       | <span data-ttu-id="4d17e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4d17e-127">Type</span></span> | <span data-ttu-id="4d17e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4d17e-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d17e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d17e-129">Authorization</span></span>  | <span data-ttu-id="4d17e-130">string</span><span class="sxs-lookup"><span data-stu-id="4d17e-130">string</span></span>  | <span data-ttu-id="4d17e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d17e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d17e-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d17e-133">Request body</span></span>
<span data-ttu-id="4d17e-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d17e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d17e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d17e-135">Response</span></span>

<span data-ttu-id="4d17e-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4d17e-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d17e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4d17e-138">Example</span></span>
<span data-ttu-id="4d17e-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4d17e-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4d17e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d17e-140">Request</span></span>
<span data-ttu-id="4d17e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d17e-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="4d17e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d17e-142">Response</span></span>
<span data-ttu-id="4d17e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d17e-143">Here is an example of the response.</span></span> 
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
