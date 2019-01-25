---
title: Получение ресурса
description: Получение двоичных данных объекта resource файла или изображения.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 60cacbe737a475183a5d08457c149c6cb631c63f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509184"
---
# <a name="get-resource"></a><span data-ttu-id="06571-103">Получение ресурса</span><span class="sxs-lookup"><span data-stu-id="06571-103">Get resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06571-104">Получение двоичных данных объекта [resource](../resources/resource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="06571-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="06571-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06571-105">Permissions</span></span>
<span data-ttu-id="06571-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06571-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06571-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06571-108">Permission type</span></span>      | <span data-ttu-id="06571-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06571-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06571-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06571-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06571-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06571-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="06571-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06571-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06571-113">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06571-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="06571-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06571-114">Application</span></span> | <span data-ttu-id="06571-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06571-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06571-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06571-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="06571-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06571-117">Request headers</span></span>
| <span data-ttu-id="06571-118">Имя</span><span class="sxs-lookup"><span data-stu-id="06571-118">Name</span></span>       | <span data-ttu-id="06571-119">Тип</span><span class="sxs-lookup"><span data-stu-id="06571-119">Type</span></span> | <span data-ttu-id="06571-120">Описание</span><span class="sxs-lookup"><span data-stu-id="06571-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06571-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06571-121">Authorization</span></span>  | <span data-ttu-id="06571-122">string</span><span class="sxs-lookup"><span data-stu-id="06571-122">string</span></span>  | <span data-ttu-id="06571-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06571-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06571-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06571-125">Request body</span></span>
<span data-ttu-id="06571-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06571-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06571-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="06571-127">Response</span></span>

<span data-ttu-id="06571-128">При успешном выполнении это метод возвращает код отклика `200 OK` и двоичные данные изображения или файла в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="06571-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="06571-129">Примечание. Изображения не будут отображаться непосредственно в браузере, так как для их получения необходима авторизация (как и для остальной части содержимого страницы).</span><span class="sxs-lookup"><span data-stu-id="06571-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="06571-130">Пример</span><span class="sxs-lookup"><span data-stu-id="06571-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06571-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="06571-131">Request</span></span>
<span data-ttu-id="06571-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06571-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="06571-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="06571-133">Response</span></span>
<span data-ttu-id="06571-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06571-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/resource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
