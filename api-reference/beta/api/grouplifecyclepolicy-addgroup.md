---
title: 'groupLifecyclePolicy: addGroup'
description: Добавляет группу к политике жизненного цикла.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3909d7a25a49c95e80041a4a708a5b8e823e0c91
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926626"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="2f2e2-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="2f2e2-103">groupLifecyclePolicy: addGroup</span></span>

> <span data-ttu-id="2f2e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f2e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f2e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f2e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f2e2-106">Добавляет группу к политике жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="2f2e2-106">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f2e2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f2e2-107">Permissions</span></span>

<span data-ttu-id="2f2e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f2e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2f2e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f2e2-110">Permission type</span></span>      | <span data-ttu-id="2f2e2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f2e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f2e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f2e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2f2e2-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f2e2-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="2f2e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f2e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f2e2-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2f2e2-115">Not supported</span></span> |
|<span data-ttu-id="2f2e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f2e2-116">Application</span></span> | <span data-ttu-id="2f2e2-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f2e2-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f2e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f2e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="2f2e2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f2e2-119">Request headers</span></span>

| <span data-ttu-id="2f2e2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2f2e2-120">Name</span></span> | <span data-ttu-id="2f2e2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2f2e2-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2f2e2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f2e2-122">Authorization</span></span> | <span data-ttu-id="2f2e2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f2e2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f2e2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f2e2-125">Content-Type</span></span>  | <span data-ttu-id="2f2e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f2e2-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f2e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f2e2-127">Request body</span></span>
<span data-ttu-id="2f2e2-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2f2e2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f2e2-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="2f2e2-129">Parameter</span></span> | <span data-ttu-id="2f2e2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2f2e2-130">Type</span></span> | <span data-ttu-id="2f2e2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2f2e2-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2f2e2-132">groupId</span><span class="sxs-lookup"><span data-stu-id="2f2e2-132">groupId</span></span>|<span data-ttu-id="2f2e2-133">GUID</span><span class="sxs-lookup"><span data-stu-id="2f2e2-133">Guid</span></span>| <span data-ttu-id="2f2e2-134">Идентификатор группы, которую нужно добавить к политике.</span><span class="sxs-lookup"><span data-stu-id="2f2e2-134">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="2f2e2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f2e2-135">Response</span></span>

<span data-ttu-id="2f2e2-136">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2f2e2-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="2f2e2-137">Если к политике добавляется группа, в теле отклика возвращается значение **true**.</span><span class="sxs-lookup"><span data-stu-id="2f2e2-137">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="2f2e2-138">Если нет, то в теле отклика возвращается значение **false**.</span><span class="sxs-lookup"><span data-stu-id="2f2e2-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="2f2e2-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2f2e2-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2f2e2-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f2e2-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2f2e2-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f2e2-141">Response</span></span>
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
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
