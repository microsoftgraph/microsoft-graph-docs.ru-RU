---
title: Список существующих шаблонов синхронизации
description: Список шаблонов синхронизации, связанных с заданным приложением или директором службы.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 323a870c94ea465ce0cbfa84903090ee944a5ee7
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625943"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="8a635-103">Список существующих шаблонов синхронизации</span><span class="sxs-lookup"><span data-stu-id="8a635-103">List existing synchronization templates</span></span>

<span data-ttu-id="8a635-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a635-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a635-105">Список шаблонов синхронизации, связанных с заданным приложением или директором службы.</span><span class="sxs-lookup"><span data-stu-id="8a635-105">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a635-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a635-106">Permissions</span></span>
<span data-ttu-id="8a635-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a635-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a635-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a635-109">Permission type</span></span>                        | <span data-ttu-id="8a635-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a635-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a635-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a635-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="8a635-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a635-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="8a635-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a635-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8a635-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a635-114">Not supported.</span></span>|
|<span data-ttu-id="8a635-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8a635-115">Application</span></span>                            |<span data-ttu-id="8a635-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a635-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

### <a name="http-request"></a><span data-ttu-id="8a635-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a635-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="8a635-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8a635-118">Request headers</span></span>

| <span data-ttu-id="8a635-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8a635-119">Name</span></span>           | <span data-ttu-id="8a635-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8a635-120">Type</span></span>    | <span data-ttu-id="8a635-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8a635-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8a635-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a635-122">Authorization</span></span>  | <span data-ttu-id="8a635-123">string</span><span class="sxs-lookup"><span data-stu-id="8a635-123">string</span></span>  | <span data-ttu-id="8a635-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a635-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a635-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a635-126">Request body</span></span>

<span data-ttu-id="8a635-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a635-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="8a635-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a635-128">Response</span></span>

<span data-ttu-id="8a635-129">В случае успешной работы этот метод возвращает код отклика и аколлекцию объектов `200 OK` [синхронизацииTemplate](../resources/synchronization-synchronizationtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8a635-129">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="8a635-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8a635-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8a635-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a635-131">Request</span></span>
<span data-ttu-id="8a635-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a635-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a635-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a635-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="c"></a>[<span data-ttu-id="8a635-134">C#</span><span class="sxs-lookup"><span data-stu-id="8a635-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a635-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a635-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a635-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a635-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a635-137">Java</span><span class="sxs-lookup"><span data-stu-id="8a635-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8a635-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a635-138">Response</span></span>
<span data-ttu-id="8a635-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a635-139">The following is an example of a response.</span></span>
><span data-ttu-id="8a635-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8a635-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8a635-141">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8a635-141">All the properties will be returned in an actual call.</span></span>
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


