---
title: Получение параметра каталога
description: Получение свойств определенного объекта параметров каталога.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 839a21f1afaa2667f40e4328a066f82e5d3b025c
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312830"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="65b4c-103">Получение параметра каталога</span><span class="sxs-lookup"><span data-stu-id="65b4c-103">Get a directory setting</span></span>

<span data-ttu-id="65b4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65b4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65b4c-105">Получение свойств определенного объекта параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="65b4c-105">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="65b4c-106">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="65b4c-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="65b4c-107">Версия/v1.0 этого API была переименована, чтобы *получить граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="65b4c-107">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="65b4c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65b4c-108">Permissions</span></span>
<span data-ttu-id="65b4c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65b4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65b4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65b4c-111">Permission type</span></span>      | <span data-ttu-id="65b4c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65b4c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65b4c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65b4c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="65b4c-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65b4c-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65b4c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65b4c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65b4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65b4c-116">Not supported.</span></span>    |
|<span data-ttu-id="65b4c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65b4c-117">Application</span></span> | <span data-ttu-id="65b4c-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b4c-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65b4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65b4c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="65b4c-120">Получение определенного параметра на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="65b4c-120">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65b4c-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="65b4c-121">Optional query parameters</span></span>
<span data-ttu-id="65b4c-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="65b4c-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65b4c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65b4c-123">Request headers</span></span>
| <span data-ttu-id="65b4c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="65b4c-124">Name</span></span>      |<span data-ttu-id="65b4c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="65b4c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="65b4c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65b4c-126">Authorization</span></span>  | <span data-ttu-id="65b4c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65b4c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65b4c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65b4c-129">Request body</span></span>
<span data-ttu-id="65b4c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65b4c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65b4c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="65b4c-131">Response</span></span>

<span data-ttu-id="65b4c-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65b4c-132">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65b4c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="65b4c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65b4c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="65b4c-134">Request</span></span>
<span data-ttu-id="65b4c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65b4c-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65b4c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="65b4c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="65b4c-137">C#</span><span class="sxs-lookup"><span data-stu-id="65b4c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65b4c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65b4c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65b4c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65b4c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="65b4c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="65b4c-140">Response</span></span>
<span data-ttu-id="65b4c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65b4c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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