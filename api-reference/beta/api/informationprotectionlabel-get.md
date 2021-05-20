---
title: Получить informationProtectionLabel
description: Извлечение свойств и связей указанного объекта informationProtectionLabel.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 02b1d36a2b4639487b9dd88dcf67c9592bce1aa9
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579622"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="33ef3-103">Получить informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="33ef3-103">Get informationProtectionLabel</span></span>

<span data-ttu-id="33ef3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33ef3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33ef3-105">Извлечение свойств и связей объекта [informationProtectionLabel.](../resources/informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="33ef3-105">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="33ef3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33ef3-106">Permissions</span></span>

<span data-ttu-id="33ef3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33ef3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33ef3-109">Permission type</span></span>                        | <span data-ttu-id="33ef3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33ef3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="33ef3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33ef3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="33ef3-112">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="33ef3-112">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="33ef3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33ef3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33ef3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33ef3-114">Not supported.</span></span>                              |
| <span data-ttu-id="33ef3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33ef3-115">Application</span></span>                            | <span data-ttu-id="33ef3-116">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="33ef3-116">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="33ef3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33ef3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
<span data-ttu-id="33ef3-118">Чтобы получить метку, доступную для подписанного пользователя или указанного пользователя:</span><span class="sxs-lookup"><span data-stu-id="33ef3-118">To get a label available to the signed-in user or specified user:</span></span>
```http
GET /me/informationProtection/policy/labels/{id}
GET /users/{id | user-principal-name}/informationProtection/policy/labels/{id}
```

<span data-ttu-id="33ef3-119">Чтобы получить метку, доступную организации:</span><span class="sxs-lookup"><span data-stu-id="33ef3-119">To get a label available to the organization:</span></span>
```http
GET /informationProtection/policy/labels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33ef3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="33ef3-120">Optional query parameters</span></span>

<span data-ttu-id="33ef3-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="33ef3-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="33ef3-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="33ef3-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="33ef3-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33ef3-123">Request headers</span></span>

| <span data-ttu-id="33ef3-124">Имя</span><span class="sxs-lookup"><span data-stu-id="33ef3-124">Name</span></span>          | <span data-ttu-id="33ef3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="33ef3-125">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="33ef3-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33ef3-126">Authorization</span></span> | <span data-ttu-id="33ef3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33ef3-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="33ef3-129">User-Agent</span><span class="sxs-lookup"><span data-stu-id="33ef3-129">User-Agent</span></span>    | <span data-ttu-id="33ef3-130">Описывает имя и версию вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="33ef3-130">Describes the name and version of the calling application.</span></span> <span data-ttu-id="33ef3-131">Сведения будут всплыть в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="33ef3-131">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="33ef3-132">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="33ef3-132">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="33ef3-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="33ef3-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33ef3-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33ef3-134">Request body</span></span>

<span data-ttu-id="33ef3-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33ef3-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33ef3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="33ef3-136">Response</span></span>

<span data-ttu-id="33ef3-137">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [informationProtectionLabel](../resources/informationprotectionlabel.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="33ef3-137">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33ef3-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="33ef3-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="33ef3-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="33ef3-139">Request</span></span>

<span data-ttu-id="33ef3-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33ef3-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33ef3-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="33ef3-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```
# <a name="c"></a>[<span data-ttu-id="33ef3-142">C#</span><span class="sxs-lookup"><span data-stu-id="33ef3-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-informationprotectionlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33ef3-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33ef3-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-informationprotectionlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33ef3-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33ef3-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-informationprotectionlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33ef3-145">Java</span><span class="sxs-lookup"><span data-stu-id="33ef3-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-informationprotectionlabel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="33ef3-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="33ef3-146">Response</span></span>

<span data-ttu-id="33ef3-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="33ef3-147">The following is an example of the response.</span></span>

> <span data-ttu-id="33ef3-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="33ef3-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "id": "4b18e8bb-b4a5-4695-85d0-8ae23ef27892",
  "name": "Highly Confidential",
  "description": "Consult Contoso data labeling policy for more details.",
  "color": "",
  "sensitivity": 3,
  "tooltip": "Data classified as Contoso Highly Confidential.",
  "isActive": true,
  "parent": null
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


