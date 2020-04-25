---
title: Создание канала
description: Создание канала в Microsoft Team, как указано в тексте запроса.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c83511faf6034caab1c55ec394c3e53394011097
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806125"
---
# <a name="create-channel"></a><span data-ttu-id="9ffda-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="9ffda-103">Create Channel</span></span>

<span data-ttu-id="9ffda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ffda-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="9ffda-105">Создание [канала](../resources/channel.md) в Microsoft Team, как указано в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="9ffda-105">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="9ffda-106">**Примечание**. Существует известная проблема с разрешениями для приложений и этим API.</span><span class="sxs-lookup"><span data-stu-id="9ffda-106">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="9ffda-107">Дополнительные сведения см. в [списке известных проблем](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="9ffda-107">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ffda-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ffda-108">Permissions</span></span>
<span data-ttu-id="9ffda-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ffda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9ffda-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ffda-111">Permission type</span></span>      | <span data-ttu-id="9ffda-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ffda-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ffda-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ffda-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9ffda-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ffda-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ffda-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ffda-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ffda-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ffda-116">Not supported.</span></span>    |
|<span data-ttu-id="9ffda-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ffda-117">Application</span></span> | <span data-ttu-id="9ffda-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ffda-118">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="9ffda-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="9ffda-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9ffda-120">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="9ffda-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9ffda-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ffda-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="9ffda-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ffda-122">Request headers</span></span>
| <span data-ttu-id="9ffda-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ffda-123">Header</span></span>       | <span data-ttu-id="9ffda-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9ffda-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ffda-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ffda-125">Authorization</span></span>  | <span data-ttu-id="9ffda-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ffda-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ffda-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ffda-128">Content-Type</span></span>  | <span data-ttu-id="9ffda-129">application/json</span><span class="sxs-lookup"><span data-stu-id="9ffda-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ffda-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ffda-130">Request body</span></span>
<span data-ttu-id="9ffda-131">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ffda-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9ffda-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ffda-132">Response</span></span>

<span data-ttu-id="9ffda-133">В случае успеха этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ffda-133">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ffda-134">Пример</span><span class="sxs-lookup"><span data-stu-id="9ffda-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ffda-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ffda-135">Request</span></span>
<span data-ttu-id="9ffda-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ffda-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ffda-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ffda-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
# <a name="c"></a>[<span data-ttu-id="9ffda-138">C#</span><span class="sxs-lookup"><span data-stu-id="9ffda-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ffda-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ffda-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ffda-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ffda-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ffda-141">Java</span><span class="sxs-lookup"><span data-stu-id="9ffda-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9ffda-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ffda-142">Response</span></span>
<span data-ttu-id="9ffda-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ffda-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
