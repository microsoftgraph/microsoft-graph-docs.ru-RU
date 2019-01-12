---
title: Получение категории Outlook
description: Получение свойств и отношений указанного объекта outlookCategory.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c296aea62fec7090cb76607911f6be178f1ebdbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949719"
---
# <a name="get-outlook-category"></a><span data-ttu-id="eb562-103">Получение категории Outlook</span><span class="sxs-lookup"><span data-stu-id="eb562-103">Get Outlook category</span></span>

> <span data-ttu-id="eb562-104">**Важно**: интерфейсы API в разделе версии /beta в Microsoft Graph в предварительной версии и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eb562-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb562-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb562-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb562-106">Получение свойств и отношений указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="eb562-106">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb562-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb562-107">Permissions</span></span>
<span data-ttu-id="eb562-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb562-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb562-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb562-110">Permission type</span></span>      | <span data-ttu-id="eb562-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb562-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb562-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb562-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb562-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="eb562-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="eb562-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb562-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb562-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="eb562-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="eb562-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb562-116">Application</span></span> | <span data-ttu-id="eb562-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="eb562-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb562-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb562-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eb562-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb562-119">Optional query parameters</span></span>
<span data-ttu-id="eb562-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eb562-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb562-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb562-121">Request headers</span></span>
| <span data-ttu-id="eb562-122">Имя</span><span class="sxs-lookup"><span data-stu-id="eb562-122">Name</span></span>      |<span data-ttu-id="eb562-123">Описание</span><span class="sxs-lookup"><span data-stu-id="eb562-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb562-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb562-124">Authorization</span></span>  | <span data-ttu-id="eb562-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb562-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb562-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb562-127">Request body</span></span>
<span data-ttu-id="eb562-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb562-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb562-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb562-129">Response</span></span>

<span data-ttu-id="eb562-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [outlookCategory](../resources/outlookcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eb562-130">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb562-131">Пример</span><span class="sxs-lookup"><span data-stu-id="eb562-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb562-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb562-132">Request</span></span>
<span data-ttu-id="eb562-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb562-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories('de912e4d-c790-4da9-949c-ccd933aaa0f7')
```
##### <a name="response"></a><span data-ttu-id="eb562-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb562-134">Response</span></span>
<span data-ttu-id="eb562-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eb562-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
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
