---
title: Get printSettings
description: Извлекать параметры на всем клиенте для службы универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 47fae561c37a1315bf154a8998d8d5416895847e
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873040"
---
# <a name="get-printsettings"></a><span data-ttu-id="7d066-103">Get printSettings</span><span class="sxs-lookup"><span data-stu-id="7d066-103">Get printSettings</span></span>

<span data-ttu-id="7d066-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d066-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d066-105">Извлекать параметры на всем клиенте для службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="7d066-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d066-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d066-106">Permissions</span></span>
<span data-ttu-id="7d066-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7d066-109">Чтобы использовать службу универсальной печати, у пользователя или клиента приложения должна быть активная подписка универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7d066-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="7d066-110">Пользователь, выписав его, должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="7d066-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="7d066-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d066-111">Permission type</span></span> | <span data-ttu-id="7d066-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d066-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7d066-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d066-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7d066-114">PrintSettings.Read.All, PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d066-114">PrintSettings.Read.All, PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="7d066-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d066-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d066-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d066-116">Not Supported.</span></span>|
|<span data-ttu-id="7d066-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d066-117">Application</span></span>|<span data-ttu-id="7d066-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d066-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d066-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d066-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d066-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d066-120">Optional query parameters</span></span>
<span data-ttu-id="7d066-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7d066-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7d066-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7d066-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d066-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d066-123">Request headers</span></span>
| <span data-ttu-id="7d066-124">Имя</span><span class="sxs-lookup"><span data-stu-id="7d066-124">Name</span></span>      |<span data-ttu-id="7d066-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7d066-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d066-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d066-126">Authorization</span></span> | <span data-ttu-id="7d066-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d066-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d066-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d066-129">Request body</span></span>
<span data-ttu-id="7d066-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d066-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7d066-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d066-131">Response</span></span>
<span data-ttu-id="7d066-132">В случае успеха этот метод возвращает код отклика и объект `200 OK` [printSettings](../resources/printsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d066-132">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d066-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7d066-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d066-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d066-134">Request</span></span>
<span data-ttu-id="7d066-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d066-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d066-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d066-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/settings
```
# <a name="c"></a>[<span data-ttu-id="7d066-137">C#</span><span class="sxs-lookup"><span data-stu-id="7d066-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d066-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d066-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d066-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d066-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d066-140">Java</span><span class="sxs-lookup"><span data-stu-id="7d066-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7d066-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d066-141">Response</span></span>
<span data-ttu-id="7d066-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7d066-142">The following is an example of the response.</span></span>
><span data-ttu-id="7d066-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d066-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 144

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
