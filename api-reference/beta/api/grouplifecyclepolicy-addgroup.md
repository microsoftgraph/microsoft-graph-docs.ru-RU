---
title: 'groupLifecyclePolicy: addGroup'
description: Добавляет группу к политике жизненного цикла.
ms.openlocfilehash: 59f49429f65112488f42727cdbb46fc0a4b87800
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079948"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="1a699-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="1a699-103">groupLifecyclePolicy: addGroup</span></span>

> <span data-ttu-id="1a699-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1a699-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a699-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a699-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a699-106">Добавляет группу к политике жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="1a699-106">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a699-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a699-107">Permissions</span></span>

<span data-ttu-id="1a699-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a699-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1a699-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a699-110">Permission type</span></span>      | <span data-ttu-id="1a699-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a699-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a699-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a699-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a699-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a699-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a699-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a699-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a699-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1a699-115">Not supported</span></span> |
|<span data-ttu-id="1a699-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a699-116">Application</span></span> | <span data-ttu-id="1a699-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a699-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a699-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a699-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="1a699-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a699-119">Request headers</span></span>

| <span data-ttu-id="1a699-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1a699-120">Name</span></span> | <span data-ttu-id="1a699-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1a699-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1a699-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a699-122">Authorization</span></span> | <span data-ttu-id="1a699-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a699-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a699-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a699-125">Content-Type</span></span>  | <span data-ttu-id="1a699-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a699-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a699-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a699-127">Request body</span></span>
<span data-ttu-id="1a699-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1a699-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a699-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="1a699-129">Parameter</span></span> | <span data-ttu-id="1a699-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1a699-130">Type</span></span> | <span data-ttu-id="1a699-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1a699-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1a699-132">groupId</span><span class="sxs-lookup"><span data-stu-id="1a699-132">groupId</span></span>|<span data-ttu-id="1a699-133">GUID</span><span class="sxs-lookup"><span data-stu-id="1a699-133">Guid</span></span>| <span data-ttu-id="1a699-134">Идентификатор группы, которую нужно добавить к политике.</span><span class="sxs-lookup"><span data-stu-id="1a699-134">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="1a699-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a699-135">Response</span></span>

<span data-ttu-id="1a699-136">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1a699-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="1a699-137">Если к политике добавляется группа, в теле отклика возвращается значение **true**.</span><span class="sxs-lookup"><span data-stu-id="1a699-137">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="1a699-138">Если нет, то в теле отклика возвращается значение **false**.</span><span class="sxs-lookup"><span data-stu-id="1a699-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="1a699-139">Пример</span><span class="sxs-lookup"><span data-stu-id="1a699-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1a699-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a699-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="1a699-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a699-141">Response</span></span>
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