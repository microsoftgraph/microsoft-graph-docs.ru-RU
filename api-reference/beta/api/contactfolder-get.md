---
title: Получение объекта contactFolder
description: Получение папки контактов с помощью ее идентификатора.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5ab29eb96f900404f035442605047bd2df3e37e2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530022"
---
# <a name="get-contactfolder"></a><span data-ttu-id="a217f-103">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="a217f-103">Get contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a217f-104">Получение папки контактов с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="a217f-104">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="a217f-105">Существует два сценария, где приложение может получить папке контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a217f-105">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="a217f-106">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="a217f-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a217f-107">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя, и другой пользователь общей папке контактов с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="a217f-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a217f-108">В разделе [сведения и примеры](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="a217f-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="a217f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a217f-109">Permissions</span></span>
<span data-ttu-id="a217f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a217f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a217f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a217f-112">Permission type</span></span>      | <span data-ttu-id="a217f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a217f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a217f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a217f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a217f-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a217f-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a217f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a217f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a217f-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a217f-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a217f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a217f-118">Application</span></span> | <span data-ttu-id="a217f-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a217f-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a217f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a217f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a217f-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a217f-121">Optional query parameters</span></span>
<span data-ttu-id="a217f-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a217f-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a217f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a217f-123">Request headers</span></span>
| <span data-ttu-id="a217f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a217f-124">Name</span></span>       | <span data-ttu-id="a217f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="a217f-125">Type</span></span> | <span data-ttu-id="a217f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a217f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a217f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a217f-127">Authorization</span></span>  | <span data-ttu-id="a217f-128">string</span><span class="sxs-lookup"><span data-stu-id="a217f-128">string</span></span>  | <span data-ttu-id="a217f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a217f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a217f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a217f-131">Request body</span></span>
<span data-ttu-id="a217f-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a217f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a217f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a217f-133">Response</span></span>

<span data-ttu-id="a217f-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a217f-134">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a217f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a217f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a217f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a217f-136">Request</span></span>
<span data-ttu-id="a217f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a217f-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="a217f-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="a217f-138">Response</span></span>
<span data-ttu-id="a217f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a217f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
