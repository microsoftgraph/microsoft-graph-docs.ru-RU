---
title: Список workingWith
description: Вычисляемые insight для списка пользователей, которые пользователь работает с.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: df7f84bf42887d9052cb9d81042b5735af7bd2b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870338"
---
# <a name="list-workingwith"></a><span data-ttu-id="7ed99-103">Список workingWith</span><span class="sxs-lookup"><span data-stu-id="7ed99-103">List workingWith</span></span>

> <span data-ttu-id="7ed99-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ed99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ed99-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ed99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ed99-106">Вычисляемые insight для списка пользователей, которые пользователь работает с.</span><span class="sxs-lookup"><span data-stu-id="7ed99-106">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ed99-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ed99-107">Permissions</span></span>
<span data-ttu-id="7ed99-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ed99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ed99-110">Permission type</span></span>      | <span data-ttu-id="7ed99-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ed99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ed99-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ed99-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ed99-113">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ed99-113">User.Read.All</span></span>    |
|<span data-ttu-id="7ed99-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ed99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ed99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ed99-115">Not supported.</span></span>    |
|<span data-ttu-id="7ed99-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ed99-116">Application</span></span> | <span data-ttu-id="7ed99-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ed99-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ed99-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ed99-118">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ed99-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7ed99-119">Optional query parameters</span></span>
<span data-ttu-id="7ed99-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7ed99-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ed99-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ed99-121">Request headers</span></span>
| <span data-ttu-id="7ed99-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ed99-122">Header</span></span>         | <span data-ttu-id="7ed99-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7ed99-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="7ed99-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ed99-124">Authorization</span></span>  | <span data-ttu-id="7ed99-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ed99-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ed99-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ed99-127">Content-Type</span></span>   | <span data-ttu-id="7ed99-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7ed99-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="7ed99-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ed99-129">Request body</span></span>
<span data-ttu-id="7ed99-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ed99-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ed99-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ed99-131">Response</span></span>

<span data-ttu-id="7ed99-132">Если успешно завершена, этот метод возвращает 200 OK ответа код и коллекцию объектов- [пользователей](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7ed99-132">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ed99-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7ed99-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ed99-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ed99-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="7ed99-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ed99-135">Response</span></span>
<span data-ttu-id="7ed99-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7ed99-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
