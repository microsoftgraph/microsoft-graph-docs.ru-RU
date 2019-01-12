---
title: Получение организации
description: Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c4f0b325100ac8543e51320609e8c4e39ce130fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915454"
---
# <a name="get-organization"></a><span data-ttu-id="41e13-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="41e13-103">Get organization</span></span>

> <span data-ttu-id="41e13-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="41e13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41e13-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41e13-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41e13-106">Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="41e13-106">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="41e13-107">Поскольку ресурсов **организации** поддерживает [расширения](/graph/extensibility-overview), вы также можете использовать `GET` операции для получения данных расширения и настраиваемых свойств в экземпляре **организации** .</span><span class="sxs-lookup"><span data-stu-id="41e13-107">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="41e13-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41e13-108">Permissions</span></span>

<span data-ttu-id="41e13-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41e13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41e13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41e13-111">Permission type</span></span> | <span data-ttu-id="41e13-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41e13-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41e13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41e13-113">Delegated (work or school account)</span></span> | <span data-ttu-id="41e13-114">User.Read, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41e13-114">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="41e13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41e13-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41e13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41e13-116">Not supported.</span></span> |
|<span data-ttu-id="41e13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41e13-117">Application</span></span> | <span data-ttu-id="41e13-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41e13-118">Directory.Read.All</span></span> |

> <span data-ttu-id="41e13-119">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="41e13-119">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="41e13-120">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="41e13-120">All other properties will return with `null` values.</span></span> <span data-ttu-id="41e13-121">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="41e13-121">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="41e13-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41e13-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41e13-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="41e13-123">Optional query parameters</span></span>

<span data-ttu-id="41e13-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="41e13-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41e13-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41e13-125">Request headers</span></span>

| <span data-ttu-id="41e13-126">Имя</span><span class="sxs-lookup"><span data-stu-id="41e13-126">Name</span></span>       | <span data-ttu-id="41e13-127">Тип</span><span class="sxs-lookup"><span data-stu-id="41e13-127">Type</span></span> | <span data-ttu-id="41e13-128">Описание</span><span class="sxs-lookup"><span data-stu-id="41e13-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41e13-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="41e13-129">Authorization</span></span>  | <span data-ttu-id="41e13-130">строка</span><span class="sxs-lookup"><span data-stu-id="41e13-130">string</span></span>  | <span data-ttu-id="41e13-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41e13-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41e13-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41e13-133">Request body</span></span>

<span data-ttu-id="41e13-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41e13-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41e13-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="41e13-135">Response</span></span>

<span data-ttu-id="41e13-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41e13-136">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e13-137">Пример</span><span class="sxs-lookup"><span data-stu-id="41e13-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="41e13-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="41e13-138">Request</span></span>

<span data-ttu-id="41e13-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41e13-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="41e13-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="41e13-140">Response</span></span>

<span data-ttu-id="41e13-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="41e13-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization",
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

## <a name="see-also"></a><span data-ttu-id="41e13-144">См. также</span><span class="sxs-lookup"><span data-stu-id="41e13-144">See also</span></span>

- [<span data-ttu-id="41e13-145">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="41e13-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="41e13-146">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="41e13-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
