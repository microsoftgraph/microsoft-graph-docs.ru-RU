---
title: 'orgContact: член списка'
description: Получить список групп и администрирования единицы которой контакт.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5ad10bd9edce09849799540bcbfbfda90d7bb28
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920186"
---
# <a name="orgcontact-list-memberof"></a><span data-ttu-id="bb929-103">orgContact: член списка</span><span class="sxs-lookup"><span data-stu-id="bb929-103">orgContact: List memberOf</span></span>

> <span data-ttu-id="bb929-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb929-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb929-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb929-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb929-106">Получить список групп и администрирования единицы которой контакт.</span><span class="sxs-lookup"><span data-stu-id="bb929-106">Retrieve the list of groups and adminstrative units the contact is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb929-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb929-107">Permissions</span></span>
<span data-ttu-id="bb929-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb929-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb929-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb929-110">Permission type</span></span>      | <span data-ttu-id="bb929-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb929-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb929-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb929-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bb929-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb929-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb929-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb929-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb929-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb929-115">Not supported.</span></span>    |
|<span data-ttu-id="bb929-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb929-116">Application</span></span> | <span data-ttu-id="bb929-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb929-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb929-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb929-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb929-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bb929-119">Optional query parameters</span></span>
<span data-ttu-id="bb929-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bb929-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb929-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb929-121">Request headers</span></span>
| <span data-ttu-id="bb929-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bb929-122">Name</span></span>       | <span data-ttu-id="bb929-123">Тип</span><span class="sxs-lookup"><span data-stu-id="bb929-123">Type</span></span> | <span data-ttu-id="bb929-124">Описание</span><span class="sxs-lookup"><span data-stu-id="bb929-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb929-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb929-125">Authorization</span></span>  | <span data-ttu-id="bb929-126">string</span><span class="sxs-lookup"><span data-stu-id="bb929-126">string</span></span>  | <span data-ttu-id="bb929-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb929-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb929-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb929-129">Request body</span></span>
<span data-ttu-id="bb929-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb929-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb929-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb929-131">Response</span></span>

<span data-ttu-id="bb929-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb929-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb929-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bb929-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb929-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb929-134">Request</span></span>
<span data-ttu-id="bb929-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb929-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="bb929-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb929-136">Response</span></span>
<span data-ttu-id="bb929-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bb929-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
