---
title: Перечисление транзитивных групп устройств
description: Получение групп, участником которых является устройство. Этот запрос API является транзитивным, а также возвращает все группы, в которых устройство является вложенным членом.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93d27fcfc4163afbe5b833a2f510365d8093fbc3
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656316"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="553b7-104">Перечисление транзитивных групп устройств</span><span class="sxs-lookup"><span data-stu-id="553b7-104">List device transitive groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="553b7-105">Получение групп, участником которых является устройство.</span><span class="sxs-lookup"><span data-stu-id="553b7-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="553b7-106">Этот запрос API является транзитивным, а также возвращает все группы, в которых устройство является вложенным членом.</span><span class="sxs-lookup"><span data-stu-id="553b7-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="553b7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="553b7-107">Permissions</span></span>

<span data-ttu-id="553b7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="553b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="553b7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="553b7-110">Permission type</span></span>      | <span data-ttu-id="553b7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="553b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="553b7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="553b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="553b7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="553b7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="553b7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="553b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="553b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="553b7-115">Not supported.</span></span>    |
|<span data-ttu-id="553b7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="553b7-116">Application</span></span> | <span data-ttu-id="553b7-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="553b7-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="553b7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="553b7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="553b7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="553b7-119">Optional query parameters</span></span>

<span data-ttu-id="553b7-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="553b7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="553b7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="553b7-121">Request headers</span></span>

| <span data-ttu-id="553b7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="553b7-122">Header</span></span>       | <span data-ttu-id="553b7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="553b7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="553b7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="553b7-124">Authorization</span></span>  | <span data-ttu-id="553b7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="553b7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="553b7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="553b7-127">Accept</span></span>  | <span data-ttu-id="553b7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="553b7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="553b7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="553b7-129">Request body</span></span>

<span data-ttu-id="553b7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="553b7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="553b7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="553b7-131">Response</span></span>

<span data-ttu-id="553b7-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="553b7-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="553b7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="553b7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="553b7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="553b7-134">Request</span></span>

<span data-ttu-id="553b7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="553b7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="553b7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="553b7-136">Response</span></span>

<span data-ttu-id="553b7-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="553b7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="553b7-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="553b7-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="553b7-141">C#</span><span class="sxs-lookup"><span data-stu-id="553b7-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="553b7-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="553b7-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
