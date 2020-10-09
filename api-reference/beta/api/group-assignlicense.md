---
title: 'Группа: Ассигнлиценсе'
description: Добавление и удаление лицензий для группы. Лицензии, назначенные группе, будут назначены всем пользователям в группе.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9d8a4632f95e321f37583ac7df62f953694e3756
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403145"
---
# <a name="group-assignlicense"></a><span data-ttu-id="c87ae-104">Группа: Ассигнлиценсе</span><span class="sxs-lookup"><span data-stu-id="c87ae-104">group: assignLicense</span></span>

<span data-ttu-id="c87ae-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c87ae-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c87ae-106">Добавление и удаление лицензий для группы.</span><span class="sxs-lookup"><span data-stu-id="c87ae-106">Add or remove licenses on the group.</span></span> <span data-ttu-id="c87ae-107">Лицензии, назначенные группе, будут назначены всем пользователям в группе.</span><span class="sxs-lookup"><span data-stu-id="c87ae-107">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="c87ae-108">Чтобы узнать больше о лицензировании на основе групп, ознакомьтесь со статьей " [Лицензирование на основе групп" в Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="c87ae-108">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="c87ae-109">Чтобы получить доступ к подпискам в каталоге, выполните [запрос Get субскрибедскус](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="c87ae-109">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c87ae-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c87ae-110">Permissions</span></span>
<span data-ttu-id="c87ae-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c87ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c87ae-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c87ae-113">Permission type</span></span>      | <span data-ttu-id="c87ae-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c87ae-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c87ae-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c87ae-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c87ae-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87ae-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c87ae-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c87ae-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c87ae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c87ae-118">Not supported.</span></span>    |
|<span data-ttu-id="c87ae-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c87ae-119">Application</span></span> | <span data-ttu-id="c87ae-120">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87ae-120">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c87ae-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c87ae-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="c87ae-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c87ae-122">Request headers</span></span>
| <span data-ttu-id="c87ae-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c87ae-123">Header</span></span>       | <span data-ttu-id="c87ae-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c87ae-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c87ae-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c87ae-125">Authorization</span></span>  | <span data-ttu-id="c87ae-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c87ae-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c87ae-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c87ae-128">Content-Type</span></span>  | <span data-ttu-id="c87ae-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c87ae-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c87ae-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c87ae-131">Request body</span></span>
<span data-ttu-id="c87ae-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c87ae-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c87ae-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="c87ae-133">Parameter</span></span>    | <span data-ttu-id="c87ae-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c87ae-134">Type</span></span>   |<span data-ttu-id="c87ae-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c87ae-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c87ae-136">addLicenses</span><span class="sxs-lookup"><span data-stu-id="c87ae-136">addLicenses</span></span>|<span data-ttu-id="c87ae-137">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c87ae-137">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="c87ae-138">Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии.</span><span class="sxs-lookup"><span data-stu-id="c87ae-138">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="c87ae-139">Вы можете отключить Сервицепланс, связанные с лицензией, задав свойство **дисабледпланс** для объекта [коллекция assignedlicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="c87ae-139">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="c87ae-140">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="c87ae-140">removeLicenses</span></span>|<span data-ttu-id="c87ae-141">Коллекция GUID</span><span class="sxs-lookup"><span data-stu-id="c87ae-141">GUID collection</span></span>|<span data-ttu-id="c87ae-142">Коллекция Скуидс, идентифицирующая лицензии, которые требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="c87ae-142">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="c87ae-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c87ae-143">Response</span></span>

<span data-ttu-id="c87ae-144">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и целевой объект [Group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c87ae-144">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c87ae-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="c87ae-145">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="c87ae-146">Пример 1: Добавление лицензий в группу</span><span class="sxs-lookup"><span data-stu-id="c87ae-146">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="c87ae-147">В следующем примере в группу добавляются лицензии.</span><span class="sxs-lookup"><span data-stu-id="c87ae-147">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="c87ae-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c87ae-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c87ae-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c87ae-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
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
# <a name="c"></a>[<span data-ttu-id="c87ae-150">C#</span><span class="sxs-lookup"><span data-stu-id="c87ae-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c87ae-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c87ae-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c87ae-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c87ae-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c87ae-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c87ae-153">Response</span></span>
<span data-ttu-id="c87ae-154">Отклик — обновленный объект Group.</span><span class="sxs-lookup"><span data-stu-id="c87ae-154">The response is the updated group object.</span></span>

><span data-ttu-id="c87ae-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c87ae-155">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c87ae-156">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c87ae-156">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="c87ae-157">Пример 2: Удаление лицензий из группы</span><span class="sxs-lookup"><span data-stu-id="c87ae-157">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="c87ae-158">В следующем примере удаляются лицензии из группы.</span><span class="sxs-lookup"><span data-stu-id="c87ae-158">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="c87ae-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="c87ae-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c87ae-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="c87ae-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removelicense"
}-->

```http
POST https://graph.microsoft.com/beta/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
Content-type: application/json


{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```
# <a name="c"></a>[<span data-ttu-id="c87ae-161">C#</span><span class="sxs-lookup"><span data-stu-id="c87ae-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c87ae-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c87ae-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c87ae-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c87ae-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c87ae-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="c87ae-164">Response</span></span>
<span data-ttu-id="c87ae-165">Отклик — обновленный объект Group.</span><span class="sxs-lookup"><span data-stu-id="c87ae-165">The response is the updated group object.</span></span>

><span data-ttu-id="c87ae-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c87ae-166">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c87ae-167">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c87ae-167">All the properties will be returned from an actual call..</span></span>
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