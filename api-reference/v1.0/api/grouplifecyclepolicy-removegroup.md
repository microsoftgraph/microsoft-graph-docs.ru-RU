---
title: 'groupLifecyclePolicy: removeGroup'
description: Удаляет группу из политики жизненного цикла.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 33e5900c93801f54f4f705f59d25895e32da797d
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124632"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="2f379-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="2f379-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="2f379-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f379-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f379-105">Удаляет группу из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="2f379-105">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f379-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f379-106">Permissions</span></span>

<span data-ttu-id="2f379-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f379-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f379-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f379-109">Permission type</span></span>      | <span data-ttu-id="2f379-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f379-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f379-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f379-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2f379-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f379-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="2f379-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f379-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f379-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f379-114">Not supported.</span></span>    |
|<span data-ttu-id="2f379-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f379-115">Application</span></span> | <span data-ttu-id="2f379-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f379-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f379-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f379-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="2f379-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f379-118">Request headers</span></span>

| <span data-ttu-id="2f379-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2f379-119">Name</span></span> | <span data-ttu-id="2f379-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2f379-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2f379-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f379-121">Authorization</span></span> | <span data-ttu-id="2f379-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f379-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f379-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f379-124">Content-Type</span></span>  | <span data-ttu-id="2f379-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f379-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f379-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f379-126">Request body</span></span>
<span data-ttu-id="2f379-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2f379-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f379-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="2f379-128">Parameter</span></span> | <span data-ttu-id="2f379-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2f379-129">Type</span></span> | <span data-ttu-id="2f379-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2f379-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2f379-131">groupId</span><span class="sxs-lookup"><span data-stu-id="2f379-131">groupId</span></span>|<span data-ttu-id="2f379-132">GUID</span><span class="sxs-lookup"><span data-stu-id="2f379-132">Guid</span></span>| <span data-ttu-id="2f379-133">Идентификатор группы, которую нужно удалить из политики.</span><span class="sxs-lookup"><span data-stu-id="2f379-133">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="2f379-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f379-134">Response</span></span>

<span data-ttu-id="2f379-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2f379-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="2f379-136">Если из политики удаляется группа, в теле отклика возвращается значение **true**.</span><span class="sxs-lookup"><span data-stu-id="2f379-136">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="2f379-137">Если нет, то в теле отклика возвращается значение **false**.</span><span class="sxs-lookup"><span data-stu-id="2f379-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="2f379-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2f379-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2f379-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f379-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="2f379-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f379-140">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
