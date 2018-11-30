---
title: Список групп
description: Список всех групп, доступных в организации, в том числе из функции "Группы Office 365".
ms.openlocfilehash: 2b46891a7570a831cd1b38ae29915e59475e8540
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075034"
---
# <a name="list-groups"></a><span data-ttu-id="75865-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="75865-103">List groups</span></span>

> <span data-ttu-id="75865-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="75865-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75865-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75865-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75865-p102">Список всех групп, доступных в организации, в том числе из функции "Группы Office 365". Возвращаются [свойства по умолчанию](../api/group-get.md#default-properties) для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="75865-p102">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="75865-108">Чтобы получить только результаты из функции "Группы Office 365" (т. н. единые группы), примените фильтр **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="75865-108">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="75865-109">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="75865-109">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="75865-110">Чтобы вернуть группы, содержащие элементы с ошибками лицензии, используйте параметр **$filter** запроса:</span><span class="sxs-lookup"><span data-stu-id="75865-110">To return groups containing members with license errors, use the **$filter** query parameter:</span></span> 

```http 
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true 
```
## <a name="permissions"></a><span data-ttu-id="75865-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75865-111">Permissions</span></span>
<span data-ttu-id="75865-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75865-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75865-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75865-114">Permission type</span></span>      | <span data-ttu-id="75865-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75865-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75865-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75865-116">Delegated (work or school account)</span></span> | <span data-ttu-id="75865-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75865-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="75865-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75865-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75865-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75865-119">Not supported.</span></span>    |
|<span data-ttu-id="75865-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75865-120">Application</span></span> | <span data-ttu-id="75865-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75865-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75865-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75865-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75865-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75865-123">Optional query parameters</span></span>
<span data-ttu-id="75865-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="75865-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75865-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75865-125">Request headers</span></span>
| <span data-ttu-id="75865-126">Имя</span><span class="sxs-lookup"><span data-stu-id="75865-126">Name</span></span>       | <span data-ttu-id="75865-127">Тип</span><span class="sxs-lookup"><span data-stu-id="75865-127">Type</span></span> | <span data-ttu-id="75865-128">Описание</span><span class="sxs-lookup"><span data-stu-id="75865-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="75865-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="75865-129">Authorization</span></span>  | <span data-ttu-id="75865-130">string</span><span class="sxs-lookup"><span data-stu-id="75865-130">string</span></span>  | <span data-ttu-id="75865-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75865-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75865-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75865-133">Request body</span></span>
<span data-ttu-id="75865-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75865-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75865-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="75865-135">Response</span></span>
<span data-ttu-id="75865-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75865-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75865-137">Пример</span><span class="sxs-lookup"><span data-stu-id="75865-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="75865-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="75865-138">Request</span></span>
<span data-ttu-id="75865-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75865-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response"></a><span data-ttu-id="75865-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="75865-140">Response</span></span>
<span data-ttu-id="75865-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75865-141">The following is an example of the response.</span></span>
><span data-ttu-id="75865-142">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="75865-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="75865-143">[Свойства по умолчанию](../api/group-get.md#default-properties) возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="75865-143">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
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
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
