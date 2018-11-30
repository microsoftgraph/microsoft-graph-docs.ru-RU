---
title: Список childFolders
description: Получение коллекции дочерних папок в указанной папке контактов.
ms.openlocfilehash: 7d379e81229ee8efd4c12718147a99ed13ebdb93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077898"
---
# <a name="list-childfolders"></a><span data-ttu-id="59182-103">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="59182-103">List childFolders</span></span>

> <span data-ttu-id="59182-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="59182-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59182-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59182-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59182-106">Получение коллекции дочерних папок в указанной папке контактов.</span><span class="sxs-lookup"><span data-stu-id="59182-106">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="59182-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59182-107">Permissions</span></span>
<span data-ttu-id="59182-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59182-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59182-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59182-110">Permission type</span></span>      | <span data-ttu-id="59182-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59182-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59182-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59182-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59182-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59182-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="59182-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59182-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59182-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59182-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="59182-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59182-116">Application</span></span> | <span data-ttu-id="59182-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59182-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59182-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59182-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59182-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="59182-119">Optional query parameters</span></span>
<span data-ttu-id="59182-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="59182-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59182-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59182-121">Request headers</span></span>
| <span data-ttu-id="59182-122">Имя</span><span class="sxs-lookup"><span data-stu-id="59182-122">Name</span></span>       | <span data-ttu-id="59182-123">Тип</span><span class="sxs-lookup"><span data-stu-id="59182-123">Type</span></span> | <span data-ttu-id="59182-124">Описание</span><span class="sxs-lookup"><span data-stu-id="59182-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59182-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="59182-125">Authorization</span></span>  | <span data-ttu-id="59182-126">string</span><span class="sxs-lookup"><span data-stu-id="59182-126">string</span></span>  | <span data-ttu-id="59182-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59182-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59182-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59182-129">Request body</span></span>
<span data-ttu-id="59182-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59182-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59182-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="59182-131">Response</span></span>

<span data-ttu-id="59182-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59182-132">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59182-133">Пример</span><span class="sxs-lookup"><span data-stu-id="59182-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59182-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="59182-134">Request</span></span>
<span data-ttu-id="59182-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59182-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="59182-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="59182-136">Response</span></span>
<span data-ttu-id="59182-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="59182-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
