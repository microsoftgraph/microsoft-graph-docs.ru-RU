---
title: Список объектов contactFolder
description: Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 55558b8ea0db3c35d63abdffdef55d01488fe7e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857374"
---
# <a name="list-contactfolders"></a><span data-ttu-id="68832-103">Список объектов contactFolder</span><span class="sxs-lookup"><span data-stu-id="68832-103">List contactFolders</span></span>

<span data-ttu-id="68832-104">Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="68832-104">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="68832-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68832-105">Permissions</span></span>
<span data-ttu-id="68832-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68832-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68832-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68832-108">Permission type</span></span>      | <span data-ttu-id="68832-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68832-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68832-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68832-110">Delegated (work or school account)</span></span> | <span data-ttu-id="68832-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68832-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="68832-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68832-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68832-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68832-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="68832-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68832-114">Application</span></span> | <span data-ttu-id="68832-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68832-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="68832-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68832-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="68832-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="68832-117">Optional query parameters</span></span>
<span data-ttu-id="68832-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="68832-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="68832-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68832-119">Request headers</span></span>
| <span data-ttu-id="68832-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68832-120">Header</span></span>       | <span data-ttu-id="68832-121">Значение</span><span class="sxs-lookup"><span data-stu-id="68832-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68832-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68832-122">Authorization</span></span>  | <span data-ttu-id="68832-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68832-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="68832-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68832-125">Content-Type</span></span>   | <span data-ttu-id="68832-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68832-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68832-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68832-127">Request body</span></span>
<span data-ttu-id="68832-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68832-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68832-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="68832-129">Response</span></span>

<span data-ttu-id="68832-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68832-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68832-131">Пример</span><span class="sxs-lookup"><span data-stu-id="68832-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68832-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="68832-132">Request</span></span>
<span data-ttu-id="68832-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68832-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="68832-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="68832-134">Response</span></span>
<span data-ttu-id="68832-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="68832-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
