---
title: Список oauth2PermissionGrants
description: Получение списка объектов oauth2PermissionGrant.
ms.openlocfilehash: 947041262ddac7ef0aab43ee455979ee0cf9bbf8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079452"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="f9e3d-103">Список oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="f9e3d-103">List oauth2PermissionGrants</span></span>

> <span data-ttu-id="f9e3d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f9e3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9e3d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9e3d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9e3d-106">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="f9e3d-106">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9e3d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9e3d-107">Permissions</span></span>

<span data-ttu-id="f9e3d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9e3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f9e3d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9e3d-110">Permission type</span></span>      | <span data-ttu-id="f9e3d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9e3d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9e3d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9e3d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9e3d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9e3d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f9e3d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9e3d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9e3d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9e3d-115">Not supported.</span></span>    |
|<span data-ttu-id="f9e3d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9e3d-116">Application</span></span> | <span data-ttu-id="f9e3d-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9e3d-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9e3d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9e3d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9e3d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9e3d-119">Optional query parameters</span></span>
<span data-ttu-id="f9e3d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9e3d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9e3d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9e3d-121">Request headers</span></span>
| <span data-ttu-id="f9e3d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f9e3d-122">Name</span></span> | <span data-ttu-id="f9e3d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f9e3d-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="f9e3d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9e3d-124">Authorization</span></span>  | <span data-ttu-id="f9e3d-125">string</span><span class="sxs-lookup"><span data-stu-id="f9e3d-125">string</span></span>  | <span data-ttu-id="f9e3d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9e3d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9e3d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9e3d-128">Request body</span></span>
<span data-ttu-id="f9e3d-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9e3d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9e3d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9e3d-130">Response</span></span>

<span data-ttu-id="f9e3d-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f9e3d-131">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9e3d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f9e3d-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f9e3d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9e3d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="f9e3d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9e3d-134">Response</span></span>

<span data-ttu-id="f9e3d-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9e3d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->