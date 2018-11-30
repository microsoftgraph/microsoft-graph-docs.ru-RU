---
title: Получение oAuth2Permissiongrant
description: Извлечение свойств и связи объекта oAuth2Permissiongrant.
ms.openlocfilehash: f5df8e647c2e71df67f7ac3fad6a81e8f2383f8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078726"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="22e6f-103">Получение oAuth2Permissiongrant</span><span class="sxs-lookup"><span data-stu-id="22e6f-103">Get oAuth2Permissiongrant</span></span>

> <span data-ttu-id="22e6f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22e6f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22e6f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22e6f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22e6f-106">Извлечение свойств и связи объекта oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="22e6f-106">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22e6f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22e6f-107">Permissions</span></span>
<span data-ttu-id="22e6f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22e6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="22e6f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22e6f-110">Permission type</span></span>      | <span data-ttu-id="22e6f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22e6f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22e6f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22e6f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="22e6f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22e6f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22e6f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22e6f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22e6f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22e6f-115">Not supported.</span></span>    |
|<span data-ttu-id="22e6f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22e6f-116">Application</span></span> | <span data-ttu-id="22e6f-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22e6f-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22e6f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22e6f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="22e6f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22e6f-119">Optional query parameters</span></span>
<span data-ttu-id="22e6f-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="22e6f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22e6f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22e6f-121">Request headers</span></span>
| <span data-ttu-id="22e6f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="22e6f-122">Name</span></span>       | <span data-ttu-id="22e6f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="22e6f-123">Type</span></span> | <span data-ttu-id="22e6f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="22e6f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="22e6f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="22e6f-125">Authorization</span></span>  | <span data-ttu-id="22e6f-126">string</span><span class="sxs-lookup"><span data-stu-id="22e6f-126">string</span></span>  | <span data-ttu-id="22e6f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22e6f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22e6f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22e6f-129">Request body</span></span>
<span data-ttu-id="22e6f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22e6f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22e6f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="22e6f-131">Response</span></span>

<span data-ttu-id="22e6f-132">Успешно завершена, этот метод возвращает `200 OK` объект [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="22e6f-132">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="22e6f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="22e6f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22e6f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="22e6f-134">Request</span></span>
<span data-ttu-id="22e6f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22e6f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```http
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="22e6f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="22e6f-136">Response</span></span>
<span data-ttu-id="22e6f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="22e6f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
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
<!-- {
  "type": "#page.annotation",
  "description": "Get oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->