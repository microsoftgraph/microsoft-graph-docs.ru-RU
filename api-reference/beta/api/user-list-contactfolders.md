---
title: Список объектов contactFolder
description: Получение всех контактов папок в почтовом ящике пользователь выполнил вход.
localization_priority: Normal
ms.openlocfilehash: 17c9cc2328af813fcec2094324310a7e53f61689
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860734"
---
# <a name="list-contactfolders"></a><span data-ttu-id="cd259-103">Список объектов contactFolder</span><span class="sxs-lookup"><span data-stu-id="cd259-103">List contactFolders</span></span>

> <span data-ttu-id="cd259-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd259-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd259-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd259-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd259-106">Получение всех контактов папок в почтовом ящике пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="cd259-106">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd259-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd259-107">Permissions</span></span>
<span data-ttu-id="cd259-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd259-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd259-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd259-110">Permission type</span></span>      | <span data-ttu-id="cd259-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd259-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd259-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd259-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cd259-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd259-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cd259-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd259-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd259-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd259-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cd259-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd259-116">Application</span></span> | <span data-ttu-id="cd259-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd259-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd259-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd259-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cd259-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cd259-119">Optional query parameters</span></span>
<span data-ttu-id="cd259-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cd259-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cd259-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd259-121">Request headers</span></span>
| <span data-ttu-id="cd259-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd259-122">Header</span></span>       | <span data-ttu-id="cd259-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cd259-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd259-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd259-124">Authorization</span></span>  | <span data-ttu-id="cd259-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd259-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd259-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd259-127">Content-Type</span></span>   | <span data-ttu-id="cd259-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cd259-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd259-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd259-129">Request body</span></span>
<span data-ttu-id="cd259-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd259-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd259-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd259-131">Response</span></span>

<span data-ttu-id="cd259-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd259-132">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cd259-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cd259-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd259-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd259-134">Request</span></span>
<span data-ttu-id="cd259-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd259-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="cd259-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd259-136">Response</span></span>
<span data-ttu-id="cd259-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cd259-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
