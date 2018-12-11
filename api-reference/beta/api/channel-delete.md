---
title: Удаление канала
description: Удаление канала.
ms.openlocfilehash: eaf061df0725b10cb45ed03cc674b7ae4800272e
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222494"
---
# <a name="delete-channel"></a><span data-ttu-id="76b56-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="76b56-103">Delete channel</span></span>

> <span data-ttu-id="76b56-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="76b56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76b56-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76b56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76b56-106">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="76b56-106">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="76b56-107">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="76b56-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="76b56-108">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="76b56-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="76b56-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76b56-109">Permissions</span></span>
<span data-ttu-id="76b56-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76b56-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76b56-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76b56-112">Permission type</span></span>      | <span data-ttu-id="76b56-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76b56-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76b56-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76b56-114">Delegated (work or school account)</span></span> | <span data-ttu-id="76b56-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b56-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="76b56-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76b56-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76b56-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76b56-117">Not supported.</span></span>    |
|<span data-ttu-id="76b56-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76b56-118">Application</span></span> | <span data-ttu-id="76b56-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b56-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="76b56-120">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="76b56-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="76b56-121">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="76b56-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="76b56-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76b56-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="76b56-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76b56-123">Request headers</span></span>
| <span data-ttu-id="76b56-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76b56-124">Header</span></span>       | <span data-ttu-id="76b56-125">Значение</span><span class="sxs-lookup"><span data-stu-id="76b56-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="76b56-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76b56-126">Authorization</span></span>  | <span data-ttu-id="76b56-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76b56-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76b56-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76b56-129">Request body</span></span>
<span data-ttu-id="76b56-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76b56-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76b56-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="76b56-131">Response</span></span>

<span data-ttu-id="76b56-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="76b56-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76b56-134">Пример</span><span class="sxs-lookup"><span data-stu-id="76b56-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76b56-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="76b56-135">Request</span></span>
<span data-ttu-id="76b56-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76b56-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="76b56-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="76b56-137">Response</span></span>

<span data-ttu-id="76b56-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="76b56-138">The following is an example of the response.</span></span> 
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
