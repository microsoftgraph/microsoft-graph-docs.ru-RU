---
title: Получение privilegedRoleSummary
description: Получение свойств и связей объекта Привилежедролесуммари.
localization_priority: Normal
ms.openlocfilehash: 2261d4340d5c9feb29d81da195148047aa68ab88
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593720"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="10fed-103">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="10fed-103">Get privilegedRoleSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10fed-104">Получение свойств и связей объекта [привилежедролесуммари](../resources/privilegedrolesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="10fed-104">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="10fed-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10fed-105">Permissions</span></span>
<span data-ttu-id="10fed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="10fed-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10fed-108">Permission type</span></span>      | <span data-ttu-id="10fed-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10fed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10fed-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10fed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10fed-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10fed-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="10fed-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10fed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10fed-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10fed-113">Not supported.</span></span>    |
|<span data-ttu-id="10fed-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10fed-114">Application</span></span> | <span data-ttu-id="10fed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10fed-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10fed-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10fed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10fed-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10fed-117">Optional query parameters</span></span>
<span data-ttu-id="10fed-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10fed-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10fed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10fed-119">Request headers</span></span>
| <span data-ttu-id="10fed-120">Имя</span><span class="sxs-lookup"><span data-stu-id="10fed-120">Name</span></span>      |<span data-ttu-id="10fed-121">Описание</span><span class="sxs-lookup"><span data-stu-id="10fed-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10fed-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10fed-122">Authorization</span></span>  | <span data-ttu-id="10fed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10fed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10fed-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10fed-125">Request body</span></span>
<span data-ttu-id="10fed-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10fed-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10fed-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="10fed-127">Response</span></span>

<span data-ttu-id="10fed-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролесуммари](../resources/privilegedrolesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10fed-128">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="10fed-129">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="10fed-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="10fed-130">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="10fed-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="10fed-131">Пример</span><span class="sxs-lookup"><span data-stu-id="10fed-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10fed-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="10fed-132">Request</span></span>
<span data-ttu-id="10fed-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10fed-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="10fed-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="10fed-134">Response</span></span>
<span data-ttu-id="10fed-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10fed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="10fed-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="10fed-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="10fed-139">Языках</span><span class="sxs-lookup"><span data-stu-id="10fed-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedrolesummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10fed-140">Язык</span><span class="sxs-lookup"><span data-stu-id="10fed-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedrolesummary-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
