---
title: Получение oAuth2Permissiongrant
description: Получение свойств и связей объекта oAuth2Permissiongrant.
localization_priority: Normal
ms.openlocfilehash: 482d1f310b6eadcfe7df9e961af4ee4c229e9c12
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338221"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="6aef8-103">Получение oAuth2Permissiongrant</span><span class="sxs-lookup"><span data-stu-id="6aef8-103">Get oAuth2Permissiongrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6aef8-104">Получение свойств и связей объекта oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="6aef8-104">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6aef8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6aef8-105">Permissions</span></span>
<span data-ttu-id="6aef8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aef8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6aef8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aef8-108">Permission type</span></span>      | <span data-ttu-id="6aef8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aef8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6aef8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aef8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6aef8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6aef8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6aef8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aef8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aef8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aef8-113">Not supported.</span></span>    |
|<span data-ttu-id="6aef8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6aef8-114">Application</span></span> | <span data-ttu-id="6aef8-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aef8-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6aef8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6aef8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6aef8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6aef8-117">Optional query parameters</span></span>
<span data-ttu-id="6aef8-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6aef8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6aef8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6aef8-119">Request headers</span></span>
| <span data-ttu-id="6aef8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6aef8-120">Name</span></span>       | <span data-ttu-id="6aef8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6aef8-121">Type</span></span> | <span data-ttu-id="6aef8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6aef8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6aef8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aef8-123">Authorization</span></span>  | <span data-ttu-id="6aef8-124">string</span><span class="sxs-lookup"><span data-stu-id="6aef8-124">string</span></span>  | <span data-ttu-id="6aef8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aef8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6aef8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6aef8-127">Request body</span></span>
<span data-ttu-id="6aef8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6aef8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aef8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6aef8-129">Response</span></span>

<span data-ttu-id="6aef8-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6aef8-130">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6aef8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6aef8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6aef8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6aef8-132">Request</span></span>
<span data-ttu-id="6aef8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6aef8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```http
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="6aef8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aef8-134">Response</span></span>
<span data-ttu-id="6aef8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6aef8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "expiryTime": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
