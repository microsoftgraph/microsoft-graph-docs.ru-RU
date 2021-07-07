---
title: 'groupLifecyclePolicy: addGroup'
description: Добавляет группу к политике жизненного цикла.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8deeafa852b69af919fb79b43acaa5b588bdcd35
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316701"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="d6b0c-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="d6b0c-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="d6b0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6b0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6b0c-105">Добавляет определенные группы в политику жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="d6b0c-105">Adds specific groups to a lifecycle policy.</span></span> <span data-ttu-id="d6b0c-106">Это действие ограничивает политику жизненного цикла группы набором групп только в том случае, если установлено свойство **managedGroupTypes** [groupLifecyclePolicy.](../resources/grouplifecyclepolicy.md) `Selected`</span><span class="sxs-lookup"><span data-stu-id="d6b0c-106">This action limits the group lifecycle policy to a set of groups only if the **managedGroupTypes** property of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) is set to `Selected`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6b0c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6b0c-107">Permissions</span></span>

<span data-ttu-id="d6b0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6b0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d6b0c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6b0c-110">Permission type</span></span>      | <span data-ttu-id="d6b0c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6b0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6b0c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6b0c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d6b0c-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b0c-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6b0c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6b0c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6b0c-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d6b0c-115">Not supported</span></span> |
|<span data-ttu-id="d6b0c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6b0c-116">Application</span></span> | <span data-ttu-id="d6b0c-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b0c-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6b0c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6b0c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="d6b0c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6b0c-119">Request headers</span></span>

| <span data-ttu-id="d6b0c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d6b0c-120">Name</span></span> | <span data-ttu-id="d6b0c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d6b0c-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d6b0c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6b0c-122">Authorization</span></span> | <span data-ttu-id="d6b0c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6b0c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6b0c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6b0c-125">Content-Type</span></span>  | <span data-ttu-id="d6b0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6b0c-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6b0c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6b0c-127">Request body</span></span>
<span data-ttu-id="d6b0c-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d6b0c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d6b0c-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="d6b0c-129">Parameter</span></span> | <span data-ttu-id="d6b0c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d6b0c-130">Type</span></span> | <span data-ttu-id="d6b0c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d6b0c-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d6b0c-132">groupId</span><span class="sxs-lookup"><span data-stu-id="d6b0c-132">groupId</span></span>|<span data-ttu-id="d6b0c-133">String</span><span class="sxs-lookup"><span data-stu-id="d6b0c-133">String</span></span>| <span data-ttu-id="d6b0c-134">Идентификатор группы, добавляемой в политику.</span><span class="sxs-lookup"><span data-stu-id="d6b0c-134">The identifier of the group to add to the policy.</span></span> |

<span data-ttu-id="d6b0c-135">Когда **установлено свойство managedGroupTypes** [groupLifecyclePolicy,](../resources/grouplifecyclepolicy.md) в список можно добавить до `Selected` 500 групп.</span><span class="sxs-lookup"><span data-stu-id="d6b0c-135">When the **managedGroupTypes** property of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) is set to `Selected`, you can add up to 500 groups to the list.</span></span> <span data-ttu-id="d6b0c-136">Если вам нужно добавить более 500 групп, необходимо установить свойство **managedGroupTypes** [groupLifecyclePolicy.](../resources/grouplifecyclepolicy.md) `All`</span><span class="sxs-lookup"><span data-stu-id="d6b0c-136">If you need to add more than 500 groups, the **managedGroupTypes** property of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) must be set to `All`.</span></span>

<span data-ttu-id="d6b0c-137">На каждый запрос можно добавить только одну группу.</span><span class="sxs-lookup"><span data-stu-id="d6b0c-137">Only one group can be added per request.</span></span>

## <a name="response"></a><span data-ttu-id="d6b0c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6b0c-138">Response</span></span>

<span data-ttu-id="d6b0c-139">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d6b0c-139">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="d6b0c-140">Если группа добавлена в политику, в теле ответа возвращается `true` значение.</span><span class="sxs-lookup"><span data-stu-id="d6b0c-140">If the group is added to the policy, a `true` value is returned in the response body.</span></span> <span data-ttu-id="d6b0c-141">В противном `false` случае в теле ответа возвращается значение.</span><span class="sxs-lookup"><span data-stu-id="d6b0c-141">Otherwise, a `false` value is returned in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6b0c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d6b0c-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d6b0c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6b0c-143">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d6b0c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6b0c-144">Response</span></span>
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


