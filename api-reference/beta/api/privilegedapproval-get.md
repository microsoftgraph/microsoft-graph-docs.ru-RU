---
title: Получение privilegedApproval
description: Извлечение свойств и связи объекта privilegedapproval.
ms.openlocfilehash: 77db18f46bbdfec6a5a9a62e4e481facaab6cb8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080811"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="202d1-103">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="202d1-103">Get privilegedApproval</span></span>

> <span data-ttu-id="202d1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="202d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="202d1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="202d1-106">Извлечение свойств и связи объекта privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="202d1-106">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="202d1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="202d1-107">Permissions</span></span>
<span data-ttu-id="202d1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="202d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="202d1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="202d1-110">Permission type</span></span>      | <span data-ttu-id="202d1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="202d1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="202d1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="202d1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="202d1-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="202d1-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="202d1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="202d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="202d1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202d1-115">Not supported.</span></span>    |
|<span data-ttu-id="202d1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="202d1-116">Application</span></span> | <span data-ttu-id="202d1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202d1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="202d1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="202d1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="202d1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="202d1-119">Optional query parameters</span></span>
<span data-ttu-id="202d1-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="202d1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="202d1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="202d1-121">Request headers</span></span>
| <span data-ttu-id="202d1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="202d1-122">Name</span></span>      |<span data-ttu-id="202d1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="202d1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="202d1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="202d1-124">Authorization</span></span>  | <span data-ttu-id="202d1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="202d1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="202d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="202d1-127">Request body</span></span>
<span data-ttu-id="202d1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="202d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="202d1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="202d1-129">Response</span></span>

<span data-ttu-id="202d1-130">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedApproval](../resources/privilegedapproval.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="202d1-130">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="202d1-131">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="202d1-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="202d1-132">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="202d1-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="202d1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="202d1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="202d1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="202d1-134">Request</span></span>
<span data-ttu-id="202d1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="202d1-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="202d1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="202d1-136">Response</span></span>
<span data-ttu-id="202d1-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="202d1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
