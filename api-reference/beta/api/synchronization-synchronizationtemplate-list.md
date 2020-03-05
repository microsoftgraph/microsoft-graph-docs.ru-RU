---
title: Список существующих шаблонов синхронизации
description: Список шаблонов синхронизации, связанных с конкретным приложением или участником службы.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fa6cff80d76b12092801d9deea3d5c2d209c21d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452920"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="72e69-103">Список существующих шаблонов синхронизации</span><span class="sxs-lookup"><span data-stu-id="72e69-103">List existing synchronization templates</span></span>

<span data-ttu-id="72e69-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72e69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72e69-105">Список шаблонов синхронизации, связанных с конкретным приложением или участником службы.</span><span class="sxs-lookup"><span data-stu-id="72e69-105">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="72e69-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72e69-106">Permissions</span></span>
<span data-ttu-id="72e69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72e69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72e69-109">Permission type</span></span>                        | <span data-ttu-id="72e69-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72e69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="72e69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72e69-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="72e69-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72e69-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="72e69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72e69-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="72e69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72e69-114">Not supported.</span></span>|
|<span data-ttu-id="72e69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72e69-115">Application</span></span>                            |<span data-ttu-id="72e69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72e69-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="72e69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72e69-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="72e69-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72e69-118">Request headers</span></span>

| <span data-ttu-id="72e69-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72e69-119">Name</span></span>           | <span data-ttu-id="72e69-120">Тип</span><span class="sxs-lookup"><span data-stu-id="72e69-120">Type</span></span>    | <span data-ttu-id="72e69-121">Описание</span><span class="sxs-lookup"><span data-stu-id="72e69-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="72e69-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72e69-122">Authorization</span></span>  | <span data-ttu-id="72e69-123">string</span><span class="sxs-lookup"><span data-stu-id="72e69-123">string</span></span>  | <span data-ttu-id="72e69-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72e69-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72e69-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72e69-126">Request body</span></span>

<span data-ttu-id="72e69-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72e69-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="72e69-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="72e69-128">Response</span></span>

<span data-ttu-id="72e69-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и Аколлектион объектов [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="72e69-129">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="72e69-130">Пример</span><span class="sxs-lookup"><span data-stu-id="72e69-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="72e69-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="72e69-131">Request</span></span>
<span data-ttu-id="72e69-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72e69-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72e69-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="72e69-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="c"></a>[<span data-ttu-id="72e69-134">C#</span><span class="sxs-lookup"><span data-stu-id="72e69-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72e69-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72e69-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72e69-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72e69-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72e69-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="72e69-137">Response</span></span>
<span data-ttu-id="72e69-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72e69-138">The following is an example of a response.</span></span>
><span data-ttu-id="72e69-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72e69-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72e69-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72e69-140">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
