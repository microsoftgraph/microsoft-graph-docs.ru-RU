---
title: Список Директорисеттингтемплатес
description: Шаблоны параметров каталога представляют собой набор шаблонов параметров каталогов, из которых можно создавать и использовать параметры каталогов в клиенте.  Эта операция извлекает список доступных объектов Директорисеттингтемплатес.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3ff5c102652d0c04bf37c3545b50fe320071be07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433834"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="ab28b-104">Список Директорисеттингтемплатес</span><span class="sxs-lookup"><span data-stu-id="ab28b-104">List directorySettingTemplates</span></span>

<span data-ttu-id="ab28b-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ab28b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab28b-106">Шаблоны параметров каталога представляют собой набор шаблонов параметров каталогов, из которых можно создавать и использовать параметры каталогов в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ab28b-106">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="ab28b-107">Эта операция извлекает список доступных объектов Директорисеттингтемплатес.</span><span class="sxs-lookup"><span data-stu-id="ab28b-107">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="ab28b-108">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="ab28b-108">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="ab28b-109">Версия/v1.0 этого API была переименована в *List groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="ab28b-109">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab28b-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab28b-110">Permissions</span></span>
<span data-ttu-id="ab28b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab28b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab28b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab28b-113">Permission type</span></span>      | <span data-ttu-id="ab28b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab28b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab28b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab28b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ab28b-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab28b-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab28b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab28b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab28b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab28b-118">Not supported.</span></span>    |
|<span data-ttu-id="ab28b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab28b-119">Application</span></span> | <span data-ttu-id="ab28b-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab28b-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab28b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab28b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab28b-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab28b-122">Optional query parameters</span></span>
<span data-ttu-id="ab28b-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ab28b-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab28b-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab28b-124">Request headers</span></span>
| <span data-ttu-id="ab28b-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ab28b-125">Name</span></span>      |<span data-ttu-id="ab28b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ab28b-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab28b-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab28b-127">Authorization</span></span>  | <span data-ttu-id="ab28b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab28b-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab28b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab28b-130">Request body</span></span>
<span data-ttu-id="ab28b-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab28b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab28b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab28b-132">Response</span></span>

<span data-ttu-id="ab28b-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [директорисеттингтемплате](../resources/directorysettingtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab28b-133">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab28b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ab28b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab28b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab28b-135">Request</span></span>
<span data-ttu-id="ab28b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab28b-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab28b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab28b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="ab28b-138">C#</span><span class="sxs-lookup"><span data-stu-id="ab28b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab28b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab28b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab28b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab28b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ab28b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab28b-141">Response</span></span>
<span data-ttu-id="ab28b-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab28b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 343

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "description": "description-value",
      "values": [
        {
          "name": "name-value",
          "type": "type-value",
          "defaultValue": "defaultValue-value",
          "description": "description-value"
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
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
