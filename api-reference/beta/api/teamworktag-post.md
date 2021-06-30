---
title: Создание командной работы
description: Создание нового объекта teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cc943f381d796dfa4c056c342eb5563ef59d585f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210053"
---
# <a name="create-teamworktag"></a><span data-ttu-id="3003e-103">Создание командной работы</span><span class="sxs-lookup"><span data-stu-id="3003e-103">Create teamworkTag</span></span>
<span data-ttu-id="3003e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3003e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3003e-105">Создайте [стандартный тег](../resources/teamworktag.md) для участников группы.</span><span class="sxs-lookup"><span data-stu-id="3003e-105">Create a standard [tag](../resources/teamworktag.md) for members in the team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3003e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3003e-106">Permissions</span></span>
<span data-ttu-id="3003e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3003e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3003e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3003e-109">Permission type</span></span>|<span data-ttu-id="3003e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3003e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3003e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3003e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3003e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3003e-112">Not supported.</span></span>|
|<span data-ttu-id="3003e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3003e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3003e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3003e-114">Not supported.</span></span>|
|<span data-ttu-id="3003e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3003e-115">Application</span></span>|<span data-ttu-id="3003e-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3003e-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3003e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3003e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags
```

## <a name="request-headers"></a><span data-ttu-id="3003e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3003e-118">Request headers</span></span>
|<span data-ttu-id="3003e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3003e-119">Name</span></span>|<span data-ttu-id="3003e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3003e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3003e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3003e-121">Authorization</span></span>|<span data-ttu-id="3003e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3003e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3003e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3003e-124">Content-Type</span></span>|<span data-ttu-id="3003e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3003e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3003e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3003e-127">Request body</span></span>
<span data-ttu-id="3003e-128">В теле запроса поставляем представление JSON объекта [teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="3003e-128">In the request body, supply a JSON representation of the [teamworkTag](../resources/teamworktag.md) object.</span></span>

<span data-ttu-id="3003e-129">В следующей таблице показаны свойства, необходимые при создании [teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="3003e-129">The following table shows the properties that are required when you create the [teamworkTag](../resources/teamworktag.md).</span></span>

|<span data-ttu-id="3003e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3003e-130">Property</span></span>|<span data-ttu-id="3003e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3003e-131">Type</span></span>|<span data-ttu-id="3003e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3003e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3003e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3003e-133">displayName</span></span>|<span data-ttu-id="3003e-134">String</span><span class="sxs-lookup"><span data-stu-id="3003e-134">String</span></span>|<span data-ttu-id="3003e-135">Имя тега.</span><span class="sxs-lookup"><span data-stu-id="3003e-135">Name of the tag.</span></span> <span data-ttu-id="3003e-136">Значение не может быть больше 40 символов.</span><span class="sxs-lookup"><span data-stu-id="3003e-136">The value can't be more than 40 characters.</span></span>|
|<span data-ttu-id="3003e-137">members</span><span class="sxs-lookup"><span data-stu-id="3003e-137">members</span></span>| <span data-ttu-id="3003e-138">[коллекция teamworkTagMember](../resources/teamworktagmember.md)</span><span class="sxs-lookup"><span data-stu-id="3003e-138">[teamworkTagMember](../resources/teamworktagmember.md) collection</span></span> |<span data-ttu-id="3003e-139">Члены группы, добавленные в тег.</span><span class="sxs-lookup"><span data-stu-id="3003e-139">Members of the team to add to the tag.</span></span> <span data-ttu-id="3003e-140">Установите свойство идентификатора пользователя каждого участника.</span><span class="sxs-lookup"><span data-stu-id="3003e-140">Set the user identifier property of each member.</span></span> <span data-ttu-id="3003e-141">Количество участников не должно быть больше 25.</span><span class="sxs-lookup"><span data-stu-id="3003e-141">Members count shouldn't be more than 25.</span></span>|



## <a name="response"></a><span data-ttu-id="3003e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3003e-142">Response</span></span>

<span data-ttu-id="3003e-143">В случае успешной работы этот метод возвращает код отклика и объект `201 Created` [teamworkTag](../resources/teamworktag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3003e-143">If successful, this method returns a `201 Created` response code and a [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3003e-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="3003e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3003e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3003e-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3003e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="3003e-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamworktag_from"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags
Content-Type: application/json

{
  "displayName": "Finance",
  "members":[
    {
        "userId":"92f6952f-61ca-4a94-8910-508a240bc167"
    },
    {
        "userId":"085d800c-b86b-4bfc-a857-9371ad1caf29"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="3003e-147">C#</span><span class="sxs-lookup"><span data-stu-id="3003e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-teamworktag-from-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3003e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3003e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamworktag-from-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3003e-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3003e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamworktag-from-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3003e-150">Java</span><span class="sxs-lookup"><span data-stu-id="3003e-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-teamworktag-from-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3003e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3003e-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Financee",
  "memberCount": 2,
  "tagType": "standard"
}
```

