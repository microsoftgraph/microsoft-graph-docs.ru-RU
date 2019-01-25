---
title: Доверия транзитивных групп списка устройств
description: Получите, устройство является членом группы. Этот запрос API доверия транзитивных и также возвращает все группы, устройство является участником вложенных.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 69cd4e4be3f02d3609bc9f0af2f094533c67dba7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528167"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="f2851-104">Доверия транзитивных групп списка устройств</span><span class="sxs-lookup"><span data-stu-id="f2851-104">List device transitive groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2851-105">Получите, устройство является членом группы.</span><span class="sxs-lookup"><span data-stu-id="f2851-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="f2851-106">Этот запрос API доверия транзитивных и также возвращает все группы, устройство является участником вложенных.</span><span class="sxs-lookup"><span data-stu-id="f2851-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2851-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2851-107">Permissions</span></span>

<span data-ttu-id="f2851-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2851-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2851-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2851-110">Permission type</span></span>      | <span data-ttu-id="f2851-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2851-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2851-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2851-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2851-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2851-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2851-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2851-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2851-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2851-115">Not supported.</span></span>    |
|<span data-ttu-id="f2851-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2851-116">Application</span></span> | <span data-ttu-id="f2851-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2851-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2851-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2851-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2851-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2851-119">Optional query parameters</span></span>

<span data-ttu-id="f2851-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2851-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2851-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2851-121">Request headers</span></span>

| <span data-ttu-id="f2851-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2851-122">Header</span></span>       | <span data-ttu-id="f2851-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f2851-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2851-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2851-124">Authorization</span></span>  | <span data-ttu-id="f2851-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2851-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f2851-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f2851-127">Accept</span></span>  | <span data-ttu-id="f2851-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f2851-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2851-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2851-129">Request body</span></span>

<span data-ttu-id="f2851-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2851-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2851-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2851-131">Response</span></span>

<span data-ttu-id="f2851-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2851-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2851-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f2851-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2851-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2851-134">Request</span></span>

<span data-ttu-id="f2851-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2851-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="f2851-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2851-136">Response</span></span>

<span data-ttu-id="f2851-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f2851-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
