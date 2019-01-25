---
title: 'mailFolder: move'
description: Перемещение папки почты со всем ее содержимым в другую папку почты.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 836c91ee2bfd234c5c831511d1be45800be8660a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512131"
---
# <a name="mailfolder-move"></a><span data-ttu-id="10558-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="10558-103">mailFolder: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10558-104">Перемещение папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="10558-104">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="10558-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10558-105">Permissions</span></span>

<span data-ttu-id="10558-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10558-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10558-108">Permission type</span></span> | <span data-ttu-id="10558-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10558-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="10558-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10558-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10558-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10558-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="10558-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10558-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10558-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10558-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="10558-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10558-114">Application</span></span> | <span data-ttu-id="10558-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10558-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="10558-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10558-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="10558-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10558-117">Request headers</span></span>

| <span data-ttu-id="10558-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10558-118">Header</span></span> | <span data-ttu-id="10558-119">Значение</span><span class="sxs-lookup"><span data-stu-id="10558-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="10558-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="10558-120">Authorization</span></span> | <span data-ttu-id="10558-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="10558-121"></span></span> <span data-ttu-id="10558-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10558-122">Required.</span></span> |
| <span data-ttu-id="10558-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10558-123">Content-Type</span></span> | <span data-ttu-id="10558-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="10558-124"></span></span> <span data-ttu-id="10558-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10558-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10558-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10558-126">Request body</span></span>

<span data-ttu-id="10558-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="10558-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="10558-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="10558-128">Parameter</span></span> | <span data-ttu-id="10558-129">Тип</span><span class="sxs-lookup"><span data-stu-id="10558-129">Type</span></span> | <span data-ttu-id="10558-130">Описание</span><span class="sxs-lookup"><span data-stu-id="10558-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="10558-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="10558-131">destinationId</span></span>|<span data-ttu-id="10558-132">String</span><span class="sxs-lookup"><span data-stu-id="10558-132">String</span></span>|<span data-ttu-id="10558-133">Идентификатор папки, или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="10558-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="10558-134">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="10558-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="10558-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="10558-135">Response</span></span>

<span data-ttu-id="10558-136">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [mailFolder](../resources/mailfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="10558-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10558-137">Пример</span><span class="sxs-lookup"><span data-stu-id="10558-137">Example</span></span>

<span data-ttu-id="10558-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="10558-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="10558-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="10558-139">Request</span></span>

<span data-ttu-id="10558-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10558-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="10558-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="10558-141">Response</span></span>

<span data-ttu-id="10558-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10558-142">Here is an example of the response.</span></span>

> <span data-ttu-id="10558-143">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="10558-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="10558-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10558-144">All the properties will be returned from an actual call.</span></span>
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
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-move.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
