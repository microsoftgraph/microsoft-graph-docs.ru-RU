---
title: Получение соглашения
description: Извлечение свойств и связи объекта соглашения.
localization_priority: Normal
ms.openlocfilehash: da36b6cb2d12c92d4bf12ec2ce4836f5bbc5efe1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517129"
---
# <a name="get-agreement"></a><span data-ttu-id="4ef94-103">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="4ef94-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ef94-104">Извлечение свойств и связи объекта [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="4ef94-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ef94-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ef94-105">Permissions</span></span>
<span data-ttu-id="4ef94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ef94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ef94-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ef94-108">Permission type</span></span>                        | <span data-ttu-id="4ef94-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ef94-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ef94-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ef94-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ef94-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ef94-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="4ef94-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ef94-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ef94-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ef94-113">Not supported.</span></span> |
|<span data-ttu-id="4ef94-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ef94-114">Application</span></span>                            | <span data-ttu-id="4ef94-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ef94-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ef94-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ef94-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="4ef94-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ef94-117">Request headers</span></span>
| <span data-ttu-id="4ef94-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4ef94-118">Name</span></span>         | <span data-ttu-id="4ef94-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4ef94-119">Type</span></span>        | <span data-ttu-id="4ef94-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4ef94-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4ef94-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ef94-121">Authorization</span></span> | <span data-ttu-id="4ef94-122">string</span><span class="sxs-lookup"><span data-stu-id="4ef94-122">string</span></span> | <span data-ttu-id="4ef94-123">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="4ef94-123">Bearer \{token\}.</span></span> <span data-ttu-id="4ef94-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ef94-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ef94-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ef94-125">Request body</span></span>
<span data-ttu-id="4ef94-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ef94-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4ef94-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ef94-127">Response</span></span>
<span data-ttu-id="4ef94-128">Успешно завершена, этот метод возвращает `200 OK` объект [соглашение](../resources/agreement.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4ef94-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ef94-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4ef94-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ef94-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ef94-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="4ef94-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ef94-131">Response</span></span>
><span data-ttu-id="4ef94-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ef94-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
