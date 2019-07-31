---
title: Список workingWith
description: Вычисляемое представление о списке пользователей, с которыми работает пользователь.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 587a9e34db293a738e1242b3d41406bb15990834
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987483"
---
# <a name="list-workingwith"></a><span data-ttu-id="4ce85-103">Список workingWith</span><span class="sxs-lookup"><span data-stu-id="4ce85-103">List workingWith</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ce85-104">Вычисляемое представление о списке пользователей, с которыми работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="4ce85-104">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ce85-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ce85-105">Permissions</span></span>
<span data-ttu-id="4ce85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ce85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ce85-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ce85-108">Permission type</span></span>      | <span data-ttu-id="4ce85-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ce85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ce85-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ce85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ce85-111">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ce85-111">User.Read.All</span></span>    |
|<span data-ttu-id="4ce85-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ce85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ce85-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ce85-113">Not supported.</span></span>    |
|<span data-ttu-id="4ce85-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ce85-114">Application</span></span> | <span data-ttu-id="4ce85-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ce85-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ce85-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ce85-116">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ce85-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ce85-117">Optional query parameters</span></span>
<span data-ttu-id="4ce85-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ce85-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ce85-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ce85-119">Request headers</span></span>
| <span data-ttu-id="4ce85-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ce85-120">Header</span></span>         | <span data-ttu-id="4ce85-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4ce85-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="4ce85-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ce85-122">Authorization</span></span>  | <span data-ttu-id="4ce85-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ce85-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4ce85-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ce85-125">Content-Type</span></span>   | <span data-ttu-id="4ce85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ce85-126">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="4ce85-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ce85-127">Request body</span></span>
<span data-ttu-id="4ce85-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ce85-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ce85-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ce85-129">Response</span></span>

<span data-ttu-id="4ce85-130">В случае успешного выполнения этот метод возвращает код ответа 200 ОК и коллекцию объектов [User](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ce85-130">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ce85-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4ce85-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ce85-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ce85-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="4ce85-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ce85-133">Response</span></span>
<span data-ttu-id="4ce85-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ce85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
