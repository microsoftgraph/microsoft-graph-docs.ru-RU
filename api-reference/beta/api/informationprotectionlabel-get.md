---
title: Получить informationProtectionLabel
description: Извлечение свойств и связей указанного объекта informationProtectionLabel.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: df3941dd135cf33fe28f281132be4856c65baac0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040338"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="ee20d-103">Получить informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="ee20d-103">Get informationProtectionLabel</span></span>

<span data-ttu-id="ee20d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee20d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee20d-105">Извлечение свойств и связей объекта [informationProtectionLabel.](../resources/informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="ee20d-105">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee20d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee20d-106">Permissions</span></span>

<span data-ttu-id="ee20d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee20d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee20d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee20d-109">Permission type</span></span>                        | <span data-ttu-id="ee20d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee20d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ee20d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee20d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee20d-112">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="ee20d-112">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="ee20d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee20d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee20d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee20d-114">Not supported.</span></span>                              |
| <span data-ttu-id="ee20d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee20d-115">Application</span></span>                            | <span data-ttu-id="ee20d-116">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee20d-116">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="ee20d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee20d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
<span data-ttu-id="ee20d-118">Чтобы получить метку, доступную для подписанного пользователя или указанного пользователя:</span><span class="sxs-lookup"><span data-stu-id="ee20d-118">To get a label available to the signed-in user or specified user:</span></span>
```http
GET /me/informationProtection/policy/labels/{id}
GET /users/{id | user-principal-name}/informationProtection/policy/labels/{id}
```

<span data-ttu-id="ee20d-119">Чтобы получить метку, доступную организации:</span><span class="sxs-lookup"><span data-stu-id="ee20d-119">To get a label available to the organization:</span></span>
```http
GET /informationProtection/policy/labels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee20d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee20d-120">Optional query parameters</span></span>

<span data-ttu-id="ee20d-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ee20d-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ee20d-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ee20d-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee20d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee20d-123">Request headers</span></span>

| <span data-ttu-id="ee20d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ee20d-124">Name</span></span>          | <span data-ttu-id="ee20d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ee20d-125">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ee20d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee20d-126">Authorization</span></span> | <span data-ttu-id="ee20d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee20d-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="ee20d-129">User-Agent</span><span class="sxs-lookup"><span data-stu-id="ee20d-129">User-Agent</span></span>    | <span data-ttu-id="ee20d-130">Описывает имя и версию вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="ee20d-130">Describes the name and version of the calling application.</span></span> <span data-ttu-id="ee20d-131">Сведения будут всплыть в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="ee20d-131">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="ee20d-132">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="ee20d-132">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="ee20d-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ee20d-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee20d-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee20d-134">Request body</span></span>

<span data-ttu-id="ee20d-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee20d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee20d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee20d-136">Response</span></span>

<span data-ttu-id="ee20d-137">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [informationProtectionLabel](../resources/informationprotectionlabel.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ee20d-137">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee20d-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="ee20d-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee20d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee20d-139">Request</span></span>

<span data-ttu-id="ee20d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee20d-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee20d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee20d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```
# <a name="c"></a>[<span data-ttu-id="ee20d-142">C#</span><span class="sxs-lookup"><span data-stu-id="ee20d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-informationprotectionlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee20d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee20d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-informationprotectionlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee20d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee20d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-informationprotectionlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee20d-145">Java</span><span class="sxs-lookup"><span data-stu-id="ee20d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-informationprotectionlabel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee20d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee20d-146">Response</span></span>

<span data-ttu-id="ee20d-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ee20d-147">The following is an example of the response.</span></span>

> <span data-ttu-id="ee20d-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ee20d-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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


