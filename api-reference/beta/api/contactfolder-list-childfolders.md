---
title: Список childFolders
description: Получение коллекции дочерних папок в указанной папке контактов.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 78d2780b2089f5d4f90c9f7b090c43afe15c07f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941249"
---
# <a name="list-childfolders"></a><span data-ttu-id="7376f-103">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="7376f-103">List childFolders</span></span>

> <span data-ttu-id="7376f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7376f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7376f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7376f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7376f-106">Получение коллекции дочерних папок в указанной папке контактов.</span><span class="sxs-lookup"><span data-stu-id="7376f-106">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="7376f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7376f-107">Permissions</span></span>
<span data-ttu-id="7376f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7376f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7376f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7376f-110">Permission type</span></span>      | <span data-ttu-id="7376f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7376f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7376f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7376f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7376f-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7376f-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7376f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7376f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7376f-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7376f-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7376f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7376f-116">Application</span></span> | <span data-ttu-id="7376f-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7376f-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7376f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7376f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7376f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7376f-119">Optional query parameters</span></span>
<span data-ttu-id="7376f-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7376f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7376f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7376f-121">Request headers</span></span>
| <span data-ttu-id="7376f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7376f-122">Name</span></span>       | <span data-ttu-id="7376f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7376f-123">Type</span></span> | <span data-ttu-id="7376f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7376f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7376f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7376f-125">Authorization</span></span>  | <span data-ttu-id="7376f-126">string</span><span class="sxs-lookup"><span data-stu-id="7376f-126">string</span></span>  | <span data-ttu-id="7376f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7376f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7376f-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7376f-129">Request body</span></span>
<span data-ttu-id="7376f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7376f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7376f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7376f-131">Response</span></span>

<span data-ttu-id="7376f-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7376f-132">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7376f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7376f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7376f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7376f-134">Request</span></span>
<span data-ttu-id="7376f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7376f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="7376f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7376f-136">Response</span></span>
<span data-ttu-id="7376f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7376f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
