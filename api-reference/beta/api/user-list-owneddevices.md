---
title: Список ownedDevices
description: Получение списка устройств, принадлежащих пользователю.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9956d61bace31f9a4dc51f8e8a7aa2855bfb19b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334797"
---
# <a name="list-owneddevices"></a><span data-ttu-id="33dbc-103">Список ownedDevices</span><span class="sxs-lookup"><span data-stu-id="33dbc-103">List ownedDevices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33dbc-104">Получение списка устройств, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="33dbc-104">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="33dbc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33dbc-105">Permissions</span></span>
<span data-ttu-id="33dbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33dbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33dbc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33dbc-108">Permission type</span></span>      | <span data-ttu-id="33dbc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33dbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33dbc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33dbc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="33dbc-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33dbc-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33dbc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33dbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33dbc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33dbc-113">Not supported.</span></span>    |
|<span data-ttu-id="33dbc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33dbc-114">Application</span></span> | <span data-ttu-id="33dbc-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33dbc-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33dbc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33dbc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="33dbc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="33dbc-117">Optional query parameters</span></span>
<span data-ttu-id="33dbc-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="33dbc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="33dbc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33dbc-119">Request headers</span></span>
| <span data-ttu-id="33dbc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33dbc-120">Header</span></span>       | <span data-ttu-id="33dbc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33dbc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="33dbc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33dbc-122">Authorization</span></span>  | <span data-ttu-id="33dbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33dbc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="33dbc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33dbc-125">Accept</span></span>  | <span data-ttu-id="33dbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33dbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33dbc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33dbc-127">Request body</span></span>
<span data-ttu-id="33dbc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33dbc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33dbc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="33dbc-129">Response</span></span>

<span data-ttu-id="33dbc-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33dbc-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33dbc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="33dbc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33dbc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="33dbc-132">Request</span></span>
<span data-ttu-id="33dbc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33dbc-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```http
GET https://graph.microsoft.com/beta/me/ownedDevices
```
##### <a name="response"></a><span data-ttu-id="33dbc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="33dbc-134">Response</span></span>
<span data-ttu-id="33dbc-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33dbc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List ownedDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
