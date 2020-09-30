---
title: Получение privilegedRoleSummary
description: Получение свойств и связей объекта Привилежедролесуммари.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 80f46a26c97ddb90fe197c797840691abcd986df
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313949"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="77253-103">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="77253-103">Get privilegedRoleSummary</span></span>

<span data-ttu-id="77253-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77253-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77253-105">Получение свойств и связей объекта [привилежедролесуммари](../resources/privilegedrolesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="77253-105">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="77253-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77253-106">Permissions</span></span>
<span data-ttu-id="77253-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="77253-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77253-109">Permission type</span></span>      | <span data-ttu-id="77253-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77253-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77253-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77253-111">Delegated (work or school account)</span></span> | <span data-ttu-id="77253-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77253-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77253-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77253-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77253-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77253-114">Not supported.</span></span>    |
|<span data-ttu-id="77253-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77253-115">Application</span></span> | <span data-ttu-id="77253-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77253-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77253-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77253-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="77253-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77253-118">Optional query parameters</span></span>
<span data-ttu-id="77253-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77253-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77253-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77253-120">Request headers</span></span>
| <span data-ttu-id="77253-121">Имя</span><span class="sxs-lookup"><span data-stu-id="77253-121">Name</span></span>      |<span data-ttu-id="77253-122">Описание</span><span class="sxs-lookup"><span data-stu-id="77253-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77253-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77253-123">Authorization</span></span>  | <span data-ttu-id="77253-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77253-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77253-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77253-126">Request body</span></span>
<span data-ttu-id="77253-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77253-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77253-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="77253-128">Response</span></span>

<span data-ttu-id="77253-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролесуммари](../resources/privilegedrolesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77253-129">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="77253-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="77253-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="77253-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="77253-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="77253-132">Пример</span><span class="sxs-lookup"><span data-stu-id="77253-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77253-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="77253-133">Request</span></span>
<span data-ttu-id="77253-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77253-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77253-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="77253-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
# <a name="c"></a>[<span data-ttu-id="77253-136">C#</span><span class="sxs-lookup"><span data-stu-id="77253-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77253-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77253-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77253-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77253-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77253-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="77253-139">Response</span></span>
<span data-ttu-id="77253-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77253-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->