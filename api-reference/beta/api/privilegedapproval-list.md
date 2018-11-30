---
title: Список privilegedApproval
description: Получение списка объектов privilegedapproval.
ms.openlocfilehash: 69e558a734f86dd72b35e61d9f8ceab52b9f981e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081253"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="c3907-103">Список privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="c3907-103">List privilegedApproval</span></span>

> <span data-ttu-id="c3907-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3907-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3907-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3907-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3907-106">Получение списка объектов privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="c3907-106">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="c3907-107">Чтобы отфильтровать результаты запроса, используйте стандартные OData ``$filter`` выражения в URI.</span><span class="sxs-lookup"><span data-stu-id="c3907-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3907-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3907-108">Permissions</span></span>
<span data-ttu-id="c3907-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3907-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c3907-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3907-111">Permission type</span></span>      | <span data-ttu-id="c3907-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3907-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3907-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3907-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c3907-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3907-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c3907-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3907-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3907-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3907-116">Not supported.</span></span>    |
|<span data-ttu-id="c3907-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3907-117">Application</span></span> | <span data-ttu-id="c3907-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3907-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3907-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3907-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3907-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3907-120">Optional query parameters</span></span>
<span data-ttu-id="c3907-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c3907-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3907-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3907-122">Request headers</span></span>
| <span data-ttu-id="c3907-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c3907-123">Name</span></span>      |<span data-ttu-id="c3907-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c3907-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3907-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3907-125">Authorization</span></span>  | <span data-ttu-id="c3907-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3907-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3907-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3907-128">Request body</span></span>
<span data-ttu-id="c3907-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3907-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3907-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3907-130">Response</span></span>

<span data-ttu-id="c3907-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedApproval](../resources/privilegedapproval.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c3907-131">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="c3907-132">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="c3907-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c3907-133">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="c3907-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="c3907-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c3907-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3907-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3907-135">Request</span></span>
<span data-ttu-id="c3907-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3907-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="c3907-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3907-137">Response</span></span>
<span data-ttu-id="c3907-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c3907-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
