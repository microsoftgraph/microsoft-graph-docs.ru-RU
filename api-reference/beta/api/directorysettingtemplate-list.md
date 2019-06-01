---
title: Список Директорисеттингтемплатес
description: Шаблоны параметров каталога представляют собой набор шаблонов параметров каталогов, из которых можно создавать и использовать параметры каталогов в клиенте.  Эта операция извлекает список доступных объектов Директорисеттингтемплатес.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: adfb303e24b637af4b77ac9f3cfd357ca09ece8f
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655784"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="a3bd7-104">Список Директорисеттингтемплатес</span><span class="sxs-lookup"><span data-stu-id="a3bd7-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3bd7-105">Шаблоны параметров каталога представляют собой набор шаблонов параметров каталогов, из которых можно создавать и использовать параметры каталогов в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="a3bd7-106">Эта операция извлекает список доступных объектов Директорисеттингтемплатес.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="a3bd7-107">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="a3bd7-108">Версия/v1.0 этого API была переименована в *List groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3bd7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3bd7-109">Permissions</span></span>
<span data-ttu-id="a3bd7-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3bd7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3bd7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3bd7-112">Permission type</span></span>      | <span data-ttu-id="a3bd7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3bd7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3bd7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3bd7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a3bd7-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3bd7-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3bd7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3bd7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3bd7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-117">Not supported.</span></span>    |
|<span data-ttu-id="a3bd7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3bd7-118">Application</span></span> | <span data-ttu-id="a3bd7-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3bd7-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3bd7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3bd7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a3bd7-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3bd7-121">Optional query parameters</span></span>
<span data-ttu-id="a3bd7-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3bd7-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3bd7-123">Request headers</span></span>
| <span data-ttu-id="a3bd7-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a3bd7-124">Name</span></span>      |<span data-ttu-id="a3bd7-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a3bd7-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3bd7-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3bd7-126">Authorization</span></span>  | <span data-ttu-id="a3bd7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3bd7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3bd7-129">Request body</span></span>
<span data-ttu-id="a3bd7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3bd7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3bd7-131">Response</span></span>

<span data-ttu-id="a3bd7-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [директорисеттингтемплате](../resources/directorysettingtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a3bd7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a3bd7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3bd7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3bd7-134">Request</span></span>
<span data-ttu-id="a3bd7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="a3bd7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3bd7-136">Response</span></span>
<span data-ttu-id="a3bd7-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3bd7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a3bd7-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a3bd7-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a3bd7-141">C#</span><span class="sxs-lookup"><span data-stu-id="a3bd7-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplates-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3bd7-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3bd7-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplates-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
