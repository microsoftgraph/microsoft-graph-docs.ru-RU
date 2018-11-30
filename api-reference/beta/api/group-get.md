---
title: Вывод группы
description: Получение свойств и связей объекта группы.
ms.openlocfilehash: 5bd4635e3eb9004a33c60fee0c802e77fa15a709
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082299"
---
# <a name="get-group"></a><span data-ttu-id="a5957-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="a5957-103">Get group</span></span>

> <span data-ttu-id="a5957-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5957-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5957-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5957-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5957-106">Получите свойства и связи объекта [группы](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="a5957-106">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="a5957-107">Свойства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="a5957-107">Default properties</span></span>

<span data-ttu-id="a5957-p102">Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении групп или выводе списка групп. Это подмножество всех доступных свойств.</span><span class="sxs-lookup"><span data-stu-id="a5957-p102">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="a5957-110">classification</span><span class="sxs-lookup"><span data-stu-id="a5957-110">classification</span></span>
* <span data-ttu-id="a5957-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5957-111">createdDateTime</span></span>
* <span data-ttu-id="a5957-112">description</span><span class="sxs-lookup"><span data-stu-id="a5957-112">description</span></span>
* <span data-ttu-id="a5957-113">displayName</span><span class="sxs-lookup"><span data-stu-id="a5957-113">displayName</span></span>
* <span data-ttu-id="a5957-114">groupTypes</span><span class="sxs-lookup"><span data-stu-id="a5957-114">groupTypes</span></span>
* <span data-ttu-id="a5957-115">id</span><span class="sxs-lookup"><span data-stu-id="a5957-115">id</span></span>
* <span data-ttu-id="a5957-116">mail</span><span class="sxs-lookup"><span data-stu-id="a5957-116">mail</span></span>
* <span data-ttu-id="a5957-117">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="a5957-117">mailEnabled</span></span>
* <span data-ttu-id="a5957-118">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a5957-118">mailNickname</span></span>
* <span data-ttu-id="a5957-119">membershipRule</span><span class="sxs-lookup"><span data-stu-id="a5957-119">membershipRule</span></span>
* <span data-ttu-id="a5957-120">membershipRuleProcessingState</span><span class="sxs-lookup"><span data-stu-id="a5957-120">membershipRuleProcessingState</span></span>
* <span data-ttu-id="a5957-121">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a5957-121">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="a5957-122">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="a5957-122">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="a5957-123">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="a5957-123">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="a5957-124">preferredLanguage - не поддерживается; значение для этого свойства не может быть набора и возвращает `null` при вызове.</span><span class="sxs-lookup"><span data-stu-id="a5957-124">preferredLanguage - Not supported; a value for this property cannot be set and returns `null` when called.</span></span>
* <span data-ttu-id="a5957-125">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="a5957-125">proxyAddresses</span></span>
* <span data-ttu-id="a5957-126">renewedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5957-126">renewedDateTime</span></span>
* <span data-ttu-id="a5957-127">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="a5957-127">securityEnabled</span></span>
* <span data-ttu-id="a5957-128">темы</span><span class="sxs-lookup"><span data-stu-id="a5957-128">theme</span></span>
* <span data-ttu-id="a5957-129">visibility</span><span class="sxs-lookup"><span data-stu-id="a5957-129">visibility</span></span>

<span data-ttu-id="a5957-130">По умолчанию следующие свойства групп не возвращаются:</span><span class="sxs-lookup"><span data-stu-id="a5957-130">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="a5957-131">accessType</span><span class="sxs-lookup"><span data-stu-id="a5957-131">accessType</span></span>
* <span data-ttu-id="a5957-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="a5957-132">allowExternalSenders</span></span>
* <span data-ttu-id="a5957-133">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="a5957-133">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="a5957-134">hasMembersWithLicenseErrors</span><span class="sxs-lookup"><span data-stu-id="a5957-134">hasMembersWithLicenseErrors</span></span>
* <span data-ttu-id="a5957-135">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="a5957-135">isSubscribedByMail</span></span>
* <span data-ttu-id="a5957-136">isFavorite</span><span class="sxs-lookup"><span data-stu-id="a5957-136">isFavorite</span></span>
* <span data-ttu-id="a5957-137">unseenConversationsCount</span><span class="sxs-lookup"><span data-stu-id="a5957-137">unseenConversationsCount</span></span>
* <span data-ttu-id="a5957-138">unseenCount</span><span class="sxs-lookup"><span data-stu-id="a5957-138">unseenCount</span></span>
* <span data-ttu-id="a5957-139">unseenMessagesCount</span><span class="sxs-lookup"><span data-stu-id="a5957-139">unseenMessagesCount</span></span>

<span data-ttu-id="a5957-140">Для получения этих свойств (за исключением **isFavorite** и **hasMembersWithLicenseErrors**), воспользуйтесь `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="a5957-140">To get these properties (except **isFavorite** and **hasMembersWithLicenseErrors**), use the `$select` query parameter.</span></span> <span data-ttu-id="a5957-141">Ниже представлены примеры.</span><span class="sxs-lookup"><span data-stu-id="a5957-141">The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```

<span data-ttu-id="a5957-142">Чтобы вернуть группы, содержащие элементы с ошибками лицензии, используйте параметр **$filter** запроса:</span><span class="sxs-lookup"><span data-stu-id="a5957-142">To return groups containing members with license errors, use the **$filter** query parameter:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true
```

<span data-ttu-id="a5957-143">Поскольку **группы** ресурсов поддерживает [расширения](/graph/extensibility-overview), вы также можете использовать `GET` операции для получения данных расширения и настраиваемых свойств в экземпляре **группы** .</span><span class="sxs-lookup"><span data-stu-id="a5957-143">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5957-144">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5957-144">Permissions</span></span>
<span data-ttu-id="a5957-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5957-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5957-147">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5957-147">Permission type</span></span>      | <span data-ttu-id="a5957-148">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5957-148">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5957-149">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5957-149">Delegated (work or school account)</span></span> | <span data-ttu-id="a5957-150">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5957-150">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5957-151">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5957-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5957-152">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5957-152">Not supported.</span></span>    |
|<span data-ttu-id="a5957-153">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5957-153">Application</span></span> | <span data-ttu-id="a5957-154">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5957-154">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5957-155">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5957-155">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a5957-156">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5957-156">Optional query parameters</span></span>
<span data-ttu-id="a5957-157">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a5957-157">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5957-158">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5957-158">Request headers</span></span>
| <span data-ttu-id="a5957-159">Имя</span><span class="sxs-lookup"><span data-stu-id="a5957-159">Name</span></span>       | <span data-ttu-id="a5957-160">Тип</span><span class="sxs-lookup"><span data-stu-id="a5957-160">Type</span></span> | <span data-ttu-id="a5957-161">Описание</span><span class="sxs-lookup"><span data-stu-id="a5957-161">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5957-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5957-162">Authorization</span></span>  | <span data-ttu-id="a5957-163">string</span><span class="sxs-lookup"><span data-stu-id="a5957-163">string</span></span>  | <span data-ttu-id="a5957-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5957-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5957-166">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5957-166">Request body</span></span>
<span data-ttu-id="a5957-167">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5957-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5957-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5957-168">Response</span></span>
<span data-ttu-id="a5957-169">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5957-169">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5957-170">Пример</span><span class="sxs-lookup"><span data-stu-id="a5957-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5957-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5957-171">Request</span></span>
<span data-ttu-id="a5957-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5957-172">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="a5957-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5957-173">Response</span></span>
<span data-ttu-id="a5957-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5957-174">The following is an example of the response.</span></span> 
><span data-ttu-id="a5957-175">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="a5957-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a5957-176">При фактическом вызове будут возвращены все свойства по умолчанию, как описано ранее.</span><span class="sxs-lookup"><span data-stu-id="a5957-176">The default properties will be returned from an actual call, as described before.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

## <a name="see-also"></a><span data-ttu-id="a5957-177">См. также</span><span class="sxs-lookup"><span data-stu-id="a5957-177">See also</span></span>

- [<span data-ttu-id="a5957-178">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a5957-178">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a5957-179">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="a5957-179">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a5957-180">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="a5957-180">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
