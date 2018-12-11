---
title: Удаление канала
description: Удаление канала.
ms.openlocfilehash: f24471a4f93c50d722290feb9093514c34f4cc2f
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222349"
---
# <a name="delete-channel"></a><span data-ttu-id="47178-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="47178-103">Delete channel</span></span>



<span data-ttu-id="47178-104">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="47178-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="47178-105">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="47178-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="47178-106">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="47178-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="47178-107">**Примечание**: данных в удаленные каналы будут храниться в течение нескольких недель разрешить владельцем группы для восстановления удаленных канала.</span><span class="sxs-lookup"><span data-stu-id="47178-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="47178-108">В это время новый канал с одной displayName может быть создан.</span><span class="sxs-lookup"><span data-stu-id="47178-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="47178-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47178-109">Permissions</span></span>
<span data-ttu-id="47178-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47178-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47178-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47178-112">Permission type</span></span>      | <span data-ttu-id="47178-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47178-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47178-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47178-114">Delegated (work or school account)</span></span> | <span data-ttu-id="47178-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47178-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="47178-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47178-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47178-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47178-117">Not supported.</span></span>    |
|<span data-ttu-id="47178-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47178-118">Application</span></span> | <span data-ttu-id="47178-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47178-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="47178-120">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="47178-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="47178-121">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="47178-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="47178-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47178-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="47178-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47178-123">Request headers</span></span>
| <span data-ttu-id="47178-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47178-124">Header</span></span>       | <span data-ttu-id="47178-125">Значение</span><span class="sxs-lookup"><span data-stu-id="47178-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47178-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47178-126">Authorization</span></span>  | <span data-ttu-id="47178-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47178-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47178-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47178-129">Request body</span></span>
<span data-ttu-id="47178-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47178-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47178-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="47178-131">Response</span></span>

<span data-ttu-id="47178-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="47178-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="47178-134">Пример</span><span class="sxs-lookup"><span data-stu-id="47178-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47178-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="47178-135">Request</span></span>
<span data-ttu-id="47178-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47178-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="47178-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="47178-137">Response</span></span>

<span data-ttu-id="47178-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="47178-138">The following is an example of the response.</span></span> 
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
