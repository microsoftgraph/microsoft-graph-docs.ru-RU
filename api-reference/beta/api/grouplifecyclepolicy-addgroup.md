---
title: 'groupLifecyclePolicy: addGroup'
description: Добавляет группу к политике жизненного цикла.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fa88af236a42920a80a54933175adf1cebd821c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001871"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="e256f-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="e256f-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="e256f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e256f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e256f-105">Добавляет группу к политике жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="e256f-105">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="e256f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e256f-106">Permissions</span></span>

<span data-ttu-id="e256f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e256f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e256f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e256f-109">Permission type</span></span>      | <span data-ttu-id="e256f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e256f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e256f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e256f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e256f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e256f-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e256f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e256f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e256f-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e256f-114">Not supported</span></span> |
|<span data-ttu-id="e256f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e256f-115">Application</span></span> | <span data-ttu-id="e256f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e256f-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e256f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e256f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="e256f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e256f-118">Request headers</span></span>

| <span data-ttu-id="e256f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e256f-119">Name</span></span> | <span data-ttu-id="e256f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e256f-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e256f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e256f-121">Authorization</span></span> | <span data-ttu-id="e256f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e256f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e256f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e256f-124">Content-Type</span></span>  | <span data-ttu-id="e256f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e256f-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e256f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e256f-126">Request body</span></span>
<span data-ttu-id="e256f-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e256f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e256f-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="e256f-128">Parameter</span></span> | <span data-ttu-id="e256f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e256f-129">Type</span></span> | <span data-ttu-id="e256f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e256f-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e256f-131">groupId</span><span class="sxs-lookup"><span data-stu-id="e256f-131">groupId</span></span>|<span data-ttu-id="e256f-132">GUID</span><span class="sxs-lookup"><span data-stu-id="e256f-132">Guid</span></span>| <span data-ttu-id="e256f-133">Идентификатор группы, которую нужно добавить к политике.</span><span class="sxs-lookup"><span data-stu-id="e256f-133">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="e256f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e256f-134">Response</span></span>

<span data-ttu-id="e256f-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e256f-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="e256f-136">Если к политике добавляется группа, в теле отклика возвращается значение **true**.</span><span class="sxs-lookup"><span data-stu-id="e256f-136">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="e256f-137">Если нет, то в теле отклика возвращается значение **false**.</span><span class="sxs-lookup"><span data-stu-id="e256f-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="e256f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e256f-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e256f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e256f-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="e256f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e256f-140">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


