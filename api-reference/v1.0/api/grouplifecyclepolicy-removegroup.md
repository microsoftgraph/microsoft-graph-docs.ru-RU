---
title: 'groupLifecyclePolicy: removeGroup'
description: Удаляет группу из политики жизненного цикла.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3e6ff89d43b92694a912d9f550e578b3c338501d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317051"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="7de20-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="7de20-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="7de20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7de20-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7de20-105">Удаляет группу из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="7de20-105">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="7de20-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7de20-106">Permissions</span></span>

<span data-ttu-id="7de20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7de20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7de20-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7de20-109">Permission type</span></span>      | <span data-ttu-id="7de20-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7de20-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7de20-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7de20-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7de20-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7de20-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7de20-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7de20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7de20-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7de20-114">Not supported.</span></span>    |
|<span data-ttu-id="7de20-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7de20-115">Application</span></span> | <span data-ttu-id="7de20-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7de20-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7de20-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7de20-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="7de20-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7de20-118">Request headers</span></span>

| <span data-ttu-id="7de20-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7de20-119">Name</span></span> | <span data-ttu-id="7de20-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7de20-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7de20-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7de20-121">Authorization</span></span> | <span data-ttu-id="7de20-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7de20-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7de20-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7de20-124">Content-Type</span></span>  | <span data-ttu-id="7de20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7de20-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7de20-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7de20-126">Request body</span></span>
<span data-ttu-id="7de20-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7de20-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7de20-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="7de20-128">Parameter</span></span> | <span data-ttu-id="7de20-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7de20-129">Type</span></span> | <span data-ttu-id="7de20-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7de20-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7de20-131">groupId</span><span class="sxs-lookup"><span data-stu-id="7de20-131">groupId</span></span>|<span data-ttu-id="7de20-132">String</span><span class="sxs-lookup"><span data-stu-id="7de20-132">String</span></span>| <span data-ttu-id="7de20-133">Идентификатор группы, удаляемой из политики.</span><span class="sxs-lookup"><span data-stu-id="7de20-133">The identifier of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="7de20-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7de20-134">Response</span></span>

<span data-ttu-id="7de20-135">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="7de20-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="7de20-136">Если группа удалена из политики, в теле ответа возвращается `true` значение.</span><span class="sxs-lookup"><span data-stu-id="7de20-136">If the group is removed from the policy, a `true` value is returned in the response body.</span></span> <span data-ttu-id="7de20-137">В противном `false` случае в теле ответа возвращается значение.</span><span class="sxs-lookup"><span data-stu-id="7de20-137">Otherwise, a `false` value is returned in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7de20-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7de20-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7de20-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7de20-139">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="7de20-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7de20-140">Response</span></span>
<!-- { "blockType": "response" } -->

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

