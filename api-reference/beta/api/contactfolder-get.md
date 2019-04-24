---
title: Получение объекта contactFolder
description: Получение папки контактов с помощью ее идентификатора.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5ab29eb96f900404f035442605047bd2df3e37e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455666"
---
# <a name="get-contactfolder"></a><span data-ttu-id="cd98d-103">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="cd98d-103">Get contactFolder</span></span>

<span data-ttu-id="cd98d-104">Получение папки контактов с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="cd98d-104">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="cd98d-105">Существует два сценария, в которых приложение может получить папку контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="cd98d-105">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="cd98d-106">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="cd98d-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="cd98d-107">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="cd98d-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="cd98d-108">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="cd98d-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="cd98d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd98d-109">Permissions</span></span>
<span data-ttu-id="cd98d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd98d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd98d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd98d-112">Permission type</span></span>      | <span data-ttu-id="cd98d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd98d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd98d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd98d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cd98d-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd98d-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cd98d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd98d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd98d-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd98d-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cd98d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd98d-118">Application</span></span> | <span data-ttu-id="cd98d-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd98d-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd98d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd98d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cd98d-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cd98d-121">Optional query parameters</span></span>
<span data-ttu-id="cd98d-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cd98d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cd98d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd98d-123">Request headers</span></span>
| <span data-ttu-id="cd98d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="cd98d-124">Name</span></span>       | <span data-ttu-id="cd98d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="cd98d-125">Type</span></span> | <span data-ttu-id="cd98d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cd98d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cd98d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd98d-127">Authorization</span></span>  | <span data-ttu-id="cd98d-128">string</span><span class="sxs-lookup"><span data-stu-id="cd98d-128">string</span></span>  | <span data-ttu-id="cd98d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd98d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd98d-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd98d-131">Request body</span></span>
<span data-ttu-id="cd98d-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd98d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd98d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd98d-133">Response</span></span>

<span data-ttu-id="cd98d-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd98d-134">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cd98d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="cd98d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd98d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd98d-136">Request</span></span>
<span data-ttu-id="cd98d-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd98d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="cd98d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd98d-138">Response</span></span>
<span data-ttu-id="cd98d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd98d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "parentFolderId": "AAMkAGI2AAEOAAA="
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
