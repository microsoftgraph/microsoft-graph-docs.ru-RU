---
title: Получение параметра каталога
description: Получение свойств определенного объекта параметров каталога.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a31a3d647bf00a5a827ea43f6ecda1950f5221f0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956226"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="39da6-103">Получение параметра каталога</span><span class="sxs-lookup"><span data-stu-id="39da6-103">Get a directory setting</span></span>

<span data-ttu-id="39da6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39da6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39da6-105">Получение свойств определенного объекта параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="39da6-105">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="39da6-106">**Note** : версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="39da6-106">**Note** : The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="39da6-107">Версия/v1.0 этого API была переименована, чтобы *получить граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="39da6-107">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="39da6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39da6-108">Permissions</span></span>
<span data-ttu-id="39da6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39da6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39da6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39da6-111">Permission type</span></span>      | <span data-ttu-id="39da6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39da6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39da6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39da6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="39da6-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="39da6-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="39da6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39da6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39da6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39da6-116">Not supported.</span></span>    |
|<span data-ttu-id="39da6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39da6-117">Application</span></span> | <span data-ttu-id="39da6-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39da6-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39da6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39da6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="39da6-120">Получение определенного параметра на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="39da6-120">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="39da6-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="39da6-121">Optional query parameters</span></span>
<span data-ttu-id="39da6-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="39da6-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39da6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39da6-123">Request headers</span></span>
| <span data-ttu-id="39da6-124">Имя</span><span class="sxs-lookup"><span data-stu-id="39da6-124">Name</span></span>      |<span data-ttu-id="39da6-125">Описание</span><span class="sxs-lookup"><span data-stu-id="39da6-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39da6-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39da6-126">Authorization</span></span>  | <span data-ttu-id="39da6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39da6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39da6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39da6-129">Request body</span></span>
<span data-ttu-id="39da6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39da6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39da6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="39da6-131">Response</span></span>

<span data-ttu-id="39da6-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39da6-132">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39da6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="39da6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39da6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="39da6-134">Request</span></span>
<span data-ttu-id="39da6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39da6-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39da6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="39da6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="39da6-137">C#</span><span class="sxs-lookup"><span data-stu-id="39da6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39da6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39da6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39da6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39da6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39da6-140">Java</span><span class="sxs-lookup"><span data-stu-id="39da6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="39da6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="39da6-141">Response</span></span>
<span data-ttu-id="39da6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39da6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
