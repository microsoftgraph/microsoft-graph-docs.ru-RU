---
title: Получение удаленного элемента
description: Получение свойств недавно удаленного элемента.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e6e3d70e53908133f4b195d54d8bc0f429e9ef4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273096"
---
# <a name="get-deleted-item"></a><span data-ttu-id="8578c-103">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="8578c-103">Get deleted item</span></span>

<span data-ttu-id="8578c-104">Получение свойств недавно [удаленного элемента](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="8578c-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="8578c-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="8578c-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="8578c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8578c-106">Permissions</span></span>
<span data-ttu-id="8578c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8578c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="8578c-109">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="8578c-109">For users:</span></span>

|<span data-ttu-id="8578c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8578c-110">Permission type</span></span>      | <span data-ttu-id="8578c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8578c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8578c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8578c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8578c-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8578c-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="8578c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8578c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8578c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8578c-115">Not supported.</span></span> |
|<span data-ttu-id="8578c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8578c-116">Application</span></span> | <span data-ttu-id="8578c-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8578c-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="8578c-118">Для групп:</span><span class="sxs-lookup"><span data-stu-id="8578c-118">For groups:</span></span>

|<span data-ttu-id="8578c-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8578c-119">Permission type</span></span>      | <span data-ttu-id="8578c-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8578c-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8578c-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8578c-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8578c-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8578c-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8578c-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8578c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8578c-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8578c-124">Not supported.</span></span>    |
|<span data-ttu-id="8578c-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8578c-125">Application</span></span> | <span data-ttu-id="8578c-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8578c-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8578c-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8578c-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8578c-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8578c-128">Optional query parameters</span></span>
<span data-ttu-id="8578c-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8578c-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8578c-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8578c-130">Request headers</span></span>
| <span data-ttu-id="8578c-131">Имя</span><span class="sxs-lookup"><span data-stu-id="8578c-131">Name</span></span>      |<span data-ttu-id="8578c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8578c-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8578c-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8578c-133">Authorization</span></span>  | <span data-ttu-id="8578c-134">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="8578c-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="8578c-135">Accept</span><span class="sxs-lookup"><span data-stu-id="8578c-135">Accept</span></span>  | <span data-ttu-id="8578c-136">application/json</span><span class="sxs-lookup"><span data-stu-id="8578c-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8578c-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8578c-137">Request body</span></span>
<span data-ttu-id="8578c-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8578c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8578c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8578c-139">Response</span></span>

<span data-ttu-id="8578c-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8578c-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8578c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8578c-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8578c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8578c-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="8578c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8578c-143">Response</span></span>
<span data-ttu-id="8578c-p102">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8578c-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8578c-146">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="8578c-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8578c-147">C#</span><span class="sxs-lookup"><span data-stu-id="8578c-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8578c-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="8578c-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8578c-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8578c-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
