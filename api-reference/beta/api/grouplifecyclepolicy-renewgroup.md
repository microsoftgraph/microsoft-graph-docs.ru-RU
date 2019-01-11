---
title: 'groupLifecyclePolicy: renewGroup'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
ms.openlocfilehash: 5472927769175912736f66a2d848f103cfb5b8c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833322"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="d0ada-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="d0ada-104">groupLifecyclePolicy: renewGroup</span></span>

> <span data-ttu-id="d0ada-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d0ada-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0ada-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0ada-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0ada-107">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="d0ada-107">Renews a group's expiration.</span></span> <span data-ttu-id="d0ada-108">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="d0ada-108">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="d0ada-109">**Примечание:** В версии 1.0, [Используйте группы ресурсов следует обновить запросы](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="d0ada-109">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0ada-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0ada-110">Permissions</span></span>

<span data-ttu-id="d0ada-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0ada-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="d0ada-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0ada-113">Permission type</span></span>      | <span data-ttu-id="d0ada-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0ada-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0ada-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0ada-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d0ada-116">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ada-116">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0ada-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0ada-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0ada-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d0ada-118">Not supported</span></span> |
|<span data-ttu-id="d0ada-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d0ada-119">Application</span></span> | <span data-ttu-id="d0ada-120">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ada-120">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0ada-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0ada-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="d0ada-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0ada-122">Request headers</span></span>

| <span data-ttu-id="d0ada-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d0ada-123">Name</span></span> | <span data-ttu-id="d0ada-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d0ada-124">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d0ada-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0ada-125">Authorization</span></span> | <span data-ttu-id="d0ada-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0ada-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0ada-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0ada-128">Content-Type</span></span>  | <span data-ttu-id="d0ada-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d0ada-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0ada-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0ada-130">Request body</span></span>
<span data-ttu-id="d0ada-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d0ada-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d0ada-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="d0ada-132">Parameter</span></span> | <span data-ttu-id="d0ada-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d0ada-133">Type</span></span> | <span data-ttu-id="d0ada-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d0ada-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d0ada-135">groupId</span><span class="sxs-lookup"><span data-stu-id="d0ada-135">groupId</span></span>|<span data-ttu-id="d0ada-136">GUID</span><span class="sxs-lookup"><span data-stu-id="d0ada-136">Guid</span></span>| <span data-ttu-id="d0ada-137">Идентификатор группы для обновления.</span><span class="sxs-lookup"><span data-stu-id="d0ada-137">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="d0ada-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0ada-138">Response</span></span>

<span data-ttu-id="d0ada-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d0ada-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0ada-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d0ada-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d0ada-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0ada-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="d0ada-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0ada-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
