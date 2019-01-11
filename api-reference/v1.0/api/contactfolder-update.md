---
title: Обновление объекта contactFolder
description: Обновление свойств объекта contactfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 01ecca2b59482c1c2c75096b711904f3054fd338
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836423"
---
# <a name="update-contactfolder"></a><span data-ttu-id="b7af9-103">Обновление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="b7af9-103">Update contactfolder</span></span>

<span data-ttu-id="b7af9-104">Обновление свойств объекта contactfolder.</span><span class="sxs-lookup"><span data-stu-id="b7af9-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7af9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7af9-105">Permissions</span></span>
<span data-ttu-id="b7af9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7af9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7af9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7af9-108">Permission type</span></span>      | <span data-ttu-id="b7af9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7af9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7af9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7af9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7af9-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7af9-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b7af9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7af9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7af9-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7af9-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b7af9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7af9-114">Application</span></span> | <span data-ttu-id="b7af9-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7af9-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7af9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7af9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b7af9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7af9-117">Request headers</span></span>
| <span data-ttu-id="b7af9-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7af9-118">Header</span></span>       | <span data-ttu-id="b7af9-119">Значение</span><span class="sxs-lookup"><span data-stu-id="b7af9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7af9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7af9-120">Authorization</span></span>  | <span data-ttu-id="b7af9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7af9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b7af9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7af9-123">Content-Type</span></span>  | <span data-ttu-id="b7af9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7af9-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7af9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7af9-126">Request body</span></span>
<span data-ttu-id="b7af9-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b7af9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b7af9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7af9-130">Property</span></span>     | <span data-ttu-id="b7af9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b7af9-131">Type</span></span>   |<span data-ttu-id="b7af9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b7af9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7af9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b7af9-133">displayName</span></span>|<span data-ttu-id="b7af9-134">String</span><span class="sxs-lookup"><span data-stu-id="b7af9-134">String</span></span>|<span data-ttu-id="b7af9-135">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="b7af9-135">The folder's display name.</span></span>|
|<span data-ttu-id="b7af9-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b7af9-136">parentFolderId</span></span>|<span data-ttu-id="b7af9-137">String</span><span class="sxs-lookup"><span data-stu-id="b7af9-137">String</span></span>|<span data-ttu-id="b7af9-138">Идентификатор родительской папки для данной папки.</span><span class="sxs-lookup"><span data-stu-id="b7af9-138">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="b7af9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7af9-139">Response</span></span>

<span data-ttu-id="b7af9-140">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7af9-140">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7af9-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b7af9-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7af9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7af9-142">Request</span></span>
<span data-ttu-id="b7af9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7af9-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="b7af9-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7af9-144">Response</span></span>
<span data-ttu-id="b7af9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b7af9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
