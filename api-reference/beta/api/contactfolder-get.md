---
title: Получение объекта contactFolder
description: Получение папки контактов с помощью ее идентификатора.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 86f2adf867737e31d96a75d40f50442b10a468b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985118"
---
# <a name="get-contactfolder"></a><span data-ttu-id="f75b9-103">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="f75b9-103">Get contactFolder</span></span>

> <span data-ttu-id="f75b9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f75b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f75b9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f75b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f75b9-106">Получение папки контактов с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="f75b9-106">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="f75b9-107">Существует два сценария, где приложение может получить папке контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f75b9-107">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="f75b9-108">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="f75b9-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="f75b9-109">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя, и другой пользователь общей папке контактов с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="f75b9-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="f75b9-110">В разделе [сведения и примеры](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="f75b9-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="f75b9-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f75b9-111">Permissions</span></span>
<span data-ttu-id="f75b9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f75b9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f75b9-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f75b9-114">Permission type</span></span>      | <span data-ttu-id="f75b9-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f75b9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f75b9-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f75b9-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f75b9-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f75b9-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f75b9-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f75b9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f75b9-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f75b9-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f75b9-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f75b9-120">Application</span></span> | <span data-ttu-id="f75b9-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f75b9-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f75b9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f75b9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f75b9-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f75b9-123">Optional query parameters</span></span>
<span data-ttu-id="f75b9-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f75b9-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f75b9-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f75b9-125">Request headers</span></span>
| <span data-ttu-id="f75b9-126">Имя</span><span class="sxs-lookup"><span data-stu-id="f75b9-126">Name</span></span>       | <span data-ttu-id="f75b9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f75b9-127">Type</span></span> | <span data-ttu-id="f75b9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f75b9-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f75b9-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f75b9-129">Authorization</span></span>  | <span data-ttu-id="f75b9-130">string</span><span class="sxs-lookup"><span data-stu-id="f75b9-130">string</span></span>  | <span data-ttu-id="f75b9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f75b9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f75b9-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f75b9-133">Request body</span></span>
<span data-ttu-id="f75b9-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f75b9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f75b9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f75b9-135">Response</span></span>

<span data-ttu-id="f75b9-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f75b9-136">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f75b9-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f75b9-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f75b9-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f75b9-138">Request</span></span>
<span data-ttu-id="f75b9-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f75b9-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="f75b9-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="f75b9-140">Response</span></span>
<span data-ttu-id="f75b9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f75b9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
