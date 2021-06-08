---
title: 'канал: removeEmail'
description: Удаление предварительной электронной почты канала.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4608538cf136ba4f53a960183bc0b3f4bd7fc269
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813250"
---
# <a name="channel-removeemail"></a><span data-ttu-id="01ca7-103">канал: removeEmail</span><span class="sxs-lookup"><span data-stu-id="01ca7-103">channel: removeEmail</span></span>

<span data-ttu-id="01ca7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01ca7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01ca7-105">Удаление предварительного адреса электронной почты [канала.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="01ca7-105">Remove the provisioned email address of a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="01ca7-106">Удалить адрес электронной почты можно только в том случае, если он был с помощью метода [provisionEmail](channel-provisionemail.md) или Microsoft Teams клиента.</span><span class="sxs-lookup"><span data-stu-id="01ca7-106">You can remove an email address only if it was provisioned using the [provisionEmail](channel-provisionemail.md) method or through the Microsoft Teams client.</span></span>

## <a name="permissions"></a><span data-ttu-id="01ca7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01ca7-107">Permissions</span></span>

<span data-ttu-id="01ca7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01ca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01ca7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01ca7-110">Permission type</span></span>                        | <span data-ttu-id="01ca7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01ca7-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="01ca7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01ca7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="01ca7-113">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01ca7-113">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="01ca7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01ca7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01ca7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01ca7-115">Not supported.</span></span>                              |
| <span data-ttu-id="01ca7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01ca7-116">Application</span></span>                            | <span data-ttu-id="01ca7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01ca7-117">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="01ca7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01ca7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/removeEmail
```
## <a name="request-headers"></a><span data-ttu-id="01ca7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01ca7-119">Request headers</span></span>
| <span data-ttu-id="01ca7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01ca7-120">Header</span></span>        | <span data-ttu-id="01ca7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01ca7-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="01ca7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01ca7-122">Authorization</span></span> | <span data-ttu-id="01ca7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01ca7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01ca7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01ca7-125">Request body</span></span>

<span data-ttu-id="01ca7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01ca7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01ca7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="01ca7-127">Response</span></span>

<span data-ttu-id="01ca7-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="01ca7-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="01ca7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="01ca7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="01ca7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="01ca7-130">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_removeemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/removeEmail
```

### <a name="response"></a><span data-ttu-id="01ca7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="01ca7-131">Response</span></span>
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


