---
title: Получение Информатионпротектионлабел
description: Получение свойств и связей указанного объекта Информатионпротектионлабел.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2e4f2025d899cd5f6686eb6a3800d15ac8bf8526
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995661"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="8bf36-103">Получение Информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="8bf36-103">Get informationProtectionLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bf36-104">Получение свойств и связей объекта [информатионпротектионлабел](../resources/informationprotectionlabel.md) .</span><span class="sxs-lookup"><span data-stu-id="8bf36-104">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bf36-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bf36-105">Permissions</span></span>

<span data-ttu-id="8bf36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bf36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bf36-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bf36-108">Permission type</span></span>                        | <span data-ttu-id="8bf36-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bf36-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8bf36-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bf36-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bf36-111">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="8bf36-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="8bf36-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bf36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bf36-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bf36-113">Not supported.</span></span>                              |
| <span data-ttu-id="8bf36-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bf36-114">Application</span></span>                            | <span data-ttu-id="8bf36-115">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8bf36-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="8bf36-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bf36-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationprotection/policy/labels/{id}
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8bf36-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8bf36-117">Optional query parameters</span></span>

<span data-ttu-id="8bf36-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8bf36-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8bf36-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8bf36-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bf36-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bf36-120">Request headers</span></span>

| <span data-ttu-id="8bf36-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8bf36-121">Name</span></span>          | <span data-ttu-id="8bf36-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8bf36-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="8bf36-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bf36-123">Authorization</span></span> | <span data-ttu-id="8bf36-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bf36-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="8bf36-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bf36-126">Request body</span></span>

<span data-ttu-id="8bf36-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8bf36-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bf36-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8bf36-128">Response</span></span>

<span data-ttu-id="8bf36-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [информатионпротектионлабел](../resources/informationprotectionlabel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8bf36-129">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8bf36-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="8bf36-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8bf36-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bf36-131">Request</span></span>

<span data-ttu-id="8bf36-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bf36-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8bf36-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bf36-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8bf36-134">C#</span><span class="sxs-lookup"><span data-stu-id="8bf36-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-informationprotectionlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bf36-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bf36-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-informationprotectionlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bf36-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bf36-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-informationprotectionlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8bf36-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bf36-137">Response</span></span>

<span data-ttu-id="8bf36-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8bf36-138">The following is an example of the response.</span></span>

> <span data-ttu-id="8bf36-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bf36-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels/$entity",
    "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
    "name": "LabelWithFooterAndHeaderActions_Tests",
    "description": "",
    "color": "",
    "sensitivity": 12,
    "tooltip": "LabelWithFooterAndHeaderActions_Tests",
    "isActive": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get informationProtectionLabel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
