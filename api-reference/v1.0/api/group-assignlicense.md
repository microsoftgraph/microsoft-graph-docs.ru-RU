---
title: 'Группа: Ассигнлиценсе'
description: Добавление и удаление лицензий для группы. Лицензии, назначенные группе, будут назначены всем пользователям в группе.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 43fa0a9346ccecc704c49ffc7528b71a58763fbc
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865785"
---
# <a name="group-assignlicense"></a><span data-ttu-id="1dd7e-104">Группа: Ассигнлиценсе</span><span class="sxs-lookup"><span data-stu-id="1dd7e-104">group: assignLicense</span></span>

<span data-ttu-id="1dd7e-105">Добавление и удаление лицензий для группы.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-105">Add or remove licenses on the group.</span></span> <span data-ttu-id="1dd7e-106">Лицензии, назначенные группе, будут назначены всем пользователям в группе.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-106">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="1dd7e-107">Чтобы узнать больше о лицензировании на основе групп, ознакомьтесь со статьей " [Лицензирование на основе групп" в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="1dd7e-107">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="1dd7e-108">Чтобы получить доступ к подпискам в каталоге, выполните [запрос Get субскрибедскус](../resources/subscribedsku.md).</span><span class="sxs-lookup"><span data-stu-id="1dd7e-108">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](../resources/subscribedsku.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1dd7e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dd7e-109">Permissions</span></span>
<span data-ttu-id="1dd7e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dd7e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dd7e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dd7e-112">Permission type</span></span>      | <span data-ttu-id="1dd7e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dd7e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dd7e-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dd7e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1dd7e-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd7e-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="1dd7e-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dd7e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd7e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-117">Not supported.</span></span>    |
|<span data-ttu-id="1dd7e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dd7e-118">Application</span></span> | <span data-ttu-id="1dd7e-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd7e-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dd7e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dd7e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="1dd7e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dd7e-121">Request headers</span></span>
| <span data-ttu-id="1dd7e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1dd7e-122">Header</span></span>       | <span data-ttu-id="1dd7e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1dd7e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1dd7e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dd7e-124">Authorization</span></span>  | <span data-ttu-id="1dd7e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1dd7e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1dd7e-127">Content-Type</span></span>  | <span data-ttu-id="1dd7e-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1dd7e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dd7e-130">Request body</span></span>
<span data-ttu-id="1dd7e-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1dd7e-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="1dd7e-132">Parameter</span></span>    | <span data-ttu-id="1dd7e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1dd7e-133">Type</span></span>   |<span data-ttu-id="1dd7e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1dd7e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dd7e-135">addLicenses</span><span class="sxs-lookup"><span data-stu-id="1dd7e-135">addLicenses</span></span>|<span data-ttu-id="1dd7e-136">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1dd7e-136">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="1dd7e-137">Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-137">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="1dd7e-138">Вы можете отключить Сервицепланс, связанные с лицензией, задав свойство **дисабледпланс** для объекта [коллекция assignedlicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1dd7e-138">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="1dd7e-139">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="1dd7e-139">removeLicenses</span></span>|<span data-ttu-id="1dd7e-140">Коллекция GUID</span><span class="sxs-lookup"><span data-stu-id="1dd7e-140">GUID collection</span></span>|<span data-ttu-id="1dd7e-141">Коллекция Скуидс, идентифицирующая лицензии, которые требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-141">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="1dd7e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dd7e-142">Response</span></span>

<span data-ttu-id="1dd7e-143">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и целевой объект [Group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-143">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1dd7e-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="1dd7e-144">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="1dd7e-145">Пример 1: Добавление лицензий в группу</span><span class="sxs-lookup"><span data-stu-id="1dd7e-145">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="1dd7e-146">В следующем примере в группу добавляются лицензии.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-146">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="1dd7e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dd7e-147">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1dd7e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd7e-148">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="1dd7e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dd7e-149">Response</span></span>

<span data-ttu-id="1dd7e-150">Отклик — обновленный объект Group.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-150">The response is the updated group object.</span></span>

><span data-ttu-id="1dd7e-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1dd7e-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-152">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="1dd7e-153">Пример 2: Удаление лицензий из группы</span><span class="sxs-lookup"><span data-stu-id="1dd7e-153">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="1dd7e-154">В следующем примере удаляются лицензии из группы.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-154">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="1dd7e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dd7e-155">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1dd7e-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd7e-156">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="1dd7e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dd7e-157">Response</span></span>

<span data-ttu-id="1dd7e-158">Отклик — обновленный объект Group.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-158">The response is the updated group object.</span></span>

><span data-ttu-id="1dd7e-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1dd7e-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dd7e-160">All the properties will be returned from an actual call..</span></span>
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
