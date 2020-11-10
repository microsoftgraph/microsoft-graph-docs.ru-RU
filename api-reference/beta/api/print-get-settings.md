---
title: Получение Принтсеттингс
description: Получение параметров на уровне клиента для универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6d7cf853a9204907a0dfae7c62b35a1c68d886ac
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967104"
---
# <a name="get-printsettings"></a><span data-ttu-id="0b8cd-103">Получение Принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="0b8cd-103">Get printSettings</span></span>

<span data-ttu-id="0b8cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b8cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b8cd-105">Получение параметров на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b8cd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b8cd-106">Permissions</span></span>
<span data-ttu-id="0b8cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b8cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0b8cd-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="0b8cd-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="0b8cd-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="0b8cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b8cd-111">Permission type</span></span> | <span data-ttu-id="0b8cd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b8cd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0b8cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b8cd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="0b8cd-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="0b8cd-114">User.Read</span></span> |
|<span data-ttu-id="0b8cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b8cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b8cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-116">Not Supported.</span></span>|
|<span data-ttu-id="0b8cd-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0b8cd-117">Application</span></span>|<span data-ttu-id="0b8cd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b8cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b8cd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b8cd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b8cd-120">Optional query parameters</span></span>
<span data-ttu-id="0b8cd-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0b8cd-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0b8cd-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b8cd-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b8cd-123">Request headers</span></span>
| <span data-ttu-id="0b8cd-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0b8cd-124">Name</span></span>      |<span data-ttu-id="0b8cd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0b8cd-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b8cd-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b8cd-126">Authorization</span></span> | <span data-ttu-id="0b8cd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b8cd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b8cd-129">Request body</span></span>
<span data-ttu-id="0b8cd-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0b8cd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b8cd-131">Response</span></span>
<span data-ttu-id="0b8cd-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтсеттингс](../resources/printsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-132">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b8cd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0b8cd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b8cd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b8cd-134">Request</span></span>
<span data-ttu-id="0b8cd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b8cd-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b8cd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/settings
```
# <a name="c"></a>[<span data-ttu-id="0b8cd-137">C#</span><span class="sxs-lookup"><span data-stu-id="0b8cd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b8cd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b8cd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b8cd-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b8cd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b8cd-140">Java</span><span class="sxs-lookup"><span data-stu-id="0b8cd-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b8cd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b8cd-141">Response</span></span>
<span data-ttu-id="0b8cd-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-142">The following is an example of the response.</span></span>
><span data-ttu-id="0b8cd-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b8cd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
