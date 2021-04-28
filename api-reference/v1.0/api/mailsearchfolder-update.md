---
title: Обновление mailSearchFolder
description: Обновим свойства объекта mailSearchFolder.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 590a886b73dd0adc5f08f895028e2848ed84fb60
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035388"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="a5c99-103">Обновление mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="a5c99-103">Update mailSearchFolder</span></span>

<span data-ttu-id="a5c99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5c99-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5c99-105">Обновим свойства объекта [mailSearchFolder.](../resources/mailsearchfolder.md)</span><span class="sxs-lookup"><span data-stu-id="a5c99-105">Update the writable properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5c99-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c99-106">Permissions</span></span>
<span data-ttu-id="a5c99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5c99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5c99-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c99-109">Permission type</span></span>      | <span data-ttu-id="a5c99-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5c99-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5c99-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5c99-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5c99-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5c99-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a5c99-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5c99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5c99-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5c99-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a5c99-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5c99-115">Application</span></span> | <span data-ttu-id="a5c99-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5c99-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5c99-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5c99-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5c99-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5c99-118">Request headers</span></span>
| <span data-ttu-id="a5c99-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5c99-119">Header</span></span>       | <span data-ttu-id="a5c99-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a5c99-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5c99-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5c99-121">Authorization</span></span>  | <span data-ttu-id="a5c99-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5c99-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a5c99-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5c99-124">Content-Type</span></span>  | <span data-ttu-id="a5c99-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5c99-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5c99-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5c99-127">Request body</span></span>
<span data-ttu-id="a5c99-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a5c99-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a5c99-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a5c99-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a5c99-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a5c99-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a5c99-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5c99-131">Property</span></span>     | <span data-ttu-id="a5c99-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a5c99-132">Type</span></span>   |<span data-ttu-id="a5c99-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a5c99-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5c99-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a5c99-134">displayName</span></span> | <span data-ttu-id="a5c99-135">String</span><span class="sxs-lookup"><span data-stu-id="a5c99-135">String</span></span> | <span data-ttu-id="a5c99-136">Имя отображения [почтыFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a5c99-136">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="a5c99-137">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="a5c99-137">includeNestedFolders</span></span> | <span data-ttu-id="a5c99-138">Логический</span><span class="sxs-lookup"><span data-stu-id="a5c99-138">Boolean</span></span> | <span data-ttu-id="a5c99-139">Как должна проходить иерархия папок почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="a5c99-139">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="a5c99-140">`true` означает, что глубокий поиск должен быть сделан, а значит, неглубокий `false` поиск должен быть сделан вместо.</span><span class="sxs-lookup"><span data-stu-id="a5c99-140">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="a5c99-141">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="a5c99-141">sourceFolderIds</span></span> | <span data-ttu-id="a5c99-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a5c99-142">String collection</span></span> | <span data-ttu-id="a5c99-143">Папки почтовых ящиков, которые необходимо добыть.</span><span class="sxs-lookup"><span data-stu-id="a5c99-143">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="a5c99-144">filterQuery</span><span class="sxs-lookup"><span data-stu-id="a5c99-144">filterQuery</span></span> | <span data-ttu-id="a5c99-145">String</span><span class="sxs-lookup"><span data-stu-id="a5c99-145">String</span></span> | <span data-ttu-id="a5c99-146">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="a5c99-146">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="a5c99-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c99-147">Response</span></span>
<span data-ttu-id="a5c99-148">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [mailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5c99-148">If successful, this method returns a `200 OK` response code and an updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5c99-149">Пример</span><span class="sxs-lookup"><span data-stu-id="a5c99-149">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a5c99-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5c99-150">Request</span></span>
<span data-ttu-id="a5c99-151">Ниже приводится пример запроса, который обновляет **свойство filterQuery** папки поиска.</span><span class="sxs-lookup"><span data-stu-id="a5c99-151">The following is an example request that updates the **filterQuery** property of the search folder.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5c99-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5c99-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')"
}
```
# <a name="c"></a>[<span data-ttu-id="a5c99-153">C#</span><span class="sxs-lookup"><span data-stu-id="a5c99-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5c99-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5c99-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5c99-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5c99-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5c99-156">Java</span><span class="sxs-lookup"><span data-stu-id="a5c99-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a5c99-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c99-157">Response</span></span>
<span data-ttu-id="a5c99-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5c99-158">The following is an example of the response.</span></span>
><span data-ttu-id="a5c99-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5c99-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```

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

  ]
}
-->

