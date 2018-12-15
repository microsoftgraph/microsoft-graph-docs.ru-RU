---
title: Список orgContacts
description: Получить список организационных контакты для данной организации.
ms.openlocfilehash: 01be5350898bed181f2e1d304bf58f8ec1e4e47f
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283628"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="f2f95-103">Список orgContacts</span><span class="sxs-lookup"><span data-stu-id="f2f95-103">List orgContacts</span></span>

> <span data-ttu-id="f2f95-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2f95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2f95-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2f95-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2f95-106">Получить список организационных контакты для данной организации.</span><span class="sxs-lookup"><span data-stu-id="f2f95-106">Retrieve the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2f95-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2f95-107">Permissions</span></span>
<span data-ttu-id="f2f95-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2f95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2f95-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2f95-110">Permission type</span></span>      | <span data-ttu-id="f2f95-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2f95-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2f95-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2f95-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2f95-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2f95-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2f95-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2f95-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2f95-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2f95-115">Not supported.</span></span>    |
|<span data-ttu-id="f2f95-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2f95-116">Application</span></span> | <span data-ttu-id="f2f95-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2f95-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2f95-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2f95-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f2f95-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2f95-119">Optional query parameters</span></span>
<span data-ttu-id="f2f95-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2f95-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2f95-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2f95-121">Request headers</span></span>
| <span data-ttu-id="f2f95-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f2f95-122">Name</span></span>       | <span data-ttu-id="f2f95-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f2f95-123">Type</span></span> | <span data-ttu-id="f2f95-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f95-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f2f95-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2f95-125">Authorization</span></span>  | <span data-ttu-id="f2f95-126">строка</span><span class="sxs-lookup"><span data-stu-id="f2f95-126">string</span></span>  | <span data-ttu-id="f2f95-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2f95-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2f95-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2f95-129">Request body</span></span>
<span data-ttu-id="f2f95-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2f95-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2f95-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2f95-131">Response</span></span>

<span data-ttu-id="f2f95-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [orgContact](../resources/orgcontact.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f2f95-132">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2f95-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f2f95-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2f95-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2f95-134">Request</span></span>
<span data-ttu-id="f2f95-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2f95-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts
```
##### <a name="response"></a><span data-ttu-id="f2f95-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2f95-136">Response</span></span>
<span data-ttu-id="f2f95-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f2f95-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "addresses":[
          {
            "city": "string",
            "countryOrRegion": "string",
            "officeLocation": "string",
            "postalCode": "string",
            "state": "string",
            "street": "string"
          }
      ],
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "phones":[
          {
            "type": "string",
            "number": "string"
          }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->