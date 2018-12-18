---
title: Список владельцев
description: Получение списка объектов directoryObject.
author: lleonard-msft
ms.openlocfilehash: 8b8cb478867639afa07f986c86f38e2460a17338
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325867"
---
# <a name="list-owners"></a><span data-ttu-id="50dc4-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="50dc4-103">List owners</span></span>

> <span data-ttu-id="50dc4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50dc4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50dc4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50dc4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50dc4-106">Получение списка объектов directoryObject.</span><span class="sxs-lookup"><span data-stu-id="50dc4-106">Retrieve a list of directoryObject objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="50dc4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50dc4-107">Permissions</span></span>
<span data-ttu-id="50dc4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50dc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50dc4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50dc4-110">Permission type</span></span>      | <span data-ttu-id="50dc4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50dc4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50dc4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50dc4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50dc4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50dc4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50dc4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50dc4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50dc4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50dc4-115">Not supported.</span></span>    |
|<span data-ttu-id="50dc4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50dc4-116">Application</span></span> | <span data-ttu-id="50dc4-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50dc4-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50dc4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50dc4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50dc4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50dc4-119">Optional query parameters</span></span>
<span data-ttu-id="50dc4-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50dc4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50dc4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50dc4-121">Request headers</span></span>
| <span data-ttu-id="50dc4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="50dc4-122">Name</span></span>       | <span data-ttu-id="50dc4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="50dc4-123">Type</span></span> | <span data-ttu-id="50dc4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="50dc4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="50dc4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="50dc4-125">Authorization</span></span>  | <span data-ttu-id="50dc4-126">string</span><span class="sxs-lookup"><span data-stu-id="50dc4-126">string</span></span>  | <span data-ttu-id="50dc4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50dc4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50dc4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50dc4-129">Request body</span></span>
<span data-ttu-id="50dc4-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50dc4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50dc4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="50dc4-131">Response</span></span>

<span data-ttu-id="50dc4-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50dc4-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50dc4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="50dc4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50dc4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="50dc4-134">Request</span></span>
<span data-ttu-id="50dc4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50dc4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
##### <a name="response"></a><span data-ttu-id="50dc4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="50dc4-136">Response</span></span>
<span data-ttu-id="50dc4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="50dc4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->