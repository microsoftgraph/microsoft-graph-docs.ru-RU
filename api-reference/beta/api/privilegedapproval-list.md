---
title: Список privilegedApproval
description: Получение списка объектов privilegedapproval.
localization_priority: Normal
ms.openlocfilehash: ab3a3c2670cd0ddebf8415e112305679c1d3446c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521553"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="703b7-103">Список privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="703b7-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="703b7-104">Получение списка объектов privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="703b7-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="703b7-105">Чтобы отфильтровать результаты запроса, используйте стандартные OData ``$filter`` выражения в URI.</span><span class="sxs-lookup"><span data-stu-id="703b7-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="703b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="703b7-106">Permissions</span></span>
<span data-ttu-id="703b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="703b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="703b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="703b7-109">Permission type</span></span>      | <span data-ttu-id="703b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="703b7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="703b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="703b7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="703b7-112">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="703b7-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="703b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="703b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="703b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="703b7-114">Not supported.</span></span>    |
|<span data-ttu-id="703b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="703b7-115">Application</span></span> | <span data-ttu-id="703b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="703b7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="703b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="703b7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="703b7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="703b7-118">Optional query parameters</span></span>
<span data-ttu-id="703b7-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="703b7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="703b7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="703b7-120">Request headers</span></span>
| <span data-ttu-id="703b7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="703b7-121">Name</span></span>      |<span data-ttu-id="703b7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="703b7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="703b7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="703b7-123">Authorization</span></span>  | <span data-ttu-id="703b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="703b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="703b7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="703b7-126">Request body</span></span>
<span data-ttu-id="703b7-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="703b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="703b7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="703b7-128">Response</span></span>

<span data-ttu-id="703b7-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedApproval](../resources/privilegedapproval.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="703b7-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="703b7-130">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="703b7-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="703b7-131">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="703b7-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="703b7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="703b7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="703b7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="703b7-133">Request</span></span>
<span data-ttu-id="703b7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="703b7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="703b7-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="703b7-135">Response</span></span>
<span data-ttu-id="703b7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="703b7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
