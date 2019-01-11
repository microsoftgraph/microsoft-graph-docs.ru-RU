---
title: Обновление mailSearchFolder
description: Обновление для записи свойства объекта mailSearchFolder.
localization_priority: Normal
ms.openlocfilehash: 843dbe4d4312fdeb3485b0eb9e441a76b761dd46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867231"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="6d035-103">Обновление mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="6d035-103">Update mailSearchFolder</span></span>

> <span data-ttu-id="6d035-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6d035-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d035-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d035-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d035-106">Обновление для записи свойства объекта [mailSearchFolder](../resources/mailsearchfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="6d035-106">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d035-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d035-107">Permissions</span></span>
<span data-ttu-id="6d035-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d035-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d035-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d035-110">Permission type</span></span>      | <span data-ttu-id="6d035-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d035-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d035-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d035-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d035-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d035-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6d035-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d035-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d035-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d035-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6d035-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d035-116">Application</span></span> | <span data-ttu-id="6d035-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d035-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d035-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d035-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6d035-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d035-119">Request headers</span></span>
| <span data-ttu-id="6d035-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d035-120">Header</span></span>       | <span data-ttu-id="6d035-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6d035-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d035-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d035-122">Authorization</span></span>  | <span data-ttu-id="6d035-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d035-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6d035-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d035-125">Content-Type</span></span>  | <span data-ttu-id="6d035-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d035-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d035-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d035-128">Request body</span></span>
<span data-ttu-id="6d035-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6d035-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6d035-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d035-132">Property</span></span>     | <span data-ttu-id="6d035-133">Тип</span><span class="sxs-lookup"><span data-stu-id="6d035-133">Type</span></span>   |<span data-ttu-id="6d035-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6d035-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d035-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6d035-135">displayName</span></span> | <span data-ttu-id="6d035-136">Строка</span><span class="sxs-lookup"><span data-stu-id="6d035-136">String</span></span> | <span data-ttu-id="6d035-137">Отображаемое имя [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6d035-137">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="6d035-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="6d035-138">includeNestedFolders</span></span> | <span data-ttu-id="6d035-139">Логический</span><span class="sxs-lookup"><span data-stu-id="6d035-139">Boolean</span></span> | <span data-ttu-id="6d035-140">Как следует обход иерархии папок почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6d035-140">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="6d035-141">`true`означает, что глубокого поиска должны быть в то время как `false` означает, что следует частичного поиска.</span><span class="sxs-lookup"><span data-stu-id="6d035-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="6d035-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="6d035-142">sourceFolderIDs</span></span> | <span data-ttu-id="6d035-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6d035-143">String collection</span></span> | <span data-ttu-id="6d035-144">Папки почтовых ящиков, которые должны быть получены.</span><span class="sxs-lookup"><span data-stu-id="6d035-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="6d035-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="6d035-145">filterQuery</span></span> | <span data-ttu-id="6d035-146">Строка</span><span class="sxs-lookup"><span data-stu-id="6d035-146">String</span></span> | <span data-ttu-id="6d035-147">Запросов OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="6d035-147">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="6d035-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d035-148">Response</span></span>
<span data-ttu-id="6d035-149">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d035-149">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d035-150">Пример</span><span class="sxs-lookup"><span data-stu-id="6d035-150">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6d035-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d035-151">Request</span></span>
<span data-ttu-id="6d035-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d035-152">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="6d035-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d035-153">Response</span></span>
<span data-ttu-id="6d035-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6d035-154">The following is an example of the response.</span></span>
><span data-ttu-id="6d035-155">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="6d035-155">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d035-156">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d035-156">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
