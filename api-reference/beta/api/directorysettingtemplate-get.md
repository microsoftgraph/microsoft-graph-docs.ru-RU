---
title: Получение шаблона параметров каталога
description: Позволяет получать свойства объекта Директорисеттингтемплате, включая доступные параметры и их значения по умолчанию.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd1d622a5e03603276e54c013bcad9ff78e197fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008619"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="b0c0d-103">Получение шаблона параметров каталога</span><span class="sxs-lookup"><span data-stu-id="b0c0d-103">Get a directory setting template</span></span>

<span data-ttu-id="b0c0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c0d-105">Шаблон параметров каталога представляет шаблон параметров, параметры которых могут создаваться в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="b0c0d-106">Эта операция позволяет получать свойства объекта **директорисеттингтемплате** , включая доступные параметры и их значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-106">This operation allows retrieval of the properties of the **directorySettingTemplate** object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="b0c0d-107">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="b0c0d-108">Версия/v1.0 этого API была переименована, чтобы *получить groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0c0d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0c0d-109">Permissions</span></span>
<span data-ttu-id="b0c0d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0c0d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0c0d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0c0d-112">Permission type</span></span>      | <span data-ttu-id="b0c0d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0c0d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0c0d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0c0d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b0c0d-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0c0d-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0c0d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0c0d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0c0d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-117">Not supported.</span></span>    |
|<span data-ttu-id="b0c0d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0c0d-118">Application</span></span> | <span data-ttu-id="b0c0d-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0c0d-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0c0d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0c0d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0c0d-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0c0d-121">Optional query parameters</span></span>
<span data-ttu-id="b0c0d-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0c0d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0c0d-123">Request headers</span></span>
| <span data-ttu-id="b0c0d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b0c0d-124">Name</span></span>      |<span data-ttu-id="b0c0d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b0c0d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0c0d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0c0d-126">Authorization</span></span>  | <span data-ttu-id="b0c0d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0c0d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0c0d-129">Request body</span></span>
<span data-ttu-id="b0c0d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0c0d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0c0d-131">Response</span></span>

<span data-ttu-id="b0c0d-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [директорисеттингтемплате](../resources/directorysettingtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0c0d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b0c0d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0c0d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0c0d-134">Request</span></span>
<span data-ttu-id="b0c0d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0c0d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0c0d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="b0c0d-137">C#</span><span class="sxs-lookup"><span data-stu-id="b0c0d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0c0d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0c0d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0c0d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0c0d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0c0d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0c0d-140">Response</span></span>
<span data-ttu-id="b0c0d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0c0d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


