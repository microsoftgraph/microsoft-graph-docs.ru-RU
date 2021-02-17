---
title: Создание plannerRosterMember
description: Создание объекта plannerRosterMember.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e7dac57941d50ee8b543c53982c216c4c19d5d07
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272443"
---
# <a name="create-plannerrostermember"></a><span data-ttu-id="f67d2-103">Создание plannerRosterMember</span><span class="sxs-lookup"><span data-stu-id="f67d2-103">Create plannerRosterMember</span></span>
<span data-ttu-id="f67d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f67d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f67d2-105">Добавьте член в объект [plannerRoster.](../resources/plannerrostermember.md)</span><span class="sxs-lookup"><span data-stu-id="f67d2-105">Add a member to the [plannerRoster](../resources/plannerrostermember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f67d2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f67d2-106">Permissions</span></span>
<span data-ttu-id="f67d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f67d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f67d2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f67d2-109">Permission type</span></span>|<span data-ttu-id="f67d2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f67d2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f67d2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f67d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f67d2-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f67d2-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f67d2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f67d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f67d2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f67d2-114">Not supported.</span></span>|
|<span data-ttu-id="f67d2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f67d2-115">Application</span></span>|<span data-ttu-id="f67d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f67d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f67d2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f67d2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /planner/rosters/{plannerRosterId}/members
```

## <a name="request-headers"></a><span data-ttu-id="f67d2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f67d2-118">Request headers</span></span>
|<span data-ttu-id="f67d2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f67d2-119">Name</span></span>|<span data-ttu-id="f67d2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f67d2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f67d2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f67d2-121">Authorization</span></span>|<span data-ttu-id="f67d2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f67d2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f67d2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f67d2-124">Content-Type</span></span>|<span data-ttu-id="f67d2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f67d2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f67d2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f67d2-127">Request body</span></span>
<span data-ttu-id="f67d2-128">В теле запроса укажу представление объекта [plannerRosterMember](../resources/plannerrostermember.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="f67d2-128">In the request body, supply a JSON representation of the [plannerRosterMember](../resources/plannerrostermember.md) object.</span></span>

<span data-ttu-id="f67d2-129">В следующей таблице показаны свойства, необходимые при создании [объекта plannerRosterMember.](../resources/plannerrostermember.md)</span><span class="sxs-lookup"><span data-stu-id="f67d2-129">The following table shows the properties that are required when you create the [plannerRosterMember](../resources/plannerrostermember.md).</span></span>

|<span data-ttu-id="f67d2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f67d2-130">Property</span></span>|<span data-ttu-id="f67d2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f67d2-131">Type</span></span>|<span data-ttu-id="f67d2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f67d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f67d2-133">userId</span><span class="sxs-lookup"><span data-stu-id="f67d2-133">userId</span></span>|<span data-ttu-id="f67d2-134">String</span><span class="sxs-lookup"><span data-stu-id="f67d2-134">String</span></span>|<span data-ttu-id="f67d2-135">Идентификатор .</span><span class="sxs-lookup"><span data-stu-id="f67d2-135">Identifier of the .</span></span>|
|<span data-ttu-id="f67d2-136">tenantId</span><span class="sxs-lookup"><span data-stu-id="f67d2-136">tenantId</span></span>|<span data-ttu-id="f67d2-137">String</span><span class="sxs-lookup"><span data-stu-id="f67d2-137">String</span></span>|<span data-ttu-id="f67d2-138">Идентификатор клиента, к котором принадлежит пользователь.</span><span class="sxs-lookup"><span data-stu-id="f67d2-138">Identifier of the tenant the user belongs to.</span></span> <span data-ttu-id="f67d2-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f67d2-139">Optional.</span></span> <span data-ttu-id="f67d2-140">В настоящее время участники группы не могут быть из разных клиентов.</span><span class="sxs-lookup"><span data-stu-id="f67d2-140">Currently roster members cannot be from different tenants.</span></span>|
|<span data-ttu-id="f67d2-141">roles</span><span class="sxs-lookup"><span data-stu-id="f67d2-141">roles</span></span>|<span data-ttu-id="f67d2-142">Набор строк</span><span class="sxs-lookup"><span data-stu-id="f67d2-142">String collection</span></span>|<span data-ttu-id="f67d2-143">Дополнительные роли, назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="f67d2-143">Additional roles assigned to the user.</span></span> <span data-ttu-id="f67d2-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f67d2-144">Optional.</span></span> <span data-ttu-id="f67d2-145">В настоящее время для пользователей не доступны дополнительные роли.</span><span class="sxs-lookup"><span data-stu-id="f67d2-145">Currently there are no additional roles available for users.</span></span>|



## <a name="response"></a><span data-ttu-id="f67d2-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="f67d2-146">Response</span></span>

<span data-ttu-id="f67d2-147">В случае успеха этот метод возвращает код отклика и объект `201 Created` [plannerRosterMember](../resources/plannerrostermember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f67d2-147">If successful, this method returns a `201 Created` response code and a [plannerRosterMember](../resources/plannerrostermember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f67d2-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="f67d2-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f67d2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f67d2-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f67d2-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="f67d2-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerrostermember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members
Content-Type: application/json
Content-length: 78

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "userId": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="f67d2-151">C#</span><span class="sxs-lookup"><span data-stu-id="f67d2-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerrostermember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f67d2-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f67d2-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerrostermember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f67d2-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f67d2-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerrostermember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f67d2-154">Java</span><span class="sxs-lookup"><span data-stu-id="f67d2-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerrostermember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f67d2-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f67d2-155">Response</span></span>
<span data-ttu-id="f67d2-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f67d2-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRosterMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "id": "670095cd-95cd-6700-cd95-0067cd950067",
  "userId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
  "roles": [
  ]
}
```

