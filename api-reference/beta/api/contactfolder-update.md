---
title: Обновление объекта contactFolder
description: Обновление свойств объекта contactFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1d644e3f9f74a2ff34ad557f8dac97bc131f7f03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455585"
---
# <a name="update-contactfolder"></a><span data-ttu-id="74a5b-103">Обновление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="74a5b-103">Update contactfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74a5b-104">Обновление свойств объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="74a5b-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="74a5b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74a5b-105">Permissions</span></span>
<span data-ttu-id="74a5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74a5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74a5b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74a5b-108">Permission type</span></span>      | <span data-ttu-id="74a5b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74a5b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74a5b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74a5b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74a5b-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74a5b-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="74a5b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74a5b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74a5b-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74a5b-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="74a5b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74a5b-114">Application</span></span> | <span data-ttu-id="74a5b-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74a5b-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="74a5b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74a5b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="74a5b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74a5b-117">Request headers</span></span>
| <span data-ttu-id="74a5b-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74a5b-118">Header</span></span>       | <span data-ttu-id="74a5b-119">Значение</span><span class="sxs-lookup"><span data-stu-id="74a5b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74a5b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74a5b-120">Authorization</span></span>  | <span data-ttu-id="74a5b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74a5b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="74a5b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74a5b-123">Content-Type</span></span>  | <span data-ttu-id="74a5b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74a5b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74a5b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74a5b-126">Request body</span></span>
<span data-ttu-id="74a5b-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="74a5b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="74a5b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="74a5b-130">Property</span></span>     | <span data-ttu-id="74a5b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74a5b-131">Type</span></span>   |<span data-ttu-id="74a5b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74a5b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74a5b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="74a5b-133">displayName</span></span>|<span data-ttu-id="74a5b-134">String</span><span class="sxs-lookup"><span data-stu-id="74a5b-134">String</span></span>|<span data-ttu-id="74a5b-135">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="74a5b-135">The folder's display name.</span></span>|
|<span data-ttu-id="74a5b-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="74a5b-136">parentFolderId</span></span>|<span data-ttu-id="74a5b-137">String</span><span class="sxs-lookup"><span data-stu-id="74a5b-137">String</span></span>|<span data-ttu-id="74a5b-138">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="74a5b-138">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="74a5b-139">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="74a5b-139">wellKnownName</span></span>|<span data-ttu-id="74a5b-140">строка</span><span class="sxs-lookup"><span data-stu-id="74a5b-140">string</span></span>|<span data-ttu-id="74a5b-141">Имя папки, если она является распознаваемой папкой.</span><span class="sxs-lookup"><span data-stu-id="74a5b-141">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="74a5b-142">В `contacts` настоящее время это единственная распознанная папка контактов.</span><span class="sxs-lookup"><span data-stu-id="74a5b-142">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="74a5b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="74a5b-143">Response</span></span>

<span data-ttu-id="74a5b-144">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74a5b-144">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74a5b-145">Пример</span><span class="sxs-lookup"><span data-stu-id="74a5b-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74a5b-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="74a5b-146">Request</span></span>
<span data-ttu-id="74a5b-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74a5b-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="74a5b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="74a5b-148">Response</span></span>
<span data-ttu-id="74a5b-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74a5b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "wellKnownName": "wellKnownName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
