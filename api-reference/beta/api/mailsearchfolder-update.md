---
title: Обновление Маилсеарчфолдер
description: Обновление свойств, доступных для записи, объекта Маилсеарчфолдер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6b5dee2fae2da89cd9fdff43465f1e57e3f57407
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812896"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="ba320-103">Обновление Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="ba320-103">Update mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba320-104">Обновление свойств, доступных для записи, объекта [маилсеарчфолдер](../resources/mailsearchfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="ba320-104">Update the writable properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba320-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba320-105">Permissions</span></span>
<span data-ttu-id="ba320-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba320-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba320-108">Permission type</span></span>      | <span data-ttu-id="ba320-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba320-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba320-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba320-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ba320-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba320-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ba320-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba320-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba320-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba320-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ba320-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba320-114">Application</span></span> | <span data-ttu-id="ba320-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba320-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba320-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba320-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba320-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba320-117">Request headers</span></span>
| <span data-ttu-id="ba320-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba320-118">Header</span></span>       | <span data-ttu-id="ba320-119">Значение</span><span class="sxs-lookup"><span data-stu-id="ba320-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba320-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba320-120">Authorization</span></span>  | <span data-ttu-id="ba320-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba320-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ba320-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba320-123">Content-Type</span></span>  | <span data-ttu-id="ba320-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba320-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba320-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba320-126">Request body</span></span>
<span data-ttu-id="ba320-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ba320-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ba320-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="ba320-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ba320-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ba320-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ba320-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba320-130">Property</span></span>     | <span data-ttu-id="ba320-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ba320-131">Type</span></span>   |<span data-ttu-id="ba320-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ba320-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba320-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ba320-133">displayName</span></span> | <span data-ttu-id="ba320-134">String</span><span class="sxs-lookup"><span data-stu-id="ba320-134">String</span></span> | <span data-ttu-id="ba320-135">Отображаемое имя [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ba320-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="ba320-136">Инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="ba320-136">includeNestedFolders</span></span> | <span data-ttu-id="ba320-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba320-137">Boolean</span></span> | <span data-ttu-id="ba320-138">Способ обхода иерархии папок почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="ba320-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="ba320-139">`true`означает, что следует выполнить глубокий поиск, а `false` это означает, что вместо этого следует выполнить неглубокий Поиск.</span><span class="sxs-lookup"><span data-stu-id="ba320-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="ba320-140">Саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="ba320-140">sourceFolderIds</span></span> | <span data-ttu-id="ba320-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ba320-141">String collection</span></span> | <span data-ttu-id="ba320-142">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="ba320-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="ba320-143">Филтеркуери</span><span class="sxs-lookup"><span data-stu-id="ba320-143">filterQuery</span></span> | <span data-ttu-id="ba320-144">String</span><span class="sxs-lookup"><span data-stu-id="ba320-144">String</span></span> | <span data-ttu-id="ba320-145">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="ba320-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="ba320-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba320-146">Response</span></span>
<span data-ttu-id="ba320-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba320-147">If successful, this method returns a `200 OK` response code and an updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba320-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ba320-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ba320-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba320-149">Request</span></span>
<span data-ttu-id="ba320-150">Ниже приведен пример запроса, который обновляет свойство **филтеркуери** папки поиска.</span><span class="sxs-lookup"><span data-stu-id="ba320-150">The following is an example request that updates the **filterQuery** property of the search folder.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')"
}
```

#### <a name="response"></a><span data-ttu-id="ba320-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba320-151">Response</span></span>
<span data-ttu-id="ba320-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba320-152">The following is an example of the response.</span></span>
><span data-ttu-id="ba320-153">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ba320-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ba320-154">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba320-154">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
  "sourceFolderIds": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ba320-155">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ba320-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ba320-156">C#</span><span class="sxs-lookup"><span data-stu-id="ba320-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_mailsearchfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba320-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="ba320-157">Javascript</span></span>](#tab/javascript)
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
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
