---
title: Получение объекта directoryRole
description: Получение свойств объекта directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: f8ff306359675f7bc2c569f507dbcb3baf33b384
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832230"
---
# <a name="get-directoryrole"></a><span data-ttu-id="89902-103">Получение объекта directoryRole</span><span class="sxs-lookup"><span data-stu-id="89902-103">Get directoryRole</span></span>

<span data-ttu-id="89902-104">Получение свойств объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="89902-104">Retrieve the properties of a directoryRole object.</span></span>

## <a name="permissions"></a><span data-ttu-id="89902-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89902-105">Permissions</span></span>
<span data-ttu-id="89902-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89902-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89902-108">Permission type</span></span>      | <span data-ttu-id="89902-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89902-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89902-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89902-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89902-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="89902-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="89902-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89902-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89902-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89902-113">Not supported.</span></span>    |
|<span data-ttu-id="89902-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89902-114">Application</span></span> | <span data-ttu-id="89902-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89902-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89902-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89902-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89902-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89902-117">Optional query parameters</span></span>
<span data-ttu-id="89902-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="89902-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="89902-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89902-119">Request headers</span></span>
| <span data-ttu-id="89902-120">Имя</span><span class="sxs-lookup"><span data-stu-id="89902-120">Name</span></span>       | <span data-ttu-id="89902-121">Тип</span><span class="sxs-lookup"><span data-stu-id="89902-121">Type</span></span> | <span data-ttu-id="89902-122">Описание</span><span class="sxs-lookup"><span data-stu-id="89902-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="89902-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89902-123">Authorization</span></span>  | <span data-ttu-id="89902-124">string</span><span class="sxs-lookup"><span data-stu-id="89902-124">string</span></span>  | <span data-ttu-id="89902-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89902-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89902-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89902-127">Request body</span></span>
<span data-ttu-id="89902-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89902-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89902-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="89902-129">Response</span></span>

<span data-ttu-id="89902-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89902-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89902-131">Пример</span><span class="sxs-lookup"><span data-stu-id="89902-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89902-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="89902-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="89902-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="89902-133">Response</span></span>
<span data-ttu-id="89902-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89902-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
