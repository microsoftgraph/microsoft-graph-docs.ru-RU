---
title: Получение организации
description: Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.
localization_priority: Priority
ms.openlocfilehash: f2fc708ea2d1841987f8b2a757a5388735227007
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871199"
---
# <a name="get-organization"></a><span data-ttu-id="ee94e-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="ee94e-103">Get organization</span></span>

<span data-ttu-id="ee94e-104">Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="ee94e-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee94e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee94e-105">Permissions</span></span>

<span data-ttu-id="ee94e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee94e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee94e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee94e-108">Permission type</span></span>      | <span data-ttu-id="ee94e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee94e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee94e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee94e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee94e-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee94e-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="ee94e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee94e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee94e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee94e-113">Not supported.</span></span>    |
|<span data-ttu-id="ee94e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee94e-114">Application</span></span> | <span data-ttu-id="ee94e-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee94e-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ee94e-116">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="ee94e-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="ee94e-117">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="ee94e-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="ee94e-118">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="ee94e-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="ee94e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee94e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee94e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee94e-120">Optional query parameters</span></span>

<span data-ttu-id="ee94e-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee94e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee94e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee94e-122">Request headers</span></span>

| <span data-ttu-id="ee94e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ee94e-123">Name</span></span>       | <span data-ttu-id="ee94e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ee94e-124">Type</span></span> | <span data-ttu-id="ee94e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ee94e-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ee94e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee94e-126">Authorization</span></span>  | <span data-ttu-id="ee94e-127">string</span><span class="sxs-lookup"><span data-stu-id="ee94e-127">string</span></span>  | <span data-ttu-id="ee94e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee94e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee94e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee94e-130">Request body</span></span>

<span data-ttu-id="ee94e-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee94e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee94e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee94e-132">Response</span></span>

<span data-ttu-id="ee94e-133">Успешно завершена, этот метод возвращает `200 OK` код ответа и семейства сайтов из одного объекта [организации](../resources/organization.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ee94e-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee94e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ee94e-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee94e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee94e-135">Request</span></span>

<span data-ttu-id="ee94e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee94e-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```

##### <a name="response"></a><span data-ttu-id="ee94e-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee94e-137">Response</span></span>

<span data-ttu-id="ee94e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ee94e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
