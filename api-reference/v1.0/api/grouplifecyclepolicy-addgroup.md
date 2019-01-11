---
title: 'groupLifecyclePolicy: addGroup'
description: Добавляет группу к политике жизненного цикла.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: f021a1e31e811ea9c1618adaa5750978a689fdc5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870093"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="1ef21-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="1ef21-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="1ef21-104">Добавляет группу к политике жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="1ef21-104">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ef21-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ef21-105">Permissions</span></span>

<span data-ttu-id="1ef21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ef21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1ef21-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ef21-108">Permission type</span></span>      | <span data-ttu-id="1ef21-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ef21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ef21-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ef21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ef21-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ef21-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ef21-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ef21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ef21-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ef21-113">Not supported.</span></span>    |
|<span data-ttu-id="1ef21-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ef21-114">Application</span></span> | <span data-ttu-id="1ef21-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ef21-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ef21-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ef21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="1ef21-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ef21-117">Request headers</span></span>

| <span data-ttu-id="1ef21-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1ef21-118">Name</span></span> | <span data-ttu-id="1ef21-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef21-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1ef21-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ef21-120">Authorization</span></span> | <span data-ttu-id="1ef21-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ef21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ef21-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ef21-123">Content-Type</span></span>  | <span data-ttu-id="1ef21-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ef21-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ef21-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ef21-125">Request body</span></span>
<span data-ttu-id="1ef21-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1ef21-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1ef21-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="1ef21-127">Parameter</span></span> | <span data-ttu-id="1ef21-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1ef21-128">Type</span></span> | <span data-ttu-id="1ef21-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef21-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1ef21-130">groupId</span><span class="sxs-lookup"><span data-stu-id="1ef21-130">groupId</span></span>|<span data-ttu-id="1ef21-131">GUID</span><span class="sxs-lookup"><span data-stu-id="1ef21-131">Guid</span></span>| <span data-ttu-id="1ef21-132">Идентификатор группы, которую нужно добавить к политике.</span><span class="sxs-lookup"><span data-stu-id="1ef21-132">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="1ef21-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ef21-133">Response</span></span>

<span data-ttu-id="1ef21-134">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1ef21-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="1ef21-135">Если к политике добавляется группа, в теле отклика возвращается значение **true**.</span><span class="sxs-lookup"><span data-stu-id="1ef21-135">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="1ef21-136">Если нет, то в теле отклика возвращается значение **false**.</span><span class="sxs-lookup"><span data-stu-id="1ef21-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="1ef21-137">Пример</span><span class="sxs-lookup"><span data-stu-id="1ef21-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1ef21-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ef21-138">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="1ef21-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ef21-139">Response</span></span>
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
