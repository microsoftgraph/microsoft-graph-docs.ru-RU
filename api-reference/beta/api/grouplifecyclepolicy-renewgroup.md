---
title: 'groupLifecyclePolicy: Реневграуп'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7eb0ef44a5e07c8c293ba804cc8ec31a8312576d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501853"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="2e193-104">groupLifecyclePolicy: Реневграуп</span><span class="sxs-lookup"><span data-stu-id="2e193-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e193-105">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="2e193-105">Renews a group's expiration.</span></span> <span data-ttu-id="2e193-106">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="2e193-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="2e193-107">**Примечание:** В версии 1.0 [Используйте ресурс Group, чтобы выполнить обновление запросов](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="2e193-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e193-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e193-108">Permissions</span></span>

<span data-ttu-id="2e193-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e193-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="2e193-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e193-111">Permission type</span></span>      | <span data-ttu-id="2e193-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e193-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e193-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e193-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2e193-114">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e193-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e193-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e193-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e193-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2e193-116">Not supported</span></span> |
|<span data-ttu-id="2e193-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e193-117">Application</span></span> | <span data-ttu-id="2e193-118">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e193-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e193-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e193-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="2e193-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e193-120">Request headers</span></span>

| <span data-ttu-id="2e193-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2e193-121">Name</span></span> | <span data-ttu-id="2e193-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2e193-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2e193-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e193-123">Authorization</span></span> | <span data-ttu-id="2e193-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e193-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e193-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e193-126">Content-Type</span></span>  | <span data-ttu-id="2e193-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2e193-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e193-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e193-128">Request body</span></span>
<span data-ttu-id="2e193-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2e193-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2e193-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="2e193-130">Parameter</span></span> | <span data-ttu-id="2e193-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2e193-131">Type</span></span> | <span data-ttu-id="2e193-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2e193-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2e193-133">groupId</span><span class="sxs-lookup"><span data-stu-id="2e193-133">groupId</span></span>|<span data-ttu-id="2e193-134">GUID</span><span class="sxs-lookup"><span data-stu-id="2e193-134">Guid</span></span>| <span data-ttu-id="2e193-135">Идентификатор группы, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="2e193-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="2e193-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e193-136">Response</span></span>

<span data-ttu-id="2e193-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2e193-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e193-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2e193-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2e193-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e193-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="2e193-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e193-141">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
