---
title: Получение приложения
description: Извлечение свойств и связи объекта приложения.
ms.openlocfilehash: 0ba50fa0a3fec2c1f9a6adce828e845f0c4d3b2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077589"
---
# <a name="get-application"></a><span data-ttu-id="378e4-103">Получение приложения</span><span class="sxs-lookup"><span data-stu-id="378e4-103">Get Application</span></span>

> <span data-ttu-id="378e4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="378e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="378e4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="378e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="378e4-106">Извлечение свойств и связи объекта приложения.</span><span class="sxs-lookup"><span data-stu-id="378e4-106">Retrieve the properties and relationships of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="378e4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="378e4-107">Permissions</span></span>
<span data-ttu-id="378e4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="378e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="378e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="378e4-110">Permission type</span></span>      | <span data-ttu-id="378e4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="378e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="378e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="378e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="378e4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="378e4-113">Not supported.</span></span>    |
|<span data-ttu-id="378e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="378e4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="378e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="378e4-115">Not supported.</span></span>    |
|<span data-ttu-id="378e4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="378e4-116">Application</span></span> | <span data-ttu-id="378e4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="378e4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="378e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="378e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="378e4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="378e4-119">Optional query parameters</span></span>
<span data-ttu-id="378e4-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="378e4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="378e4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="378e4-121">Request headers</span></span>
| <span data-ttu-id="378e4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="378e4-122">Name</span></span>      |<span data-ttu-id="378e4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="378e4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="378e4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="378e4-124">Authorization</span></span>  | <span data-ttu-id="378e4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="378e4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="378e4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="378e4-127">Request body</span></span>
<span data-ttu-id="378e4-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="378e4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="378e4-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="378e4-129">Response</span></span>

<span data-ttu-id="378e4-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [приложения](../resources/application.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="378e4-130">If successful, this method returns a `200 OK` response code and [Application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="378e4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="378e4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="378e4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="378e4-132">Request</span></span>
<span data-ttu-id="378e4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="378e4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="378e4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="378e4-134">Response</span></span>
<span data-ttu-id="378e4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="378e4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->