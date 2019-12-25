---
title: Перечисление транзитивных групп устройств
description: Получение групп, участником которых является устройство. Этот запрос API является транзитивным, а также возвращает все группы, в которых устройство является вложенным членом.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7fa76e01aa6e60681ba0873d7d0285e493dd3573
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868690"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="9fce2-104">Перечисление транзитивных групп устройств</span><span class="sxs-lookup"><span data-stu-id="9fce2-104">List device transitive groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fce2-105">Получение групп, участником которых является устройство.</span><span class="sxs-lookup"><span data-stu-id="9fce2-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="9fce2-106">Этот запрос API является транзитивным, а также возвращает все группы, в которых устройство является вложенным членом.</span><span class="sxs-lookup"><span data-stu-id="9fce2-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fce2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fce2-107">Permissions</span></span>

<span data-ttu-id="9fce2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fce2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fce2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fce2-110">Permission type</span></span>      | <span data-ttu-id="9fce2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fce2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fce2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fce2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9fce2-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9fce2-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9fce2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fce2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fce2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fce2-115">Not supported.</span></span>    |
|<span data-ttu-id="9fce2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fce2-116">Application</span></span> | <span data-ttu-id="9fce2-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fce2-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]


## <a name="http-request"></a><span data-ttu-id="9fce2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fce2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9fce2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9fce2-119">Optional query parameters</span></span>

<span data-ttu-id="9fce2-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9fce2-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9fce2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fce2-121">Request headers</span></span>

| <span data-ttu-id="9fce2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fce2-122">Header</span></span>       | <span data-ttu-id="9fce2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9fce2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9fce2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fce2-124">Authorization</span></span>  | <span data-ttu-id="9fce2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fce2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9fce2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9fce2-127">Accept</span></span>  | <span data-ttu-id="9fce2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9fce2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fce2-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fce2-129">Request body</span></span>

<span data-ttu-id="9fce2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fce2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fce2-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fce2-131">Response</span></span>

<span data-ttu-id="9fce2-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fce2-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fce2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9fce2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fce2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fce2-134">Request</span></span>

<span data-ttu-id="9fce2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fce2-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9fce2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fce2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fce2-137">C#</span><span class="sxs-lookup"><span data-stu-id="9fce2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fce2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fce2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fce2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fce2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9fce2-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fce2-140">Response</span></span>

<span data-ttu-id="9fce2-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fce2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
