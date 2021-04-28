---
title: 'группа: assignLicense'
description: Добавление или удаление лицензий в группе. Лицензии, присвоенные группе, будут назначены всем пользователям в группе.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e78e9bdcd2cc0383251a7fe6fde2b38aedee2a80
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035479"
---
# <a name="group-assignlicense"></a><span data-ttu-id="8159c-104">группа: assignLicense</span><span class="sxs-lookup"><span data-stu-id="8159c-104">group: assignLicense</span></span>

<span data-ttu-id="8159c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8159c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8159c-106">Добавление или удаление лицензий в группе.</span><span class="sxs-lookup"><span data-stu-id="8159c-106">Add or remove licenses on the group.</span></span> <span data-ttu-id="8159c-107">Лицензии, присвоенные группе, будут назначены всем пользователям в группе.</span><span class="sxs-lookup"><span data-stu-id="8159c-107">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="8159c-108">Дополнительные информацию о групповом лицензировании см. в этой [Azure Active Directory.](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="8159c-108">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="8159c-109">Чтобы получить подписки, доступные в каталоге, выполните [запрос GET subscribedSkus](../resources/subscribedsku.md).</span><span class="sxs-lookup"><span data-stu-id="8159c-109">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](../resources/subscribedsku.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8159c-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8159c-110">Permissions</span></span>
<span data-ttu-id="8159c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8159c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8159c-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8159c-113">Permission type</span></span>      | <span data-ttu-id="8159c-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8159c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8159c-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8159c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8159c-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8159c-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="8159c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8159c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8159c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8159c-118">Not supported.</span></span>    |
|<span data-ttu-id="8159c-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8159c-119">Application</span></span> | <span data-ttu-id="8159c-120">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8159c-120">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8159c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8159c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="8159c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8159c-122">Request headers</span></span>
| <span data-ttu-id="8159c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8159c-123">Header</span></span>       | <span data-ttu-id="8159c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8159c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8159c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8159c-125">Authorization</span></span>  | <span data-ttu-id="8159c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8159c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8159c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8159c-128">Content-Type</span></span>  | <span data-ttu-id="8159c-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8159c-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8159c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8159c-131">Request body</span></span>
<span data-ttu-id="8159c-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8159c-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8159c-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="8159c-133">Parameter</span></span>    | <span data-ttu-id="8159c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="8159c-134">Type</span></span>   |<span data-ttu-id="8159c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="8159c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8159c-136">addLicenses</span><span class="sxs-lookup"><span data-stu-id="8159c-136">addLicenses</span></span>|<span data-ttu-id="8159c-137">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8159c-137">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="8159c-138">Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии.</span><span class="sxs-lookup"><span data-stu-id="8159c-138">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="8159c-139">Вы можете отключить servicePlans, связанные с лицензией, установив свойство **disabledPlans** на [объекте assignedLicense.](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8159c-139">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="8159c-140">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="8159c-140">removeLicenses</span></span>|<span data-ttu-id="8159c-141">Коллекция GUID</span><span class="sxs-lookup"><span data-stu-id="8159c-141">GUID collection</span></span>|<span data-ttu-id="8159c-142">Коллекция skuIds, которые идентифицируют лицензии для удаления.</span><span class="sxs-lookup"><span data-stu-id="8159c-142">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="8159c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8159c-143">Response</span></span>

<span data-ttu-id="8159c-144">В случае успешной работы этот метод возвращает код ответа и объект целевой группы `202 Accepted` в тексте [](../resources/group.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="8159c-144">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8159c-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="8159c-145">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="8159c-146">Пример 1. Добавление лицензий в группу</span><span class="sxs-lookup"><span data-stu-id="8159c-146">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="8159c-147">В следующем примере добавляется лицензии в группу.</span><span class="sxs-lookup"><span data-stu-id="8159c-147">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="8159c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8159c-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8159c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="8159c-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
Content-type: application/json


{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```
# <a name="c"></a>[<span data-ttu-id="8159c-150">C#</span><span class="sxs-lookup"><span data-stu-id="8159c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8159c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8159c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8159c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8159c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8159c-153">Java</span><span class="sxs-lookup"><span data-stu-id="8159c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8159c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="8159c-154">Response</span></span>

<span data-ttu-id="8159c-155">Ответ — это обновленный групповой объект.</span><span class="sxs-lookup"><span data-stu-id="8159c-155">The response is the updated group object.</span></span>

><span data-ttu-id="8159c-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8159c-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/d056d009-17b3-4106-8173-cd3978ada898/directoryObjects/1ad75eeb-7e5a-4367-a493-9214d90d54d0/Microsoft.DirectoryServices.Group

{
  "id": "1ad75eeb-7e5a-4367-a493-9214d90d54d0",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-04-18T22:05:03Z",
  "securityEnabled": true,

}
```

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="8159c-157">Пример 2. Удаление лицензий из группы</span><span class="sxs-lookup"><span data-stu-id="8159c-157">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="8159c-158">В следующем примере из группы удаляются лицензии.</span><span class="sxs-lookup"><span data-stu-id="8159c-158">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="8159c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="8159c-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8159c-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="8159c-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removelicense"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
Content-type: application/json


{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```
# <a name="c"></a>[<span data-ttu-id="8159c-161">C#</span><span class="sxs-lookup"><span data-stu-id="8159c-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8159c-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8159c-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8159c-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8159c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8159c-164">Java</span><span class="sxs-lookup"><span data-stu-id="8159c-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removelicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8159c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8159c-165">Response</span></span>

<span data-ttu-id="8159c-166">Ответ — это обновленный групповой объект.</span><span class="sxs-lookup"><span data-stu-id="8159c-166">The response is the updated group object.</span></span>

><span data-ttu-id="8159c-167">**Примечание:** Объект ответа, показанный здесь, может быть сокращен для читаемости..</span><span class="sxs-lookup"><span data-stu-id="8159c-167">**Note:** The response object shown here might be shortened for readability..</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/d056d009-17b3-4106-8173-cd3978ada898/directoryObjects/1ad75eeb-7e5a-4367-a493-9214d90d54d0/Microsoft.DirectoryServices.Group


{
  "id": "1ad75eeb-7e5a-4367-a493-9214d90d54d0",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-04-18T22:05:03Z",
  "securityEnabled": true,

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

