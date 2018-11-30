---
title: Список объектов mailFolder
description: Получите все почтовые папки в почтовом ящике пользователь выполнил вход.
ms.openlocfilehash: c93c870447e2414dfbdeb4e248f65c3aa5e0a4a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080530"
---
# <a name="list-mailfolders"></a><span data-ttu-id="479b4-103">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="479b4-103">List mailFolders</span></span>

> <span data-ttu-id="479b4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="479b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="479b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="479b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="479b4-106">Получите все почтовые папки в почтовом ящике пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="479b4-106">Get all the mail folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="479b4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="479b4-107">Permissions</span></span>
<span data-ttu-id="479b4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="479b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="479b4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="479b4-110">Permission type</span></span>      | <span data-ttu-id="479b4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="479b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="479b4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="479b4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="479b4-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="479b4-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="479b4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="479b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="479b4-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="479b4-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="479b4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="479b4-116">Application</span></span> | <span data-ttu-id="479b4-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="479b4-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="479b4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="479b4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="479b4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="479b4-119">Optional query parameters</span></span>
<span data-ttu-id="479b4-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="479b4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="479b4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="479b4-121">Request headers</span></span>
| <span data-ttu-id="479b4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="479b4-122">Header</span></span>       | <span data-ttu-id="479b4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="479b4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="479b4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="479b4-124">Authorization</span></span>  | <span data-ttu-id="479b4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="479b4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="479b4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="479b4-127">Content-Type</span></span>   | <span data-ttu-id="479b4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="479b4-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="479b4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="479b4-129">Request body</span></span>
<span data-ttu-id="479b4-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="479b4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="479b4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="479b4-131">Response</span></span>

<span data-ttu-id="479b4-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [MailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="479b4-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="479b4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="479b4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="479b4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="479b4-134">Request</span></span>
<span data-ttu-id="479b4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="479b4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="479b4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="479b4-136">Response</span></span>
<span data-ttu-id="479b4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="479b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
