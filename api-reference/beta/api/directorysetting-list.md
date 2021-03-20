---
title: Параметры каталога списков
description: Извлечение списка объектов настройки каталогов.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 752b3cff056d2dd49bce3ac8bb9a03c7d37c9d94
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946553"
---
# <a name="list-directory-settings"></a><span data-ttu-id="f5fb0-103">Параметры каталога списков</span><span class="sxs-lookup"><span data-stu-id="f5fb0-103">List directory settings</span></span>

<span data-ttu-id="f5fb0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5fb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5fb0-105">Извлечение списка объектов настройки каталогов.</span><span class="sxs-lookup"><span data-stu-id="f5fb0-105">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="f5fb0-106">**Примечание.** Бета-версия этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="f5fb0-106">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f5fb0-107">Версия /v1.0 этого API переименована в *List groupSettings.*</span><span class="sxs-lookup"><span data-stu-id="f5fb0-107">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5fb0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5fb0-108">Permissions</span></span>
<span data-ttu-id="f5fb0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5fb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5fb0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5fb0-111">Permission type</span></span>      | <span data-ttu-id="f5fb0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5fb0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5fb0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5fb0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f5fb0-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5fb0-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f5fb0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5fb0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5fb0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5fb0-116">Not supported.</span></span>    |
|<span data-ttu-id="f5fb0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5fb0-117">Application</span></span> | <span data-ttu-id="f5fb0-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5fb0-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5fb0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5fb0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f5fb0-120">Список параметров клиента или группы</span><span class="sxs-lookup"><span data-stu-id="f5fb0-120">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5fb0-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f5fb0-121">Optional query parameters</span></span>
<span data-ttu-id="f5fb0-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f5fb0-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5fb0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5fb0-123">Request headers</span></span>
| <span data-ttu-id="f5fb0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f5fb0-124">Name</span></span>      |<span data-ttu-id="f5fb0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f5fb0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f5fb0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5fb0-126">Authorization</span></span>  | <span data-ttu-id="f5fb0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5fb0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5fb0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5fb0-129">Request body</span></span>
<span data-ttu-id="f5fb0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5fb0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5fb0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5fb0-131">Response</span></span>

<span data-ttu-id="f5fb0-132">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов directorySetting](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f5fb0-132">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5fb0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f5fb0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5fb0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5fb0-134">Request</span></span>
<span data-ttu-id="f5fb0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5fb0-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5fb0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5fb0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings
```
# <a name="c"></a>[<span data-ttu-id="f5fb0-137">C#</span><span class="sxs-lookup"><span data-stu-id="f5fb0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5fb0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5fb0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5fb0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5fb0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5fb0-140">Java</span><span class="sxs-lookup"><span data-stu-id="f5fb0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f5fb0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5fb0-141">Response</span></span>
<span data-ttu-id="f5fb0-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5fb0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
