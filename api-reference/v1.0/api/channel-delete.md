---
title: Удаление канала
description: Удаление канала.
ms.openlocfilehash: b2756de636f38a14063a345ba2094c1cb628517c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024361"
---
# <a name="delete-channel"></a><span data-ttu-id="8690c-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="8690c-103">Delete channel</span></span>



<span data-ttu-id="8690c-104">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="8690c-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="8690c-105">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="8690c-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="8690c-106">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="8690c-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="8690c-107">**Примечание**: данных в удаленные каналы будут храниться в течение нескольких недель разрешить владельцем группы для восстановления удаленных канала.</span><span class="sxs-lookup"><span data-stu-id="8690c-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="8690c-108">В это время новый канал с одной displayName может быть создан.</span><span class="sxs-lookup"><span data-stu-id="8690c-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="8690c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8690c-109">Permissions</span></span>
<span data-ttu-id="8690c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8690c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8690c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8690c-112">Permission type</span></span>      | <span data-ttu-id="8690c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8690c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8690c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8690c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8690c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8690c-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8690c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8690c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8690c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8690c-117">Not supported.</span></span>    |
|<span data-ttu-id="8690c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8690c-118">Application</span></span> | <span data-ttu-id="8690c-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8690c-119">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="8690c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8690c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8690c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8690c-121">Request headers</span></span>
| <span data-ttu-id="8690c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8690c-122">Header</span></span>       | <span data-ttu-id="8690c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8690c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8690c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8690c-124">Authorization</span></span>  | <span data-ttu-id="8690c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8690c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8690c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8690c-127">Request body</span></span>
<span data-ttu-id="8690c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8690c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8690c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8690c-129">Response</span></span>

<span data-ttu-id="8690c-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8690c-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8690c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8690c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8690c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8690c-133">Request</span></span>
<span data-ttu-id="8690c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8690c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="8690c-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="8690c-135">Response</span></span>

<span data-ttu-id="8690c-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8690c-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
