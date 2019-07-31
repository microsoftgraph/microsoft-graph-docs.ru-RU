---
title: Параметры каталога списка
description: Получение списка объектов параметров каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9475acfdbe802978a513481a47ccc2973ae89542
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957579"
---
# <a name="list-directory-settings"></a><span data-ttu-id="79200-103">Параметры каталога списка</span><span class="sxs-lookup"><span data-stu-id="79200-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79200-104">Получение списка объектов параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="79200-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="79200-105">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="79200-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="79200-106">Версия/v1.0 этого API была переименована в *List граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="79200-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="79200-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79200-107">Permissions</span></span>
<span data-ttu-id="79200-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79200-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79200-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79200-110">Permission type</span></span>      | <span data-ttu-id="79200-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79200-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79200-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79200-112">Delegated (work or school account)</span></span> | <span data-ttu-id="79200-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79200-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="79200-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79200-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79200-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79200-115">Not supported.</span></span>    |
|<span data-ttu-id="79200-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79200-116">Application</span></span> | <span data-ttu-id="79200-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79200-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79200-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79200-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="79200-119">Перечисление параметров на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="79200-119">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79200-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79200-120">Optional query parameters</span></span>
<span data-ttu-id="79200-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="79200-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79200-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79200-122">Request headers</span></span>
| <span data-ttu-id="79200-123">Имя</span><span class="sxs-lookup"><span data-stu-id="79200-123">Name</span></span>      |<span data-ttu-id="79200-124">Описание</span><span class="sxs-lookup"><span data-stu-id="79200-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79200-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79200-125">Authorization</span></span>  | <span data-ttu-id="79200-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79200-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79200-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79200-128">Request body</span></span>
<span data-ttu-id="79200-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79200-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79200-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="79200-130">Response</span></span>

<span data-ttu-id="79200-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79200-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79200-132">Пример</span><span class="sxs-lookup"><span data-stu-id="79200-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79200-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="79200-133">Request</span></span>
<span data-ttu-id="79200-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79200-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79200-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="79200-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79200-136">C#</span><span class="sxs-lookup"><span data-stu-id="79200-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79200-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="79200-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79200-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="79200-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79200-139">Java</span><span class="sxs-lookup"><span data-stu-id="79200-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="79200-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="79200-140">Response</span></span>
<span data-ttu-id="79200-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79200-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
