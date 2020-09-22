---
title: 'Привилежедролеассигнмент: My'
description: Получение привилегированных назначений ролей запрашивающей стороны.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: fdcde1ab1b3bd5f901c2d4e05cc23ce7f6ef9023
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035038"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="cf92c-103">Привилежедролеассигнмент: My</span><span class="sxs-lookup"><span data-stu-id="cf92c-103">privilegedRoleAssignment: my</span></span>

<span data-ttu-id="cf92c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf92c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf92c-105">Получение привилегированных назначений ролей запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="cf92c-105">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf92c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf92c-106">Permissions</span></span>
<span data-ttu-id="cf92c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf92c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf92c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf92c-109">Permission type</span></span>      | <span data-ttu-id="cf92c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf92c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf92c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf92c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf92c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cf92c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cf92c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf92c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf92c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf92c-114">Not supported.</span></span>    |
|<span data-ttu-id="cf92c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf92c-115">Application</span></span> | <span data-ttu-id="cf92c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf92c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf92c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf92c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="cf92c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf92c-118">Request headers</span></span>
| <span data-ttu-id="cf92c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cf92c-119">Name</span></span>       | <span data-ttu-id="cf92c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cf92c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cf92c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf92c-121">Authorization</span></span>  | <span data-ttu-id="cf92c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf92c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf92c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf92c-124">Request body</span></span>
<span data-ttu-id="cf92c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf92c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf92c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf92c-126">Response</span></span>

<span data-ttu-id="cf92c-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf92c-127">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf92c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="cf92c-128">Example</span></span>
<span data-ttu-id="cf92c-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cf92c-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cf92c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf92c-130">Request</span></span>
<span data-ttu-id="cf92c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf92c-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf92c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf92c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```
# <a name="c"></a>[<span data-ttu-id="cf92c-133">C#</span><span class="sxs-lookup"><span data-stu-id="cf92c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf92c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf92c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf92c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf92c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cf92c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf92c-136">Response</span></span>
<span data-ttu-id="cf92c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf92c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


