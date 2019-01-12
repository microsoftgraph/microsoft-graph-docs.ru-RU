---
title: Получение категории Outlook
description: Получение свойств и отношений указанного объекта outlookCategory.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4359c3bd87a5eecc3d8b153538b15039ab8be7c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934907"
---
# <a name="get-outlook-category"></a><span data-ttu-id="a63e6-103">Получение категории Outlook</span><span class="sxs-lookup"><span data-stu-id="a63e6-103">Get Outlook category</span></span>


<span data-ttu-id="a63e6-104">Получение свойств и отношений указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="a63e6-104">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a63e6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a63e6-105">Permissions</span></span>
<span data-ttu-id="a63e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a63e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a63e6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a63e6-108">Permission type</span></span>      | <span data-ttu-id="a63e6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a63e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a63e6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a63e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a63e6-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="a63e6-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="a63e6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a63e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a63e6-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="a63e6-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="a63e6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a63e6-114">Application</span></span> | <span data-ttu-id="a63e6-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="a63e6-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a63e6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a63e6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a63e6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a63e6-117">Optional query parameters</span></span>
<span data-ttu-id="a63e6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a63e6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a63e6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a63e6-119">Request headers</span></span>
| <span data-ttu-id="a63e6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a63e6-120">Name</span></span>      |<span data-ttu-id="a63e6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a63e6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a63e6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a63e6-122">Authorization</span></span>  | <span data-ttu-id="a63e6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a63e6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a63e6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a63e6-125">Request body</span></span>
<span data-ttu-id="a63e6-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a63e6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a63e6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a63e6-127">Response</span></span>

<span data-ttu-id="a63e6-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [outlookCategory](../resources/outlookcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a63e6-128">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a63e6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a63e6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a63e6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a63e6-130">Request</span></span>
<span data-ttu-id="a63e6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a63e6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["de912e4d-c790-4da9-949c-ccd933aaa0f7"],
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
##### <a name="response"></a><span data-ttu-id="a63e6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a63e6-132">Response</span></span>
<span data-ttu-id="a63e6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a63e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
