---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d2f61152b8edd98aa11fc7c6b34d2c2b04b72f55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990126"
---
# <a name="get-mailfolder"></a><span data-ttu-id="aa9de-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="aa9de-103">Get mailFolder</span></span>

<span data-ttu-id="aa9de-104">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="aa9de-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="aa9de-105">Существует два сценария, где приложение может получить почтовой папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa9de-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="aa9de-106">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="aa9de-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="aa9de-107">Если приложение имеет соответствующий делегированных [разрешений](#permissions) от одного пользователя и другой пользователь доступ к папке почты с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="aa9de-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="aa9de-108">В разделе [сведения и примеры](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="aa9de-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="aa9de-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa9de-109">Permissions</span></span>
<span data-ttu-id="aa9de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa9de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa9de-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa9de-112">Permission type</span></span>      | <span data-ttu-id="aa9de-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa9de-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa9de-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa9de-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aa9de-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa9de-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aa9de-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa9de-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa9de-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa9de-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aa9de-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa9de-118">Application</span></span> | <span data-ttu-id="aa9de-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa9de-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa9de-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa9de-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa9de-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa9de-121">Optional query parameters</span></span>
<span data-ttu-id="aa9de-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa9de-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="aa9de-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa9de-123">Request headers</span></span>
| <span data-ttu-id="aa9de-124">Имя</span><span class="sxs-lookup"><span data-stu-id="aa9de-124">Name</span></span>       | <span data-ttu-id="aa9de-125">Тип</span><span class="sxs-lookup"><span data-stu-id="aa9de-125">Type</span></span> | <span data-ttu-id="aa9de-126">Описание</span><span class="sxs-lookup"><span data-stu-id="aa9de-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa9de-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa9de-127">Authorization</span></span>  | <span data-ttu-id="aa9de-128">строка</span><span class="sxs-lookup"><span data-stu-id="aa9de-128">string</span></span>  | <span data-ttu-id="aa9de-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa9de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa9de-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa9de-131">Request body</span></span>
<span data-ttu-id="aa9de-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa9de-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa9de-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa9de-133">Response</span></span>

<span data-ttu-id="aa9de-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa9de-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa9de-135">Пример</span><span class="sxs-lookup"><span data-stu-id="aa9de-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa9de-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa9de-136">Request</span></span>
<span data-ttu-id="aa9de-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa9de-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="aa9de-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa9de-138">Response</span></span>
<span data-ttu-id="aa9de-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aa9de-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
