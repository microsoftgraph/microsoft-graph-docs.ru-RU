---
title: Обновление mailFolder
description: Обновление свойств объекта mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 63642678a58271bd0c0218879bf22504842c11e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540646"
---
# <a name="update-mailfolder"></a><span data-ttu-id="f9a85-103">Обновление mailFolder</span><span class="sxs-lookup"><span data-stu-id="f9a85-103">Update mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9a85-104">Обновление свойств объекта [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="f9a85-104">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9a85-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9a85-105">Permissions</span></span>
<span data-ttu-id="f9a85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9a85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9a85-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9a85-108">Permission type</span></span>      | <span data-ttu-id="f9a85-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9a85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9a85-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9a85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9a85-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9a85-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f9a85-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9a85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9a85-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9a85-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f9a85-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9a85-114">Application</span></span> | <span data-ttu-id="f9a85-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9a85-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9a85-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9a85-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f9a85-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9a85-117">Request headers</span></span>
| <span data-ttu-id="f9a85-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9a85-118">Header</span></span>       | <span data-ttu-id="f9a85-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f9a85-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9a85-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9a85-120">Authorization</span></span>  | <span data-ttu-id="f9a85-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9a85-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f9a85-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9a85-123">Content-Type</span></span>  | <span data-ttu-id="f9a85-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9a85-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9a85-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9a85-126">Request body</span></span>
<span data-ttu-id="f9a85-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f9a85-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f9a85-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9a85-130">Property</span></span>     | <span data-ttu-id="f9a85-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f9a85-131">Type</span></span>   |<span data-ttu-id="f9a85-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f9a85-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9a85-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f9a85-133">displayName</span></span>|<span data-ttu-id="f9a85-134">String</span><span class="sxs-lookup"><span data-stu-id="f9a85-134">String</span></span>|<span data-ttu-id="f9a85-135">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f9a85-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="f9a85-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9a85-136">Response</span></span>
<span data-ttu-id="f9a85-137">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9a85-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9a85-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f9a85-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f9a85-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9a85-139">Request</span></span>
<span data-ttu-id="f9a85-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9a85-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="f9a85-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9a85-141">Response</span></span>
<span data-ttu-id="f9a85-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f9a85-142">The following is an example of the response.</span></span>
><span data-ttu-id="f9a85-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f9a85-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f9a85-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9a85-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
