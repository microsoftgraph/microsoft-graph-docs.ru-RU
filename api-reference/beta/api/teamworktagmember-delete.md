---
title: Удаление командной работыTagMember
description: Удаление объекта teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 84a97aaf87fa2f2bcf5b1ff16d30a3ac6383266f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210006"
---
# <a name="delete-teamworktagmember"></a><span data-ttu-id="e4fc1-103">Удаление командной работыTagMember</span><span class="sxs-lookup"><span data-stu-id="e4fc1-103">Delete teamworkTagMember</span></span>
<span data-ttu-id="e4fc1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4fc1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4fc1-105">Удаление [участника из](../resources/teamworktagmember.md) стандартного тега в команде.</span><span class="sxs-lookup"><span data-stu-id="e4fc1-105">Delete a [member](../resources/teamworktagmember.md) from a standard tag in the team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e4fc1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4fc1-106">Permissions</span></span>
<span data-ttu-id="e4fc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4fc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4fc1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4fc1-109">Permission type</span></span>|<span data-ttu-id="e4fc1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4fc1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4fc1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4fc1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e4fc1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4fc1-112">Not supported.</span></span>|
|<span data-ttu-id="e4fc1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4fc1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4fc1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4fc1-114">Not supported.</span></span>|
|<span data-ttu-id="e4fc1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e4fc1-115">Application</span></span>|<span data-ttu-id="e4fc1-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4fc1-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4fc1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4fc1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-Id}/tags/{teamworkTag-Id}/members/{teamworkTagMember-Id}
```

## <a name="request-headers"></a><span data-ttu-id="e4fc1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4fc1-118">Request headers</span></span>
|<span data-ttu-id="e4fc1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e4fc1-119">Name</span></span>|<span data-ttu-id="e4fc1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e4fc1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4fc1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4fc1-121">Authorization</span></span>|<span data-ttu-id="e4fc1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4fc1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4fc1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4fc1-124">Request body</span></span>
<span data-ttu-id="e4fc1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4fc1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4fc1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4fc1-126">Response</span></span>

<span data-ttu-id="e4fc1-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4fc1-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e4fc1-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e4fc1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4fc1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4fc1-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e4fc1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4fc1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamworktagmember"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==
```
# <a name="c"></a>[<span data-ttu-id="e4fc1-131">C#</span><span class="sxs-lookup"><span data-stu-id="e4fc1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamworktagmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4fc1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4fc1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamworktagmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4fc1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4fc1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamworktagmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4fc1-134">Java</span><span class="sxs-lookup"><span data-stu-id="e4fc1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamworktagmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e4fc1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4fc1-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
