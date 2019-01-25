---
title: Обновление mailSearchFolder
description: Обновление для записи свойства объекта mailSearchFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 54e901751fc404ba2099205c6b16d86c99d9b05f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528468"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="5cf90-103">Обновление mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="5cf90-103">Update mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cf90-104">Обновление для записи свойства объекта [mailSearchFolder](../resources/mailsearchfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="5cf90-104">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cf90-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cf90-105">Permissions</span></span>
<span data-ttu-id="5cf90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cf90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cf90-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cf90-108">Permission type</span></span>      | <span data-ttu-id="5cf90-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cf90-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cf90-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cf90-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5cf90-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cf90-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5cf90-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cf90-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cf90-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cf90-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5cf90-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cf90-114">Application</span></span> | <span data-ttu-id="5cf90-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cf90-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cf90-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cf90-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5cf90-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cf90-117">Request headers</span></span>
| <span data-ttu-id="5cf90-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cf90-118">Header</span></span>       | <span data-ttu-id="5cf90-119">Значение</span><span class="sxs-lookup"><span data-stu-id="5cf90-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5cf90-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cf90-120">Authorization</span></span>  | <span data-ttu-id="5cf90-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cf90-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5cf90-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5cf90-123">Content-Type</span></span>  | <span data-ttu-id="5cf90-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cf90-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cf90-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cf90-126">Request body</span></span>
<span data-ttu-id="5cf90-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5cf90-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5cf90-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cf90-130">Property</span></span>     | <span data-ttu-id="5cf90-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5cf90-131">Type</span></span>   |<span data-ttu-id="5cf90-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5cf90-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5cf90-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5cf90-133">displayName</span></span> | <span data-ttu-id="5cf90-134">String</span><span class="sxs-lookup"><span data-stu-id="5cf90-134">String</span></span> | <span data-ttu-id="5cf90-135">Отображаемое имя [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5cf90-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="5cf90-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="5cf90-136">includeNestedFolders</span></span> | <span data-ttu-id="5cf90-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="5cf90-137">Boolean</span></span> | <span data-ttu-id="5cf90-138">Как следует обход иерархии папок почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5cf90-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="5cf90-139">`true`означает, что глубокого поиска должны быть в то время как `false` означает, что следует частичного поиска.</span><span class="sxs-lookup"><span data-stu-id="5cf90-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="5cf90-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="5cf90-140">sourceFolderIDs</span></span> | <span data-ttu-id="5cf90-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5cf90-141">String collection</span></span> | <span data-ttu-id="5cf90-142">Папки почтовых ящиков, которые должны быть получены.</span><span class="sxs-lookup"><span data-stu-id="5cf90-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="5cf90-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="5cf90-143">filterQuery</span></span> | <span data-ttu-id="5cf90-144">String</span><span class="sxs-lookup"><span data-stu-id="5cf90-144">String</span></span> | <span data-ttu-id="5cf90-145">Запросов OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="5cf90-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="5cf90-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cf90-146">Response</span></span>
<span data-ttu-id="5cf90-147">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cf90-147">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cf90-148">Пример</span><span class="sxs-lookup"><span data-stu-id="5cf90-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5cf90-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cf90-149">Request</span></span>
<span data-ttu-id="5cf90-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cf90-150">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="5cf90-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cf90-151">Response</span></span>
<span data-ttu-id="5cf90-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5cf90-152">The following is an example of the response.</span></span>
><span data-ttu-id="5cf90-153">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5cf90-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5cf90-154">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5cf90-154">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
