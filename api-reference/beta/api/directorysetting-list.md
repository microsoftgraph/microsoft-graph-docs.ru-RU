---
title: Параметры каталога списка
description: Получение списка объектов параметров каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c183aacfc557a682cc965963b6a48d4a6eb9b71d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718170"
---
# <a name="list-directory-settings"></a><span data-ttu-id="3c3e1-103">Параметры каталога списка</span><span class="sxs-lookup"><span data-stu-id="3c3e1-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c3e1-104">Получение списка объектов параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="3c3e1-105">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="3c3e1-106">Версия/v1.0 этого API была переименована в *List граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c3e1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c3e1-107">Permissions</span></span>
<span data-ttu-id="3c3e1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c3e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c3e1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c3e1-110">Permission type</span></span>      | <span data-ttu-id="3c3e1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c3e1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c3e1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c3e1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c3e1-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c3e1-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c3e1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c3e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c3e1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-115">Not supported.</span></span>    |
|<span data-ttu-id="3c3e1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c3e1-116">Application</span></span> | <span data-ttu-id="3c3e1-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c3e1-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c3e1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c3e1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="3c3e1-119">Перечисление параметров на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="3c3e1-119">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c3e1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c3e1-120">Optional query parameters</span></span>
<span data-ttu-id="3c3e1-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c3e1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c3e1-122">Request headers</span></span>
| <span data-ttu-id="3c3e1-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3c3e1-123">Name</span></span>      |<span data-ttu-id="3c3e1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3c3e1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3c3e1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c3e1-125">Authorization</span></span>  | <span data-ttu-id="3c3e1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c3e1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c3e1-128">Request body</span></span>
<span data-ttu-id="3c3e1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c3e1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c3e1-130">Response</span></span>

<span data-ttu-id="3c3e1-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c3e1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3c3e1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c3e1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c3e1-133">Request</span></span>
<span data-ttu-id="3c3e1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3c3e1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c3e1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c3e1-136">C#</span><span class="sxs-lookup"><span data-stu-id="3c3e1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c3e1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c3e1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c3e1-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3c3e1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c3e1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c3e1-139">Response</span></span>
<span data-ttu-id="3c3e1-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c3e1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
