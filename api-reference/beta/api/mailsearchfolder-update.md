---
title: Обновление Маилсеарчфолдер
description: Обновление свойств, доступных для записи, объекта Маилсеарчфолдер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: fb11e06ac450aa218a8e1102557eb9e3a79f874c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598199"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="01f6c-103">Обновление Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="01f6c-103">Update mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01f6c-104">Обновление свойств, доступных для записи, объекта [маилсеарчфолдер](../resources/mailsearchfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="01f6c-104">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="01f6c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01f6c-105">Permissions</span></span>
<span data-ttu-id="01f6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01f6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f6c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01f6c-108">Permission type</span></span>      | <span data-ttu-id="01f6c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01f6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01f6c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01f6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01f6c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01f6c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="01f6c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01f6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01f6c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01f6c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="01f6c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01f6c-114">Application</span></span> | <span data-ttu-id="01f6c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01f6c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="01f6c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01f6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="01f6c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01f6c-117">Request headers</span></span>
| <span data-ttu-id="01f6c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01f6c-118">Header</span></span>       | <span data-ttu-id="01f6c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="01f6c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01f6c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01f6c-120">Authorization</span></span>  | <span data-ttu-id="01f6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01f6c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01f6c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01f6c-123">Content-Type</span></span>  | <span data-ttu-id="01f6c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01f6c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01f6c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01f6c-126">Request body</span></span>
<span data-ttu-id="01f6c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="01f6c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="01f6c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01f6c-130">Property</span></span>     | <span data-ttu-id="01f6c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01f6c-131">Type</span></span>   |<span data-ttu-id="01f6c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01f6c-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="01f6c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="01f6c-133">displayName</span></span> | <span data-ttu-id="01f6c-134">String</span><span class="sxs-lookup"><span data-stu-id="01f6c-134">String</span></span> | <span data-ttu-id="01f6c-135">Отображаемое имя [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="01f6c-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="01f6c-136">Инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="01f6c-136">includeNestedFolders</span></span> | <span data-ttu-id="01f6c-137">Логический</span><span class="sxs-lookup"><span data-stu-id="01f6c-137">Boolean</span></span> | <span data-ttu-id="01f6c-138">Способ обхода иерархии папок почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="01f6c-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="01f6c-139">`true`означает, что следует выполнить глубокий поиск, а `false` это означает, что вместо этого следует выполнить неглубокий Поиск.</span><span class="sxs-lookup"><span data-stu-id="01f6c-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="01f6c-140">Саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="01f6c-140">sourceFolderIDs</span></span> | <span data-ttu-id="01f6c-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="01f6c-141">String collection</span></span> | <span data-ttu-id="01f6c-142">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="01f6c-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="01f6c-143">Филтеркуери</span><span class="sxs-lookup"><span data-stu-id="01f6c-143">filterQuery</span></span> | <span data-ttu-id="01f6c-144">String</span><span class="sxs-lookup"><span data-stu-id="01f6c-144">String</span></span> | <span data-ttu-id="01f6c-145">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="01f6c-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="01f6c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="01f6c-146">Response</span></span>
<span data-ttu-id="01f6c-147">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01f6c-147">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01f6c-148">Пример</span><span class="sxs-lookup"><span data-stu-id="01f6c-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="01f6c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="01f6c-149">Request</span></span>
<span data-ttu-id="01f6c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01f6c-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')))"
}
```

#### <a name="response"></a><span data-ttu-id="01f6c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="01f6c-151">Response</span></span>
<span data-ttu-id="01f6c-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01f6c-152">The following is an example of the response.</span></span>
><span data-ttu-id="01f6c-153">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="01f6c-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="01f6c-154">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01f6c-154">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="01f6c-155">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="01f6c-155">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01f6c-156">Язык</span><span class="sxs-lookup"><span data-stu-id="01f6c-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_mailsearchfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
