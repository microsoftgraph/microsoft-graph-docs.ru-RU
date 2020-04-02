---
title: Список workingWith
description: Вычисляемое представление о списке пользователей, с которыми работает пользователь.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 806aa9e1f6a95d5f1d723714869546ea3943c725
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107537"
---
# <a name="list-workingwith"></a><span data-ttu-id="bf47f-103">Список workingWith</span><span class="sxs-lookup"><span data-stu-id="bf47f-103">List workingWith</span></span>

<span data-ttu-id="bf47f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf47f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf47f-105">Вычисляемое представление о списке пользователей, с которыми работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="bf47f-105">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf47f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf47f-106">Permissions</span></span>
<span data-ttu-id="bf47f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf47f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf47f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf47f-109">Permission type</span></span>      | <span data-ttu-id="bf47f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf47f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf47f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf47f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf47f-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf47f-112">User.Read.All</span></span>    |
|<span data-ttu-id="bf47f-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf47f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf47f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf47f-114">Not supported.</span></span>    |
|<span data-ttu-id="bf47f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf47f-115">Application</span></span> | <span data-ttu-id="bf47f-116">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf47f-116">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf47f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf47f-117">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bf47f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bf47f-118">Optional query parameters</span></span>
<span data-ttu-id="bf47f-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bf47f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf47f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf47f-120">Request headers</span></span>
| <span data-ttu-id="bf47f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf47f-121">Header</span></span>         | <span data-ttu-id="bf47f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bf47f-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="bf47f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf47f-123">Authorization</span></span>  | <span data-ttu-id="bf47f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf47f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf47f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf47f-126">Content-Type</span></span>   | <span data-ttu-id="bf47f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bf47f-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="bf47f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bf47f-128">Request body</span></span>
<span data-ttu-id="bf47f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf47f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf47f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf47f-130">Response</span></span>

<span data-ttu-id="bf47f-131">В случае успешного выполнения этот метод возвращает код ответа 200 ОК и коллекцию объектов [User](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf47f-131">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf47f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bf47f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf47f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf47f-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="bf47f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf47f-134">Response</span></span>
<span data-ttu-id="bf47f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf47f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
