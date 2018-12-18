---
title: 'mailFolder: copy'
description: Копирование папки почты со всем ее содержимым в другую папку почты.
author: angelgolfer-ms
ms.openlocfilehash: 74a9c072089f3bd76439ce0fa7bd15f28f8cae2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335625"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="1082b-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="1082b-103">mailFolder: copy</span></span>

> <span data-ttu-id="1082b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1082b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1082b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1082b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1082b-106">Копирование папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="1082b-106">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1082b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1082b-107">Permissions</span></span>

<span data-ttu-id="1082b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1082b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1082b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1082b-110">Permission type</span></span> | <span data-ttu-id="1082b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1082b-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="1082b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1082b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1082b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1082b-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1082b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1082b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1082b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1082b-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1082b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1082b-116">Application</span></span> | <span data-ttu-id="1082b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1082b-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1082b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1082b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="1082b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1082b-119">Request headers</span></span>

| <span data-ttu-id="1082b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1082b-120">Header</span></span> | <span data-ttu-id="1082b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1082b-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="1082b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1082b-122">Authorization</span></span> | <span data-ttu-id="1082b-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="1082b-123"></span></span> <span data-ttu-id="1082b-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1082b-124">Required.</span></span> |
| <span data-ttu-id="1082b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1082b-125">Content-Type</span></span> | <span data-ttu-id="1082b-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="1082b-126"></span></span> <span data-ttu-id="1082b-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1082b-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1082b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1082b-128">Request body</span></span>

<span data-ttu-id="1082b-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1082b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1082b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="1082b-130">Parameter</span></span> | <span data-ttu-id="1082b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1082b-131">Type</span></span> | <span data-ttu-id="1082b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1082b-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="1082b-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="1082b-133">destinationId</span></span>|<span data-ttu-id="1082b-134">String</span><span class="sxs-lookup"><span data-stu-id="1082b-134">String</span></span>|<span data-ttu-id="1082b-135">Идентификатор папки, или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="1082b-135">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="1082b-136">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="1082b-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="1082b-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="1082b-137">Response</span></span>

<span data-ttu-id="1082b-138">Успешно завершена, этот метод возвращает `200 OK` код ответа и ресурсов [mailFolder](../resources/mailfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1082b-138">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1082b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="1082b-139">Example</span></span>

<span data-ttu-id="1082b-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1082b-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1082b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1082b-141">Request</span></span>

<span data-ttu-id="1082b-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1082b-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="1082b-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="1082b-143">Response</span></span>

<span data-ttu-id="1082b-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1082b-144">Here is an example of the response.</span></span>

> <span data-ttu-id="1082b-145">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="1082b-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1082b-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1082b-146">All the properties will be returned from an actual call.</span></span>

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
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
