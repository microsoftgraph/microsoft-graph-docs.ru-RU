---
title: Получение appRoleAssignment
description: Извлечение свойств и связи объекта approleassignment.
localization_priority: Priority
ms.openlocfilehash: 465ef0365bee8c1dd002fa423232cc615fc45635
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809662"
---
# <a name="get-approleassignment"></a><span data-ttu-id="0c6f9-103">Получение appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0c6f9-103">Get appRoleAssignment</span></span>

> <span data-ttu-id="0c6f9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c6f9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c6f9-106">Извлечение свойств и связи объекта approleassignment.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-106">Retrieve the properties and relationships of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c6f9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c6f9-107">Permissions</span></span>
<span data-ttu-id="0c6f9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c6f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c6f9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c6f9-110">Permission type</span></span>      | <span data-ttu-id="0c6f9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c6f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c6f9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c6f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0c6f9-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c6f9-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0c6f9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c6f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c6f9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-115">Not supported.</span></span>    |
|<span data-ttu-id="0c6f9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c6f9-116">Application</span></span> | <span data-ttu-id="0c6f9-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c6f9-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c6f9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c6f9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignedTo
GET /groups/{id}/appRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0c6f9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0c6f9-119">Optional query parameters</span></span>
<span data-ttu-id="0c6f9-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c6f9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c6f9-121">Request headers</span></span>
| <span data-ttu-id="0c6f9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0c6f9-122">Name</span></span>       | <span data-ttu-id="0c6f9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0c6f9-123">Type</span></span> | <span data-ttu-id="0c6f9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0c6f9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0c6f9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c6f9-125">Authorization</span></span>  | <span data-ttu-id="0c6f9-126">string</span><span class="sxs-lookup"><span data-stu-id="0c6f9-126">string</span></span>  | <span data-ttu-id="0c6f9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c6f9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c6f9-129">Request body</span></span>
<span data-ttu-id="0c6f9-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c6f9-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c6f9-131">Response</span></span>

<span data-ttu-id="0c6f9-132">Успешно завершена, этот метод возвращает `200 OK` объект [appRoleAssignment](../resources/approleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-132">If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c6f9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0c6f9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c6f9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c6f9-134">Request</span></span>
<span data-ttu-id="0c6f9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="0c6f9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c6f9-136">Response</span></span>
<span data-ttu-id="0c6f9-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0c6f9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
