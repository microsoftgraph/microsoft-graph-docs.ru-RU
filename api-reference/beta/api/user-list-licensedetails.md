---
title: Перечисление licenseDetails
description: Получение списка объектов licenseDetails.
author: dkershaw10
ms.openlocfilehash: 9c8c7d9ddcc951df7a2ac8c8151ae368c7e76483
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351368"
---
# <a name="list-licensedetails"></a><span data-ttu-id="8221d-103">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="8221d-103">List licenseDetails</span></span>

> <span data-ttu-id="8221d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8221d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8221d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8221d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8221d-106">Получение списка объектов licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="8221d-106">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8221d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8221d-107">Permissions</span></span>
<span data-ttu-id="8221d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8221d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8221d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8221d-110">Permission type</span></span>      | <span data-ttu-id="8221d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8221d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8221d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8221d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8221d-113">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8221d-113">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8221d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8221d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8221d-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="8221d-115">User.Read</span></span>    |
|<span data-ttu-id="8221d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8221d-116">Application</span></span> | <span data-ttu-id="8221d-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8221d-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8221d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8221d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8221d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8221d-119">Optional query parameters</span></span>
<span data-ttu-id="8221d-120">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="8221d-120">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8221d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8221d-121">Request headers</span></span>
| <span data-ttu-id="8221d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8221d-122">Name</span></span>      |<span data-ttu-id="8221d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8221d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8221d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8221d-124">Authorization</span></span>  | <span data-ttu-id="8221d-125">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="8221d-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="8221d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8221d-126">Request body</span></span>
<span data-ttu-id="8221d-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8221d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8221d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8221d-128">Response</span></span>

<span data-ttu-id="8221d-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [licenseDetails](../resources/licensedetails.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8221d-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8221d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8221d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8221d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8221d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="8221d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8221d-132">Response</span></span>
<span data-ttu-id="8221d-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8221d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->