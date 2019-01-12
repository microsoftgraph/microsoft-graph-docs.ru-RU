---
title: Список групп
description: Список всех групп, доступных в организации, в том числе из функции "Группы Office 365".
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 05d3872fbc376933a0ff2fe772a79239e4d62928
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955172"
---
# <a name="list-groups"></a><span data-ttu-id="e125a-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="e125a-103">List groups</span></span>
<span data-ttu-id="e125a-p101">Список всех групп, доступных в организации, в том числе из функции "Группы Office 365". Возвращаются [свойства по умолчанию](../api/group-get.md#default-properties) для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="e125a-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="e125a-106">Чтобы получить только результаты из функции "Группы Office 365" (т. н. единые группы), примените фильтр **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="e125a-106">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="e125a-107">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="e125a-107">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

## <a name="permissions"></a><span data-ttu-id="e125a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e125a-108">Permissions</span></span>
<span data-ttu-id="e125a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e125a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e125a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e125a-111">Permission type</span></span>      | <span data-ttu-id="e125a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e125a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e125a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e125a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e125a-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e125a-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e125a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e125a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e125a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e125a-116">Not supported.</span></span>    |
|<span data-ttu-id="e125a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e125a-117">Application</span></span> | <span data-ttu-id="e125a-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e125a-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e125a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e125a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e125a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e125a-120">Optional query parameters</span></span>
<span data-ttu-id="e125a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e125a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e125a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e125a-122">Request headers</span></span>
| <span data-ttu-id="e125a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e125a-123">Name</span></span>       | <span data-ttu-id="e125a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e125a-124">Type</span></span> | <span data-ttu-id="e125a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e125a-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e125a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e125a-126">Authorization</span></span>  | <span data-ttu-id="e125a-127">строка</span><span class="sxs-lookup"><span data-stu-id="e125a-127">string</span></span>  | <span data-ttu-id="e125a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e125a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e125a-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e125a-130">Request body</span></span>
<span data-ttu-id="e125a-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e125a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e125a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e125a-132">Response</span></span>
<span data-ttu-id="e125a-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e125a-133">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e125a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e125a-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e125a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e125a-135">Request</span></span>
<span data-ttu-id="e125a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e125a-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="e125a-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e125a-137">Response</span></span>
<span data-ttu-id="e125a-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e125a-138">The following is an example of the response.</span></span>

><span data-ttu-id="e125a-139">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="e125a-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e125a-140">[Свойства по умолчанию](../api/group-get.md#default-properties) возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e125a-140">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

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
