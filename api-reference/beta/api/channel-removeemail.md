---
title: 'канал: removeEmail'
description: Удаление предварительной электронной почты канала.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 66efdd201217d34ba367df4ae1f30713cd939df4
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869611"
---
# <a name="channel-removeemail"></a><span data-ttu-id="64bd9-103">канал: removeEmail</span><span class="sxs-lookup"><span data-stu-id="64bd9-103">channel: removeEmail</span></span>

<span data-ttu-id="64bd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64bd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64bd9-105">Удаление предварительного адреса электронной почты [канала.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="64bd9-105">Remove the provisioned email address of a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="64bd9-106">Удалить адрес электронной почты можно только в том случае, если он был с помощью метода [provisionEmail](channel-provisionemail.md) или Microsoft Teams клиента.</span><span class="sxs-lookup"><span data-stu-id="64bd9-106">You can remove an email address only if it was provisioned using the [provisionEmail](channel-provisionemail.md) method or through the Microsoft Teams client.</span></span>

## <a name="permissions"></a><span data-ttu-id="64bd9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64bd9-107">Permissions</span></span>

<span data-ttu-id="64bd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64bd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64bd9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64bd9-110">Permission type</span></span>                        | <span data-ttu-id="64bd9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64bd9-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="64bd9-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64bd9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="64bd9-113">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bd9-113">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="64bd9-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64bd9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64bd9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64bd9-115">Not supported.</span></span>                              |
| <span data-ttu-id="64bd9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64bd9-116">Application</span></span>                            | <span data-ttu-id="64bd9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64bd9-117">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="64bd9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64bd9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/removeEmail
```
## <a name="request-headers"></a><span data-ttu-id="64bd9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64bd9-119">Request headers</span></span>
| <span data-ttu-id="64bd9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64bd9-120">Header</span></span>        | <span data-ttu-id="64bd9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64bd9-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="64bd9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64bd9-122">Authorization</span></span> | <span data-ttu-id="64bd9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64bd9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64bd9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64bd9-125">Request body</span></span>

<span data-ttu-id="64bd9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64bd9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64bd9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="64bd9-127">Response</span></span>

<span data-ttu-id="64bd9-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="64bd9-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="64bd9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="64bd9-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="64bd9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="64bd9-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64bd9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="64bd9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_removeemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/removeEmail
```
# <a name="c"></a>[<span data-ttu-id="64bd9-132">C#</span><span class="sxs-lookup"><span data-stu-id="64bd9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-removeemail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64bd9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64bd9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-removeemail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64bd9-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64bd9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-removeemail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64bd9-135">Java</span><span class="sxs-lookup"><span data-stu-id="64bd9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-removeemail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64bd9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="64bd9-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove channel email",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


