---
title: Получение параметра каталога
description: Получение свойств определенного объекта параметров каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48195a099b7fb8c0cc84f4f7dd9455cf18247d4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957586"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="3cf62-103">Получение параметра каталога</span><span class="sxs-lookup"><span data-stu-id="3cf62-103">Get a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cf62-104">Получение свойств определенного объекта параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="3cf62-104">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="3cf62-105">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="3cf62-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="3cf62-106">Версия/v1.0 этого API была переименована, чтобы *получить граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="3cf62-106">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cf62-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cf62-107">Permissions</span></span>
<span data-ttu-id="3cf62-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cf62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cf62-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cf62-110">Permission type</span></span>      | <span data-ttu-id="3cf62-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cf62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cf62-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cf62-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3cf62-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3cf62-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3cf62-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cf62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cf62-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cf62-115">Not supported.</span></span>    |
|<span data-ttu-id="3cf62-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cf62-116">Application</span></span> | <span data-ttu-id="3cf62-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cf62-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cf62-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cf62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="3cf62-119">Получение определенного параметра на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="3cf62-119">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3cf62-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3cf62-120">Optional query parameters</span></span>
<span data-ttu-id="3cf62-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3cf62-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cf62-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cf62-122">Request headers</span></span>
| <span data-ttu-id="3cf62-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3cf62-123">Name</span></span>      |<span data-ttu-id="3cf62-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3cf62-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3cf62-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cf62-125">Authorization</span></span>  | <span data-ttu-id="3cf62-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cf62-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cf62-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3cf62-128">Request body</span></span>
<span data-ttu-id="3cf62-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3cf62-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cf62-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cf62-130">Response</span></span>

<span data-ttu-id="3cf62-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3cf62-131">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3cf62-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3cf62-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cf62-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cf62-133">Request</span></span>
<span data-ttu-id="3cf62-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cf62-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3cf62-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cf62-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3cf62-136">C#</span><span class="sxs-lookup"><span data-stu-id="3cf62-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cf62-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cf62-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3cf62-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3cf62-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3cf62-139">Java</span><span class="sxs-lookup"><span data-stu-id="3cf62-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3cf62-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cf62-140">Response</span></span>
<span data-ttu-id="3cf62-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3cf62-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 198

{
  "id": "id-value",
  "displayName": "displayName-value",
  "settingTemplateId": "settingTemplateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
