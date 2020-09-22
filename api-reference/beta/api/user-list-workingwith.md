---
title: Список workingWith
description: Вычисляемое представление о списке пользователей, с которыми работает пользователь.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ce7c0e915105ff837c1a96185610553123fc82c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024712"
---
# <a name="list-workingwith"></a><span data-ttu-id="4b97c-103">Список workingWith</span><span class="sxs-lookup"><span data-stu-id="4b97c-103">List workingWith</span></span>

<span data-ttu-id="4b97c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b97c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b97c-105">Вычисляемое представление о списке пользователей, с которыми работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="4b97c-105">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b97c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b97c-106">Permissions</span></span>
<span data-ttu-id="4b97c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b97c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b97c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b97c-109">Permission type</span></span>      | <span data-ttu-id="4b97c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b97c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b97c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b97c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b97c-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b97c-112">User.Read.All</span></span>    |
|<span data-ttu-id="4b97c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b97c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b97c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b97c-114">Not supported.</span></span>    |
|<span data-ttu-id="4b97c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b97c-115">Application</span></span> | <span data-ttu-id="4b97c-116">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b97c-116">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b97c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b97c-117">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4b97c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4b97c-118">Optional query parameters</span></span>
<span data-ttu-id="4b97c-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4b97c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b97c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b97c-120">Request headers</span></span>
| <span data-ttu-id="4b97c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b97c-121">Header</span></span>         | <span data-ttu-id="4b97c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b97c-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="4b97c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b97c-123">Authorization</span></span>  | <span data-ttu-id="4b97c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b97c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4b97c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b97c-126">Content-Type</span></span>   | <span data-ttu-id="4b97c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4b97c-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="4b97c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b97c-128">Request body</span></span>
<span data-ttu-id="4b97c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b97c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b97c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b97c-130">Response</span></span>

<span data-ttu-id="4b97c-131">В случае успешного выполнения этот метод возвращает код ответа 200 ОК и коллекцию объектов [User](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b97c-131">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b97c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4b97c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b97c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b97c-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="4b97c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b97c-134">Response</span></span>
<span data-ttu-id="4b97c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b97c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


