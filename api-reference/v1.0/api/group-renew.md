---
title: 'group: renew'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 46a51d0a1d4bea5cebc4c3178f6776d80f313fbd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922734"
---
# <a name="group-renew"></a><span data-ttu-id="9e24b-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="9e24b-104">group: renew</span></span>

<span data-ttu-id="9e24b-105">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="9e24b-105">Renews a group's expiration.</span></span> <span data-ttu-id="9e24b-106">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="9e24b-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e24b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e24b-107">Permissions</span></span>

<span data-ttu-id="9e24b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e24b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="9e24b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e24b-110">Permission type</span></span>      | <span data-ttu-id="9e24b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e24b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e24b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e24b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9e24b-113">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e24b-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e24b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e24b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e24b-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9e24b-115">Not supported</span></span> |
|<span data-ttu-id="9e24b-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9e24b-116">Application</span></span> | <span data-ttu-id="9e24b-117">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e24b-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e24b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e24b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="9e24b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e24b-119">Request headers</span></span>
| <span data-ttu-id="9e24b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9e24b-120">Name</span></span>       | <span data-ttu-id="9e24b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9e24b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9e24b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e24b-122">Authorization</span></span>  | <span data-ttu-id="9e24b-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9e24b-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="9e24b-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e24b-124">Request body</span></span>

<span data-ttu-id="9e24b-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e24b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e24b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e24b-126">Response</span></span>

<span data-ttu-id="9e24b-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9e24b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e24b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9e24b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9e24b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e24b-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="9e24b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e24b-131">Response</span></span>
<span data-ttu-id="9e24b-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e24b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
