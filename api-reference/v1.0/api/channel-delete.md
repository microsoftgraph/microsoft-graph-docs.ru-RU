---
title: Удаление канала
description: Удаление канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 846aa0b00fc07a0a25e3eb3aae07bcccdbd936ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565599"
---
# <a name="delete-channel"></a><span data-ttu-id="01b80-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="01b80-103">Delete channel</span></span>



<span data-ttu-id="01b80-104">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="01b80-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="01b80-105">**Note**: существует известная проблема, связанная с разрешениями приложения и этим API.</span><span class="sxs-lookup"><span data-stu-id="01b80-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="01b80-106">Дополнительные сведения см. в [списке известных проблем](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="01b80-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="01b80-107">**Note**: данные в удаленных каналах продолжат храниться в течение нескольких недель, чтобы владелец группы мог восстановить удаленный канал.</span><span class="sxs-lookup"><span data-stu-id="01b80-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="01b80-108">В течение этого времени не создается новый канал с таким же отображаемым именем (displayName).</span><span class="sxs-lookup"><span data-stu-id="01b80-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="01b80-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01b80-109">Permissions</span></span>
<span data-ttu-id="01b80-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01b80-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01b80-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01b80-112">Permission type</span></span>      | <span data-ttu-id="01b80-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01b80-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01b80-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01b80-114">Delegated (work or school account)</span></span> | <span data-ttu-id="01b80-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01b80-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="01b80-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01b80-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01b80-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01b80-117">Not supported.</span></span>    |
|<span data-ttu-id="01b80-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01b80-118">Application</span></span> | <span data-ttu-id="01b80-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01b80-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="01b80-120">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="01b80-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="01b80-121">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="01b80-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="01b80-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01b80-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="01b80-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01b80-123">Request headers</span></span>
| <span data-ttu-id="01b80-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01b80-124">Header</span></span>       | <span data-ttu-id="01b80-125">Значение</span><span class="sxs-lookup"><span data-stu-id="01b80-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01b80-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01b80-126">Authorization</span></span>  | <span data-ttu-id="01b80-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01b80-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01b80-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01b80-129">Request body</span></span>
<span data-ttu-id="01b80-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01b80-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01b80-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="01b80-131">Response</span></span>

<span data-ttu-id="01b80-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="01b80-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01b80-134">Пример</span><span class="sxs-lookup"><span data-stu-id="01b80-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01b80-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="01b80-135">Request</span></span>
<span data-ttu-id="01b80-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01b80-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="01b80-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="01b80-137">Response</span></span>

<span data-ttu-id="01b80-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01b80-138">The following is an example of the response.</span></span> 
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
