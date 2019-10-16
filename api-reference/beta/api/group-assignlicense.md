---
title: 'Группа: Ассигнлиценсе'
description: Добавление и удаление лицензий для группы. Лицензии, назначенные группе, будут назначены всем пользователям в группе.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d014be80c99a6f9c39b0dc67f65a5b940c8cd67
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535608"
---
# <a name="group-assignlicense"></a><span data-ttu-id="7d79a-104">Группа: Ассигнлиценсе</span><span class="sxs-lookup"><span data-stu-id="7d79a-104">group: assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d79a-105">Добавление и удаление лицензий для группы.</span><span class="sxs-lookup"><span data-stu-id="7d79a-105">Add or remove licenses on the group.</span></span> <span data-ttu-id="7d79a-106">Лицензии, назначенные группе, будут назначены всем пользователям в группе.</span><span class="sxs-lookup"><span data-stu-id="7d79a-106">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="7d79a-107">Чтобы узнать больше о лицензировании на основе групп, ознакомьтесь со статьей " [Лицензирование на основе групп" в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="7d79a-107">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="7d79a-108">Чтобы получить доступ к подпискам в каталоге, выполните [запрос Get субскрибедскус](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="7d79a-108">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7d79a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d79a-109">Permissions</span></span>
<span data-ttu-id="7d79a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d79a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d79a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d79a-112">Permission type</span></span>      | <span data-ttu-id="7d79a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d79a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d79a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d79a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7d79a-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d79a-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7d79a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d79a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d79a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d79a-117">Not supported.</span></span>    |
|<span data-ttu-id="7d79a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d79a-118">Application</span></span> | <span data-ttu-id="7d79a-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d79a-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d79a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d79a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="7d79a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d79a-121">Request headers</span></span>
| <span data-ttu-id="7d79a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d79a-122">Header</span></span>       | <span data-ttu-id="7d79a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7d79a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7d79a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d79a-124">Authorization</span></span>  | <span data-ttu-id="7d79a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d79a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7d79a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d79a-127">Content-Type</span></span>  | <span data-ttu-id="7d79a-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d79a-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7d79a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d79a-130">Request body</span></span>
<span data-ttu-id="7d79a-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7d79a-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7d79a-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="7d79a-132">Parameter</span></span>    | <span data-ttu-id="7d79a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="7d79a-133">Type</span></span>   |<span data-ttu-id="7d79a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="7d79a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d79a-135">addLicenses</span><span class="sxs-lookup"><span data-stu-id="7d79a-135">addLicenses</span></span>|<span data-ttu-id="7d79a-136">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7d79a-136">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="7d79a-137">Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии.</span><span class="sxs-lookup"><span data-stu-id="7d79a-137">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="7d79a-138">Вы можете отключить Сервицепланс, связанные с лицензией, задав свойство **дисабледпланс** для объекта [коллекция assignedlicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="7d79a-138">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="7d79a-139">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="7d79a-139">removeLicenses</span></span>|<span data-ttu-id="7d79a-140">Коллекция GUID</span><span class="sxs-lookup"><span data-stu-id="7d79a-140">GUID collection</span></span>|<span data-ttu-id="7d79a-141">Коллекция Скуидс, идентифицирующая лицензии, которые требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="7d79a-141">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="7d79a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d79a-142">Response</span></span>

<span data-ttu-id="7d79a-143">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и целевой объект [Group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d79a-143">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d79a-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="7d79a-144">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="7d79a-145">Пример 1: Добавление лицензий в группу</span><span class="sxs-lookup"><span data-stu-id="7d79a-145">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="7d79a-146">В следующем примере в группу добавляются лицензии.</span><span class="sxs-lookup"><span data-stu-id="7d79a-146">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="7d79a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d79a-147">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7d79a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d79a-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7d79a-149">C#</span><span class="sxs-lookup"><span data-stu-id="7d79a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d79a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d79a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7d79a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d79a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d79a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d79a-152">Response</span></span>
<span data-ttu-id="7d79a-153">Отклик — обновленный объект Group.</span><span class="sxs-lookup"><span data-stu-id="7d79a-153">The response is the updated group object.</span></span>

><span data-ttu-id="7d79a-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7d79a-154">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7d79a-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d79a-155">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="7d79a-156">Пример 2: Удаление лицензий из группы</span><span class="sxs-lookup"><span data-stu-id="7d79a-156">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="7d79a-157">В следующем примере удаляются лицензии из группы.</span><span class="sxs-lookup"><span data-stu-id="7d79a-157">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="7d79a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d79a-158">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7d79a-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d79a-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7d79a-160">C#</span><span class="sxs-lookup"><span data-stu-id="7d79a-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d79a-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d79a-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7d79a-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d79a-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d79a-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d79a-163">Response</span></span>
<span data-ttu-id="7d79a-164">Отклик — обновленный объект Group.</span><span class="sxs-lookup"><span data-stu-id="7d79a-164">The response is the updated group object.</span></span>

><span data-ttu-id="7d79a-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7d79a-165">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7d79a-166">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d79a-166">All the properties will be returned from an actual call..</span></span>
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
