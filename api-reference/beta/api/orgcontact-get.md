---
title: Получение orgContact
description: Извлечение свойств и связи объекта orgcontact.
ms.openlocfilehash: 178d670c55cdd904c604e1be1f6fb0aef3a4b953
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076085"
---
# <a name="get-orgcontact"></a><span data-ttu-id="1ff5c-103">Получение orgContact</span><span class="sxs-lookup"><span data-stu-id="1ff5c-103">Get orgContact</span></span>

> <span data-ttu-id="1ff5c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1ff5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ff5c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ff5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1ff5c-106">Извлечение свойств и связи объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="1ff5c-106">Retrieve the properties and relationships of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ff5c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ff5c-107">Permissions</span></span>
<span data-ttu-id="1ff5c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ff5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ff5c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ff5c-110">Permission type</span></span>      | <span data-ttu-id="1ff5c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ff5c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ff5c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ff5c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1ff5c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1ff5c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1ff5c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ff5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ff5c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ff5c-115">Not supported.</span></span>    |
|<span data-ttu-id="1ff5c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ff5c-116">Application</span></span> | <span data-ttu-id="1ff5c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ff5c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ff5c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ff5c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1ff5c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1ff5c-119">Optional query parameters</span></span>
<span data-ttu-id="1ff5c-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1ff5c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ff5c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ff5c-121">Request headers</span></span>
| <span data-ttu-id="1ff5c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1ff5c-122">Name</span></span>       | <span data-ttu-id="1ff5c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="1ff5c-123">Type</span></span> | <span data-ttu-id="1ff5c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1ff5c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1ff5c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ff5c-125">Authorization</span></span>  | <span data-ttu-id="1ff5c-126">string</span><span class="sxs-lookup"><span data-stu-id="1ff5c-126">string</span></span>  | <span data-ttu-id="1ff5c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ff5c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ff5c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ff5c-129">Request body</span></span>
<span data-ttu-id="1ff5c-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ff5c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ff5c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ff5c-131">Response</span></span>

<span data-ttu-id="1ff5c-132">Успешно завершена, этот метод возвращает `200 OK` объект [orgContact](../resources/orgcontact.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1ff5c-132">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ff5c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1ff5c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ff5c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ff5c-134">Request</span></span>
<span data-ttu-id="1ff5c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ff5c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="1ff5c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ff5c-136">Response</span></span>
<span data-ttu-id="1ff5c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1ff5c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->