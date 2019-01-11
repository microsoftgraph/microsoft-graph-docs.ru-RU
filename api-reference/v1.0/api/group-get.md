---
title: Вывод группы
description: Получение свойств и связей объекта группы.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 554a0b6bf6fcb4afb2a57f12e2c814cf5fa57951
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873411"
---
# <a name="get-group"></a><span data-ttu-id="7511c-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="7511c-103">Get group</span></span>
<span data-ttu-id="7511c-104">Получение свойств и связей объекта группы.</span><span class="sxs-lookup"><span data-stu-id="7511c-104">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="7511c-105">Свойства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="7511c-105">Default properties</span></span>

<span data-ttu-id="7511c-p101">Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении групп или выводе списка групп. Это подмножество всех доступных свойств.</span><span class="sxs-lookup"><span data-stu-id="7511c-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="7511c-108">description</span><span class="sxs-lookup"><span data-stu-id="7511c-108">description</span></span>
* <span data-ttu-id="7511c-109">displayName</span><span class="sxs-lookup"><span data-stu-id="7511c-109">displayName</span></span>
* <span data-ttu-id="7511c-110">groupTypes</span><span class="sxs-lookup"><span data-stu-id="7511c-110">groupTypes</span></span>
* <span data-ttu-id="7511c-111">id</span><span class="sxs-lookup"><span data-stu-id="7511c-111">id</span></span>
* <span data-ttu-id="7511c-112">mail</span><span class="sxs-lookup"><span data-stu-id="7511c-112">mail</span></span>
* <span data-ttu-id="7511c-113">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7511c-113">mailEnabled</span></span>
* <span data-ttu-id="7511c-114">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7511c-114">mailNickname</span></span>
* <span data-ttu-id="7511c-115">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7511c-115">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="7511c-116">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="7511c-116">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="7511c-117">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="7511c-117">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="7511c-118">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="7511c-118">proxyAddresses</span></span>
* <span data-ttu-id="7511c-119">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7511c-119">securityEnabled</span></span>
* <span data-ttu-id="7511c-120">visibility</span><span class="sxs-lookup"><span data-stu-id="7511c-120">visibility</span></span>

<span data-ttu-id="7511c-121">По умолчанию следующие свойства групп не возвращаются:</span><span class="sxs-lookup"><span data-stu-id="7511c-121">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="7511c-122">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="7511c-122">allowExternalSenders</span></span>
* <span data-ttu-id="7511c-123">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="7511c-123">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="7511c-124">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="7511c-124">isSubscribedByMail</span></span>
* <span data-ttu-id="7511c-125">unseenCount</span><span class="sxs-lookup"><span data-stu-id="7511c-125">unseenCount</span></span>

<span data-ttu-id="7511c-p102">Для их получения используйте параметр запроса **$select**. Примеры.</span><span class="sxs-lookup"><span data-stu-id="7511c-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="7511c-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7511c-128">Permissions</span></span>
<span data-ttu-id="7511c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7511c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7511c-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7511c-131">Permission type</span></span>      | <span data-ttu-id="7511c-132">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7511c-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7511c-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7511c-133">Delegated (work or school account)</span></span> | <span data-ttu-id="7511c-134">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7511c-134">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7511c-135">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7511c-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7511c-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7511c-136">Not supported.</span></span>    |
|<span data-ttu-id="7511c-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7511c-137">Application</span></span> | <span data-ttu-id="7511c-138">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7511c-138">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7511c-139">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7511c-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7511c-140">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7511c-140">Optional query parameters</span></span>
<span data-ttu-id="7511c-141">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7511c-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7511c-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7511c-142">Request headers</span></span>
| <span data-ttu-id="7511c-143">Имя</span><span class="sxs-lookup"><span data-stu-id="7511c-143">Name</span></span>       | <span data-ttu-id="7511c-144">Тип</span><span class="sxs-lookup"><span data-stu-id="7511c-144">Type</span></span> | <span data-ttu-id="7511c-145">Описание</span><span class="sxs-lookup"><span data-stu-id="7511c-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7511c-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="7511c-146">Authorization</span></span>  | <span data-ttu-id="7511c-147">string</span><span class="sxs-lookup"><span data-stu-id="7511c-147">string</span></span>  | <span data-ttu-id="7511c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7511c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7511c-150">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7511c-150">Request body</span></span>
<span data-ttu-id="7511c-151">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7511c-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7511c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7511c-152">Response</span></span>
<span data-ttu-id="7511c-153">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7511c-153">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7511c-154">Пример</span><span class="sxs-lookup"><span data-stu-id="7511c-154">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7511c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="7511c-155">Request</span></span>
<span data-ttu-id="7511c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7511c-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="7511c-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="7511c-157">Response</span></span>
<span data-ttu-id="7511c-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7511c-158">The following is an example of the response.</span></span>

><span data-ttu-id="7511c-159">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="7511c-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7511c-160">При фактическом вызове будут возвращены все свойства по умолчанию, как описано ранее.</span><span class="sxs-lookup"><span data-stu-id="7511c-160">The default properties will be returned from an actual call, as described before.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
