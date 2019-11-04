---
title: Список владельцев
description: Получение списка владельцев (объектов directoryObject) для приложения.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8f7c8f18985921b0a96c9ad9598f830e2ca47e6e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939714"
---
# <a name="list-owners"></a><span data-ttu-id="c58b5-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="c58b5-103">List owners</span></span>

<span data-ttu-id="c58b5-104">Получение списка владельцев для приложения, которое является [directoryObject](../resources/directoryobject.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="c58b5-104">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c58b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c58b5-105">Permissions</span></span>
<span data-ttu-id="c58b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c58b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c58b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c58b5-108">Permission type</span></span>      | <span data-ttu-id="c58b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c58b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c58b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c58b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c58b5-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c58b5-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c58b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c58b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c58b5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c58b5-113">Not supported.</span></span>    |
|<span data-ttu-id="c58b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c58b5-114">Application</span></span> | <span data-ttu-id="c58b5-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c58b5-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c58b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c58b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c58b5-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c58b5-117">Optional query parameters</span></span>
<span data-ttu-id="c58b5-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c58b5-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c58b5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c58b5-119">Request headers</span></span>
| <span data-ttu-id="c58b5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c58b5-120">Name</span></span>       | <span data-ttu-id="c58b5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c58b5-121">Type</span></span> | <span data-ttu-id="c58b5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c58b5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c58b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c58b5-123">Authorization</span></span>  | <span data-ttu-id="c58b5-124">string</span><span class="sxs-lookup"><span data-stu-id="c58b5-124">string</span></span>  | <span data-ttu-id="c58b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c58b5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c58b5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c58b5-127">Request body</span></span>
<span data-ttu-id="c58b5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c58b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c58b5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c58b5-129">Response</span></span>

<span data-ttu-id="c58b5-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c58b5-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c58b5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c58b5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c58b5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c58b5-132">Request</span></span>
<span data-ttu-id="c58b5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c58b5-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/applications/{id}/owners
```
##### <a name="response"></a><span data-ttu-id="c58b5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c58b5-134">Response</span></span>
<span data-ttu-id="c58b5-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c58b5-135">Here is an example of the response.</span></span> 

><span data-ttu-id="c58b5-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c58b5-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
