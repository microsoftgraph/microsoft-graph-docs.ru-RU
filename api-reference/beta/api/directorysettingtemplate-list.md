---
title: List directorySettingTemplates
description: Эта операция извлекает список доступных объектов directorySettingTemplates.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 06b62e868991f7da1012b23fbacc940665cd8350
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046547"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="780ba-103">List directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="780ba-103">List directorySettingTemplates</span></span>

<span data-ttu-id="780ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="780ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="780ba-105">Шаблоны параметров каталогов представляют собой набор шаблонов параметров каталогов, из которых можно создавать и использовать параметры каталога в клиенте.</span><span class="sxs-lookup"><span data-stu-id="780ba-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="780ba-106">Эта операция извлекает список доступных **объектов directorySettingTemplates.**</span><span class="sxs-lookup"><span data-stu-id="780ba-106">This operation retrieves the list of available **directorySettingTemplates** objects.</span></span>

> <span data-ttu-id="780ba-107">**Примечание.** Бета-версия этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="780ba-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="780ba-108">Версия /v1.0 этого API переименована в *list groupSettingTemplate.*</span><span class="sxs-lookup"><span data-stu-id="780ba-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="780ba-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="780ba-109">Permissions</span></span>
<span data-ttu-id="780ba-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="780ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="780ba-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="780ba-112">Permission type</span></span>      | <span data-ttu-id="780ba-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="780ba-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="780ba-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="780ba-114">Delegated (work or school account)</span></span> | <span data-ttu-id="780ba-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="780ba-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="780ba-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="780ba-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="780ba-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="780ba-117">Not supported.</span></span>    |
|<span data-ttu-id="780ba-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="780ba-118">Application</span></span> | <span data-ttu-id="780ba-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="780ba-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="780ba-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="780ba-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="780ba-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="780ba-121">Optional query parameters</span></span>
<span data-ttu-id="780ba-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="780ba-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="780ba-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="780ba-123">Request headers</span></span>
| <span data-ttu-id="780ba-124">Имя</span><span class="sxs-lookup"><span data-stu-id="780ba-124">Name</span></span>      |<span data-ttu-id="780ba-125">Описание</span><span class="sxs-lookup"><span data-stu-id="780ba-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="780ba-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="780ba-126">Authorization</span></span>  | <span data-ttu-id="780ba-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="780ba-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="780ba-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="780ba-129">Request body</span></span>
<span data-ttu-id="780ba-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="780ba-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="780ba-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="780ba-131">Response</span></span>

<span data-ttu-id="780ba-132">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов directorySettingTemplate](../resources/directorysettingtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="780ba-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="780ba-133">Пример</span><span class="sxs-lookup"><span data-stu-id="780ba-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="780ba-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="780ba-134">Request</span></span>
<span data-ttu-id="780ba-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="780ba-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="780ba-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="780ba-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="780ba-137">C#</span><span class="sxs-lookup"><span data-stu-id="780ba-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="780ba-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="780ba-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="780ba-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="780ba-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="780ba-140">Java</span><span class="sxs-lookup"><span data-stu-id="780ba-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="780ba-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="780ba-141">Response</span></span>
<span data-ttu-id="780ba-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="780ba-142">Here is an example of the response.</span></span> <span data-ttu-id="780ba-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="780ba-143">Note: The response object shown here might be shortened for readability.</span></span>
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


