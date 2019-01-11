---
title: Создание appRoleAssignment
description: Используйте этот интерфейс API для создания нового appRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: ce498312f294ff11b97f12b136a6f48ebb4d3791
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886984"
---
# <a name="create-approleassignment"></a><span data-ttu-id="74488-103">Создание appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="74488-103">Create appRoleAssignment</span></span>

> <span data-ttu-id="74488-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74488-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74488-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74488-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74488-106">Используйте этот интерфейс API для создания нового appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="74488-106">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="74488-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74488-107">Permissions</span></span>
<span data-ttu-id="74488-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74488-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74488-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74488-110">Permission type</span></span>      | <span data-ttu-id="74488-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74488-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74488-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74488-112">Delegated (work or school account)</span></span> | <span data-ttu-id="74488-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74488-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="74488-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74488-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74488-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74488-115">Not supported.</span></span>    |
|<span data-ttu-id="74488-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74488-116">Application</span></span> | <span data-ttu-id="74488-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74488-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74488-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74488-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="74488-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74488-119">Request headers</span></span>
| <span data-ttu-id="74488-120">Имя</span><span class="sxs-lookup"><span data-stu-id="74488-120">Name</span></span>       | <span data-ttu-id="74488-121">Тип</span><span class="sxs-lookup"><span data-stu-id="74488-121">Type</span></span> | <span data-ttu-id="74488-122">Описание</span><span class="sxs-lookup"><span data-stu-id="74488-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74488-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74488-123">Authorization</span></span>  | <span data-ttu-id="74488-124">string</span><span class="sxs-lookup"><span data-stu-id="74488-124">string</span></span>  | <span data-ttu-id="74488-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74488-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74488-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74488-127">Request body</span></span>
<span data-ttu-id="74488-128">В тексте запроса укажите представление JSON объекта [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="74488-128">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="74488-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="74488-129">Response</span></span>

<span data-ttu-id="74488-130">Успешно завершена, этот метод возвращает `201 Created` объект [appRoleAssignment](../resources/approleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74488-130">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74488-131">Пример</span><span class="sxs-lookup"><span data-stu-id="74488-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74488-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="74488-132">Request</span></span>
<span data-ttu-id="74488-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74488-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
<span data-ttu-id="74488-134">В тексте запроса укажите представление JSON объекта [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="74488-134">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="74488-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="74488-135">Response</span></span>
<span data-ttu-id="74488-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="74488-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
