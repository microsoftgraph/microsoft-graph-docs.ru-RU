---
title: Список rejectedSenders
description: 'Получение пользователей или групп из списка rejectedSenders для данной группы. '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 2ce1f5244997e9ef38c9e57b020fa1f0bfb22e37
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849142"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="8f39e-103">Список rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="8f39e-103">List rejectedSenders</span></span>

> <span data-ttu-id="8f39e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f39e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f39e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f39e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f39e-106">Получение пользователей или групп из списка rejectedSenders для данной группы.</span><span class="sxs-lookup"><span data-stu-id="8f39e-106">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="8f39e-p102">Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса GET). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="8f39e-p102">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f39e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f39e-109">Permissions</span></span>
<span data-ttu-id="8f39e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f39e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f39e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f39e-112">Permission type</span></span>      | <span data-ttu-id="8f39e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f39e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f39e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f39e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8f39e-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f39e-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f39e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f39e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f39e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f39e-117">Not supported.</span></span>    |
|<span data-ttu-id="8f39e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f39e-118">Application</span></span> | <span data-ttu-id="8f39e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f39e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f39e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f39e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f39e-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f39e-121">Optional query parameters</span></span>
<span data-ttu-id="8f39e-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8f39e-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f39e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f39e-123">Request headers</span></span>
| <span data-ttu-id="8f39e-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f39e-124">Header</span></span>       | <span data-ttu-id="8f39e-125">Значение</span><span class="sxs-lookup"><span data-stu-id="8f39e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8f39e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f39e-126">Authorization</span></span>  | <span data-ttu-id="8f39e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f39e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f39e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f39e-129">Request body</span></span>
<span data-ttu-id="8f39e-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f39e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f39e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f39e-131">Response</span></span>
<span data-ttu-id="8f39e-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f39e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f39e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8f39e-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8f39e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f39e-134">Request</span></span>
<span data-ttu-id="8f39e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f39e-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="8f39e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f39e-136">Response</span></span>
<span data-ttu-id="8f39e-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f39e-137">The following is an example of the response.</span></span>
><span data-ttu-id="8f39e-138">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="8f39e-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8f39e-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f39e-139">All the properties will be returned from an actual call.</span></span>
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
