---
title: 'groupLifecyclePolicy: addGroup'
description: Добавляет группу к политике жизненного цикла.
author: dkershaw10
ms.openlocfilehash: 57af4383c471832acbffb4136a057c91a1d061d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327911"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="c5850-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="c5850-103">groupLifecyclePolicy: addGroup</span></span>

> <span data-ttu-id="c5850-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5850-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5850-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5850-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5850-106">Добавляет группу к политике жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="c5850-106">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5850-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5850-107">Permissions</span></span>

<span data-ttu-id="c5850-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5850-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c5850-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5850-110">Permission type</span></span>      | <span data-ttu-id="c5850-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5850-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5850-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5850-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5850-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5850-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c5850-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5850-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5850-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c5850-115">Not supported</span></span> |
|<span data-ttu-id="c5850-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5850-116">Application</span></span> | <span data-ttu-id="c5850-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5850-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5850-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5850-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="c5850-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5850-119">Request headers</span></span>

| <span data-ttu-id="c5850-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c5850-120">Name</span></span> | <span data-ttu-id="c5850-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c5850-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c5850-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5850-122">Authorization</span></span> | <span data-ttu-id="c5850-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5850-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5850-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5850-125">Content-Type</span></span>  | <span data-ttu-id="c5850-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5850-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5850-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5850-127">Request body</span></span>
<span data-ttu-id="c5850-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c5850-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5850-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="c5850-129">Parameter</span></span> | <span data-ttu-id="c5850-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c5850-130">Type</span></span> | <span data-ttu-id="c5850-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c5850-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c5850-132">groupId</span><span class="sxs-lookup"><span data-stu-id="c5850-132">groupId</span></span>|<span data-ttu-id="c5850-133">GUID</span><span class="sxs-lookup"><span data-stu-id="c5850-133">Guid</span></span>| <span data-ttu-id="c5850-134">Идентификатор группы, которую нужно добавить к политике.</span><span class="sxs-lookup"><span data-stu-id="c5850-134">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="c5850-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5850-135">Response</span></span>

<span data-ttu-id="c5850-136">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c5850-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="c5850-137">Если к политике добавляется группа, в теле отклика возвращается значение **true**.</span><span class="sxs-lookup"><span data-stu-id="c5850-137">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="c5850-138">Если нет, то в теле отклика возвращается значение **false**.</span><span class="sxs-lookup"><span data-stu-id="c5850-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="c5850-139">Пример</span><span class="sxs-lookup"><span data-stu-id="c5850-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c5850-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5850-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c5850-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5850-141">Response</span></span>
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