---
title: Получение шаблона параметров каталога
description: Шаблон параметров каталога представляет шаблон параметров, параметры которых могут создаваться в клиенте. Эта операция позволяет получать свойства объекта Директорисеттингтемплате, включая доступные параметры и их значения по умолчанию.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d706c08e8c94eceb8a1eaa1d5615766aaa9ae3af
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436748"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="6a198-104">Получение шаблона параметров каталога</span><span class="sxs-lookup"><span data-stu-id="6a198-104">Get a directory setting template</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a198-105">Шаблон параметров каталога представляет шаблон параметров, параметры которых могут создаваться в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6a198-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="6a198-106">Эта операция позволяет получать свойства объекта Директорисеттингтемплате, включая доступные параметры и их значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6a198-106">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="6a198-107">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="6a198-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="6a198-108">Версия/v1.0 этого API была переименована, чтобы *получить groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="6a198-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a198-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a198-109">Permissions</span></span>
<span data-ttu-id="6a198-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a198-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a198-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a198-112">Permission type</span></span>      | <span data-ttu-id="6a198-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a198-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a198-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a198-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6a198-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a198-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a198-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a198-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a198-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a198-117">Not supported.</span></span>    |
|<span data-ttu-id="6a198-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a198-118">Application</span></span> | <span data-ttu-id="6a198-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a198-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a198-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a198-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a198-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a198-121">Optional query parameters</span></span>
<span data-ttu-id="6a198-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6a198-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a198-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a198-123">Request headers</span></span>
| <span data-ttu-id="6a198-124">Имя</span><span class="sxs-lookup"><span data-stu-id="6a198-124">Name</span></span>      |<span data-ttu-id="6a198-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6a198-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a198-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a198-126">Authorization</span></span>  | <span data-ttu-id="6a198-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a198-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a198-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6a198-129">Request body</span></span>
<span data-ttu-id="6a198-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a198-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a198-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a198-131">Response</span></span>

<span data-ttu-id="6a198-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [директорисеттингтемплате](../resources/directorysettingtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a198-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a198-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6a198-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a198-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a198-134">Request</span></span>
<span data-ttu-id="6a198-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a198-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a198-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a198-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a198-137">C#</span><span class="sxs-lookup"><span data-stu-id="6a198-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a198-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a198-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a198-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6a198-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6a198-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a198-140">Response</span></span>
<span data-ttu-id="6a198-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a198-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
