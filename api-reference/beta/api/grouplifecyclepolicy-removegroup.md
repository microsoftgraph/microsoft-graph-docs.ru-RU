---
title: 'groupLifecyclePolicy: removeGroup'
description: Удаляет группу из политики жизненного цикла.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8519429a6824801ca6759077a55542c21982c542
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123967"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="e1fb7-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="e1fb7-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="e1fb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1fb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1fb7-105">Удаляет группу из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="e1fb7-105">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1fb7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1fb7-106">Permissions</span></span>

<span data-ttu-id="e1fb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1fb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e1fb7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1fb7-109">Permission type</span></span>      | <span data-ttu-id="e1fb7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1fb7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1fb7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1fb7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e1fb7-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1fb7-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1fb7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1fb7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1fb7-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e1fb7-114">Not supported</span></span> |
|<span data-ttu-id="e1fb7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1fb7-115">Application</span></span> |  <span data-ttu-id="e1fb7-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1fb7-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1fb7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1fb7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="e1fb7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1fb7-118">Request headers</span></span>

| <span data-ttu-id="e1fb7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e1fb7-119">Name</span></span> | <span data-ttu-id="e1fb7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e1fb7-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e1fb7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1fb7-121">Authorization</span></span> | <span data-ttu-id="e1fb7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1fb7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1fb7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1fb7-124">Content-Type</span></span>  | <span data-ttu-id="e1fb7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1fb7-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1fb7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1fb7-126">Request body</span></span>
<span data-ttu-id="e1fb7-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e1fb7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e1fb7-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="e1fb7-128">Parameter</span></span> | <span data-ttu-id="e1fb7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e1fb7-129">Type</span></span> | <span data-ttu-id="e1fb7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e1fb7-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e1fb7-131">groupId</span><span class="sxs-lookup"><span data-stu-id="e1fb7-131">groupId</span></span>|<span data-ttu-id="e1fb7-132">GUID</span><span class="sxs-lookup"><span data-stu-id="e1fb7-132">Guid</span></span>| <span data-ttu-id="e1fb7-133">Идентификатор группы, которую нужно удалить из политики.</span><span class="sxs-lookup"><span data-stu-id="e1fb7-133">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="e1fb7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1fb7-134">Response</span></span>

<span data-ttu-id="e1fb7-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e1fb7-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="e1fb7-136">Если из политики удаляется группа, в теле отклика возвращается значение **true**.</span><span class="sxs-lookup"><span data-stu-id="e1fb7-136">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="e1fb7-137">Если нет, то в теле отклика возвращается значение **false**.</span><span class="sxs-lookup"><span data-stu-id="e1fb7-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="e1fb7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e1fb7-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e1fb7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1fb7-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="e1fb7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1fb7-140">Response</span></span>
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
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
