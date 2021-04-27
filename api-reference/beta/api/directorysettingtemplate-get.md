---
title: Получить шаблон настройки каталога
description: Позволяет получить свойства объекта directorySettingTemplate, включая доступные параметры и их значения по умолчанию.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 55b3d9d2f5a4bc141a6d8af177d30aa882a8e090
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046561"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="d2333-103">Получить шаблон настройки каталога</span><span class="sxs-lookup"><span data-stu-id="d2333-103">Get a directory setting template</span></span>

<span data-ttu-id="d2333-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2333-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2333-105">Шаблон настройки каталога представляет шаблон параметров, из которых можно создать параметры в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d2333-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="d2333-106">Эта операция позволяет получить свойства объекта **directorySettingTemplate,** включая доступные параметры и их по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d2333-106">This operation allows retrieval of the properties of the **directorySettingTemplate** object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="d2333-107">**Примечание.** Бета-версия этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="d2333-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d2333-108">Версия /v1.0 этого API переименована в *Get groupSettingTemplate.*</span><span class="sxs-lookup"><span data-stu-id="d2333-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2333-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2333-109">Permissions</span></span>
<span data-ttu-id="d2333-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2333-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2333-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2333-112">Permission type</span></span>      | <span data-ttu-id="d2333-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2333-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2333-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2333-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d2333-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2333-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d2333-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2333-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2333-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2333-117">Not supported.</span></span>    |
|<span data-ttu-id="d2333-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2333-118">Application</span></span> | <span data-ttu-id="d2333-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2333-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2333-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2333-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2333-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2333-121">Optional query parameters</span></span>
<span data-ttu-id="d2333-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d2333-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2333-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2333-123">Request headers</span></span>
| <span data-ttu-id="d2333-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d2333-124">Name</span></span>      |<span data-ttu-id="d2333-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d2333-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2333-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2333-126">Authorization</span></span>  | <span data-ttu-id="d2333-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2333-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2333-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2333-129">Request body</span></span>
<span data-ttu-id="d2333-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2333-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2333-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2333-131">Response</span></span>

<span data-ttu-id="d2333-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект directorySettingTemplate](../resources/directorysettingtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2333-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2333-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d2333-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2333-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2333-134">Request</span></span>
<span data-ttu-id="d2333-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2333-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2333-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2333-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="d2333-137">C#</span><span class="sxs-lookup"><span data-stu-id="d2333-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2333-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2333-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2333-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2333-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2333-140">Java</span><span class="sxs-lookup"><span data-stu-id="d2333-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysettingtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2333-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2333-141">Response</span></span>
<span data-ttu-id="d2333-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2333-142">Here is an example of the response.</span></span> <span data-ttu-id="d2333-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d2333-143">Note: The response object shown here might be shortened for readability.</span></span>
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


