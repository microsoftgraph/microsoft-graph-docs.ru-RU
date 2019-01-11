---
title: 'mailFolder: move'
description: Перемещение папки почты со всем ее содержимым в другую папку почты.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 8d96e01c54c91b3de38b0594c29e38ccf8691603
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831117"
---
# <a name="mailfolder-move"></a><span data-ttu-id="24fa6-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="24fa6-103">mailFolder: move</span></span>

> <span data-ttu-id="24fa6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="24fa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24fa6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24fa6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24fa6-106">Перемещение папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="24fa6-106">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="24fa6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24fa6-107">Permissions</span></span>

<span data-ttu-id="24fa6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24fa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24fa6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24fa6-110">Permission type</span></span> | <span data-ttu-id="24fa6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24fa6-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="24fa6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24fa6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="24fa6-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24fa6-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="24fa6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24fa6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24fa6-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24fa6-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="24fa6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24fa6-116">Application</span></span> | <span data-ttu-id="24fa6-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24fa6-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="24fa6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24fa6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="24fa6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24fa6-119">Request headers</span></span>

| <span data-ttu-id="24fa6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24fa6-120">Header</span></span> | <span data-ttu-id="24fa6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="24fa6-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="24fa6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24fa6-122">Authorization</span></span> | <span data-ttu-id="24fa6-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="24fa6-123"></span></span> <span data-ttu-id="24fa6-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24fa6-124">Required.</span></span> |
| <span data-ttu-id="24fa6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24fa6-125">Content-Type</span></span> | <span data-ttu-id="24fa6-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="24fa6-126"></span></span> <span data-ttu-id="24fa6-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24fa6-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24fa6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24fa6-128">Request body</span></span>

<span data-ttu-id="24fa6-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="24fa6-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24fa6-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="24fa6-130">Parameter</span></span> | <span data-ttu-id="24fa6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="24fa6-131">Type</span></span> | <span data-ttu-id="24fa6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="24fa6-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="24fa6-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="24fa6-133">destinationId</span></span>|<span data-ttu-id="24fa6-134">String</span><span class="sxs-lookup"><span data-stu-id="24fa6-134">String</span></span>|<span data-ttu-id="24fa6-135">Идентификатор папки, или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="24fa6-135">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="24fa6-136">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="24fa6-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="24fa6-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="24fa6-137">Response</span></span>

<span data-ttu-id="24fa6-138">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [mailFolder](../resources/mailfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="24fa6-138">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24fa6-139">Пример</span><span class="sxs-lookup"><span data-stu-id="24fa6-139">Example</span></span>

<span data-ttu-id="24fa6-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="24fa6-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="24fa6-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="24fa6-141">Request</span></span>

<span data-ttu-id="24fa6-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24fa6-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="24fa6-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="24fa6-143">Response</span></span>

<span data-ttu-id="24fa6-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="24fa6-144">Here is an example of the response.</span></span>

> <span data-ttu-id="24fa6-145">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="24fa6-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="24fa6-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24fa6-146">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
