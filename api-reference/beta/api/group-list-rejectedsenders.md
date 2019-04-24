---
title: Список rejectedSenders
description: 'Получение пользователей или групп из списка rejectedSenders для данной группы. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5dd03644b91ad847b61350f48792afdaa087d59b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502066"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="8c34f-103">Список rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="8c34f-103">List rejectedSenders</span></span>
<span data-ttu-id="8c34f-104">Получение пользователей или групп из списка rejectedSenders для данной группы.</span><span class="sxs-lookup"><span data-stu-id="8c34f-104">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="8c34f-p101">Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса GET). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="8c34f-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c34f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c34f-107">Permissions</span></span>
<span data-ttu-id="8c34f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c34f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c34f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c34f-110">Permission type</span></span>      | <span data-ttu-id="8c34f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c34f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c34f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c34f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c34f-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c34f-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c34f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c34f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c34f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c34f-115">Not supported.</span></span>    |
|<span data-ttu-id="8c34f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c34f-116">Application</span></span> | <span data-ttu-id="8c34f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c34f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c34f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c34f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c34f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c34f-119">Optional query parameters</span></span>
<span data-ttu-id="8c34f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8c34f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c34f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c34f-121">Request headers</span></span>
| <span data-ttu-id="8c34f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c34f-122">Header</span></span>       | <span data-ttu-id="8c34f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8c34f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c34f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c34f-124">Authorization</span></span>  | <span data-ttu-id="8c34f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c34f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c34f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c34f-127">Request body</span></span>
<span data-ttu-id="8c34f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c34f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c34f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c34f-129">Response</span></span>
<span data-ttu-id="8c34f-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c34f-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c34f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8c34f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8c34f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c34f-132">Request</span></span>
<span data-ttu-id="8c34f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c34f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="8c34f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c34f-134">Response</span></span>
<span data-ttu-id="8c34f-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c34f-135">The following is an example of the response.</span></span>
><span data-ttu-id="8c34f-136">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c34f-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8c34f-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c34f-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
