---
title: Список workingWith
description: Вычисляемые insight для списка пользователей, которые пользователь работает с.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ca5fdd4602d109d98002c0ef54fde5ad341e1903
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521623"
---
# <a name="list-workingwith"></a><span data-ttu-id="5cf20-103">Список workingWith</span><span class="sxs-lookup"><span data-stu-id="5cf20-103">List workingWith</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cf20-104">Вычисляемые insight для списка пользователей, которые пользователь работает с.</span><span class="sxs-lookup"><span data-stu-id="5cf20-104">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cf20-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cf20-105">Permissions</span></span>
<span data-ttu-id="5cf20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cf20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cf20-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cf20-108">Permission type</span></span>      | <span data-ttu-id="5cf20-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cf20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cf20-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cf20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5cf20-111">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cf20-111">User.Read.All</span></span>    |
|<span data-ttu-id="5cf20-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cf20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cf20-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cf20-113">Not supported.</span></span>    |
|<span data-ttu-id="5cf20-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cf20-114">Application</span></span> | <span data-ttu-id="5cf20-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cf20-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cf20-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cf20-116">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5cf20-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5cf20-117">Optional query parameters</span></span>
<span data-ttu-id="5cf20-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5cf20-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cf20-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cf20-119">Request headers</span></span>
| <span data-ttu-id="5cf20-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cf20-120">Header</span></span>         | <span data-ttu-id="5cf20-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5cf20-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="5cf20-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cf20-122">Authorization</span></span>  | <span data-ttu-id="5cf20-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cf20-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5cf20-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5cf20-125">Content-Type</span></span>   | <span data-ttu-id="5cf20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cf20-126">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="5cf20-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cf20-127">Request body</span></span>
<span data-ttu-id="5cf20-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5cf20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cf20-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cf20-129">Response</span></span>

<span data-ttu-id="5cf20-130">Если успешно завершена, этот метод возвращает 200 OK ответа код и коллекцию объектов- [пользователей](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5cf20-130">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cf20-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5cf20-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cf20-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cf20-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="5cf20-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cf20-133">Response</span></span>
<span data-ttu-id="5cf20-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5cf20-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "id": "id-value",
  "preferredName": "preferredName-value",
  "Email": "Email-value",
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-workingwith.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
