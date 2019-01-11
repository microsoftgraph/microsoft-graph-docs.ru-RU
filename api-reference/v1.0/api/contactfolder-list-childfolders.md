---
title: Список childFolders
description: Получение коллекции дочерних папок в указанной папке контактов.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 7574b1d269a5ebdda0dbcc4549e8669d6540e1a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873572"
---
# <a name="list-childfolders"></a><span data-ttu-id="9d3ee-103">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="9d3ee-103">List childFolders</span></span>

<span data-ttu-id="9d3ee-104">Получение коллекции дочерних папок в указанной папке контактов.</span><span class="sxs-lookup"><span data-stu-id="9d3ee-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d3ee-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d3ee-105">Permissions</span></span>
<span data-ttu-id="9d3ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d3ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d3ee-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d3ee-108">Permission type</span></span>      | <span data-ttu-id="9d3ee-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d3ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d3ee-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d3ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d3ee-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d3ee-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9d3ee-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d3ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d3ee-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d3ee-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9d3ee-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d3ee-114">Application</span></span> | <span data-ttu-id="9d3ee-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d3ee-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d3ee-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d3ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d3ee-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9d3ee-117">Optional query parameters</span></span>
<span data-ttu-id="9d3ee-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9d3ee-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9d3ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d3ee-119">Request headers</span></span>
| <span data-ttu-id="9d3ee-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9d3ee-120">Name</span></span>       | <span data-ttu-id="9d3ee-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9d3ee-121">Type</span></span> | <span data-ttu-id="9d3ee-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9d3ee-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d3ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d3ee-123">Authorization</span></span>  | <span data-ttu-id="9d3ee-124">string</span><span class="sxs-lookup"><span data-stu-id="9d3ee-124">string</span></span>  | <span data-ttu-id="9d3ee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d3ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d3ee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d3ee-127">Request body</span></span>
<span data-ttu-id="9d3ee-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d3ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d3ee-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d3ee-129">Response</span></span>

<span data-ttu-id="9d3ee-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d3ee-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d3ee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9d3ee-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d3ee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d3ee-132">Request</span></span>
<span data-ttu-id="9d3ee-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d3ee-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="9d3ee-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d3ee-134">Response</span></span>
<span data-ttu-id="9d3ee-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9d3ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
