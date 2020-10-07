---
title: Получение параметра каталога
description: Получение свойств определенного объекта параметров каталога.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5aa600ddd17009916a9926e3ece103591f9ab152
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48371335"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="2c9b1-103">Получение параметра каталога</span><span class="sxs-lookup"><span data-stu-id="2c9b1-103">Get a directory setting</span></span>

<span data-ttu-id="2c9b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c9b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c9b1-105">Получение свойств определенного объекта параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-105">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="2c9b1-106">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="2c9b1-107">Версия/v1.0 этого API была переименована, чтобы *получить граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-107">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c9b1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c9b1-108">Permissions</span></span>
<span data-ttu-id="2c9b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c9b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c9b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c9b1-111">Permission type</span></span>      | <span data-ttu-id="2c9b1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c9b1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c9b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c9b1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2c9b1-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c9b1-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c9b1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c9b1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c9b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-116">Not supported.</span></span>    |
|<span data-ttu-id="2c9b1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c9b1-117">Application</span></span> | <span data-ttu-id="2c9b1-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c9b1-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c9b1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c9b1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="2c9b1-120">Получение определенного параметра на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="2c9b1-120">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2c9b1-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2c9b1-121">Optional query parameters</span></span>
<span data-ttu-id="2c9b1-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c9b1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c9b1-123">Request headers</span></span>
| <span data-ttu-id="2c9b1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="2c9b1-124">Name</span></span>      |<span data-ttu-id="2c9b1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2c9b1-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c9b1-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c9b1-126">Authorization</span></span>  | <span data-ttu-id="2c9b1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c9b1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c9b1-129">Request body</span></span>
<span data-ttu-id="2c9b1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c9b1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c9b1-131">Response</span></span>

<span data-ttu-id="2c9b1-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-132">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2c9b1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2c9b1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c9b1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c9b1-134">Request</span></span>
<span data-ttu-id="2c9b1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c9b1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c9b1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="2c9b1-137">C#</span><span class="sxs-lookup"><span data-stu-id="2c9b1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c9b1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c9b1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c9b1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c9b1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2c9b1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c9b1-140">Response</span></span>
<span data-ttu-id="2c9b1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c9b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
