---
title: Получение Информатионпротектионлабел
description: Получение свойств и связей указанного объекта Информатионпротектионлабел.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9c4b923279004c91b3e9d4e185d87f9ee15457ed
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216682"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="57668-103">Получение Информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="57668-103">Get informationProtectionLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57668-104">Получение свойств и связей объекта [информатионпротектионлабел](../resources/informationprotectionlabel.md) .</span><span class="sxs-lookup"><span data-stu-id="57668-104">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57668-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57668-105">Permissions</span></span>

<span data-ttu-id="57668-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57668-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57668-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57668-108">Permission type</span></span>                        | <span data-ttu-id="57668-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57668-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="57668-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57668-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="57668-111">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="57668-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="57668-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57668-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57668-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57668-113">Not supported.</span></span>                              |
| <span data-ttu-id="57668-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="57668-114">Application</span></span>                            | <span data-ttu-id="57668-115">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="57668-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="57668-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57668-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationprotection/policy/labels/{id}
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57668-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57668-117">Optional query parameters</span></span>

<span data-ttu-id="57668-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="57668-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="57668-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="57668-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="57668-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57668-120">Request headers</span></span>

| <span data-ttu-id="57668-121">Имя</span><span class="sxs-lookup"><span data-stu-id="57668-121">Name</span></span>          | <span data-ttu-id="57668-122">Описание</span><span class="sxs-lookup"><span data-stu-id="57668-122">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="57668-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57668-123">Authorization</span></span> | <span data-ttu-id="57668-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57668-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="57668-126">User — Agent</span><span class="sxs-lookup"><span data-stu-id="57668-126">User-Agent</span></span>    | <span data-ttu-id="57668-127">Описывает имя и версию вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="57668-127">Describes the name and version of the calling application.</span></span> <span data-ttu-id="57668-128">Подробные сведения отображаются в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="57668-128">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="57668-129">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="57668-129">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="57668-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="57668-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57668-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57668-131">Request body</span></span>

<span data-ttu-id="57668-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57668-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57668-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="57668-133">Response</span></span>

<span data-ttu-id="57668-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [информатионпротектионлабел](../resources/informationprotectionlabel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57668-134">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57668-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="57668-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57668-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="57668-136">Request</span></span>

<span data-ttu-id="57668-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57668-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="57668-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="57668-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="57668-139">C#</span><span class="sxs-lookup"><span data-stu-id="57668-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-informationprotectionlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57668-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57668-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-informationprotectionlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="57668-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57668-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-informationprotectionlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57668-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="57668-142">Response</span></span>

<span data-ttu-id="57668-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57668-143">The following is an example of the response.</span></span>

> <span data-ttu-id="57668-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57668-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
User-agent: ContosoLOBApp/1.0

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
