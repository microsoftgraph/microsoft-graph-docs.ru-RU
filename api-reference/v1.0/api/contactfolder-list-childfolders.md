---
title: Список childFolders
description: Получение коллекции дочерних папок в указанной папке контактов.
ms.openlocfilehash: 7495d91636ac9c40c8f597cc020ad515b58bd73d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025265"
---
# <a name="list-childfolders"></a><span data-ttu-id="a87c6-103">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="a87c6-103">List childFolders</span></span>

<span data-ttu-id="a87c6-104">Получение коллекции дочерних папок в указанной папке контактов.</span><span class="sxs-lookup"><span data-stu-id="a87c6-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a87c6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a87c6-105">Permissions</span></span>
<span data-ttu-id="a87c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a87c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a87c6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a87c6-108">Permission type</span></span>      | <span data-ttu-id="a87c6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a87c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a87c6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a87c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a87c6-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a87c6-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a87c6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a87c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a87c6-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a87c6-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a87c6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a87c6-114">Application</span></span> | <span data-ttu-id="a87c6-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a87c6-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a87c6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a87c6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a87c6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a87c6-117">Optional query parameters</span></span>
<span data-ttu-id="a87c6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a87c6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a87c6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a87c6-119">Request headers</span></span>
| <span data-ttu-id="a87c6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a87c6-120">Name</span></span>       | <span data-ttu-id="a87c6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a87c6-121">Type</span></span> | <span data-ttu-id="a87c6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a87c6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a87c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a87c6-123">Authorization</span></span>  | <span data-ttu-id="a87c6-124">string</span><span class="sxs-lookup"><span data-stu-id="a87c6-124">string</span></span>  | <span data-ttu-id="a87c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a87c6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a87c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a87c6-127">Request body</span></span>
<span data-ttu-id="a87c6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a87c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a87c6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a87c6-129">Response</span></span>

<span data-ttu-id="a87c6-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a87c6-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a87c6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a87c6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a87c6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a87c6-132">Request</span></span>
<span data-ttu-id="a87c6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a87c6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="a87c6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a87c6-134">Response</span></span>
<span data-ttu-id="a87c6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a87c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
