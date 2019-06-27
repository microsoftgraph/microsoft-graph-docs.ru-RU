---
title: Получение шаблона параметров каталога
description: Шаблон параметров каталога представляет шаблон параметров, параметры которых могут создаваться в клиенте. Эта операция позволяет получать свойства объекта Директорисеттингтемплате, включая доступные параметры и их значения по умолчанию.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8ee8a2562f19d988b13c1b2f6cf1027876ac9bf5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260524"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="4c6b1-104">Получение шаблона параметров каталога</span><span class="sxs-lookup"><span data-stu-id="4c6b1-104">Get a directory setting template</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c6b1-105">Шаблон параметров каталога представляет шаблон параметров, параметры которых могут создаваться в клиенте.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="4c6b1-106">Эта операция позволяет получать свойства объекта Директорисеттингтемплате, включая доступные параметры и их значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-106">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="4c6b1-107">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="4c6b1-108">Версия/v1.0 этого API была переименована, чтобы *получить groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c6b1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c6b1-109">Permissions</span></span>
<span data-ttu-id="4c6b1-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c6b1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c6b1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c6b1-112">Permission type</span></span>      | <span data-ttu-id="4c6b1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c6b1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c6b1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c6b1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4c6b1-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c6b1-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c6b1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c6b1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c6b1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-117">Not supported.</span></span>    |
|<span data-ttu-id="4c6b1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c6b1-118">Application</span></span> | <span data-ttu-id="4c6b1-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c6b1-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c6b1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c6b1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c6b1-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c6b1-121">Optional query parameters</span></span>
<span data-ttu-id="4c6b1-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c6b1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c6b1-123">Request headers</span></span>
| <span data-ttu-id="4c6b1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4c6b1-124">Name</span></span>      |<span data-ttu-id="4c6b1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4c6b1-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c6b1-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c6b1-126">Authorization</span></span>  | <span data-ttu-id="4c6b1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c6b1-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c6b1-129">Request body</span></span>
<span data-ttu-id="4c6b1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c6b1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c6b1-131">Response</span></span>

<span data-ttu-id="4c6b1-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [директорисеттингтемплате](../resources/directorysettingtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c6b1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4c6b1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c6b1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c6b1-134">Request</span></span>
<span data-ttu-id="4c6b1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="4c6b1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c6b1-136">Response</span></span>
<span data-ttu-id="4c6b1-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c6b1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 270

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
  ],
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4c6b1-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4c6b1-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4c6b1-141">C#</span><span class="sxs-lookup"><span data-stu-id="4c6b1-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c6b1-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c6b1-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4c6b1-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4c6b1-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
