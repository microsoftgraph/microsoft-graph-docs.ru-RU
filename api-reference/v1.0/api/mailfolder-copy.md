---
title: 'mailFolder: copy'
description: Копирование папки почты со всем ее содержимым в другую папку почты.
author: angelgolfer-ms
ms.openlocfilehash: 44df53219e00479cdc48d057286f1af410e13c77
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356928"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="f8962-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="f8962-103">mailFolder: copy</span></span>

<span data-ttu-id="f8962-104">Копирование папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="f8962-104">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8962-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8962-105">Permissions</span></span>

<span data-ttu-id="f8962-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8962-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8962-108">Permission type</span></span> | <span data-ttu-id="f8962-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8962-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="f8962-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8962-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f8962-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8962-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f8962-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8962-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8962-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8962-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f8962-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8962-114">Application</span></span> | <span data-ttu-id="f8962-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8962-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8962-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8962-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="f8962-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8962-117">Request headers</span></span>
| <span data-ttu-id="f8962-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8962-118">Header</span></span> | <span data-ttu-id="f8962-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f8962-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="f8962-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8962-120">Authorization</span></span> | <span data-ttu-id="f8962-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="f8962-121"></span></span> <span data-ttu-id="f8962-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8962-122">Required.</span></span> |
| <span data-ttu-id="f8962-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8962-123">Content-Type</span></span> | <span data-ttu-id="f8962-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="f8962-124"></span></span> <span data-ttu-id="f8962-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8962-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8962-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8962-126">Request body</span></span>

<span data-ttu-id="f8962-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f8962-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8962-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="f8962-128">Parameter</span></span> | <span data-ttu-id="f8962-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f8962-129">Type</span></span> | <span data-ttu-id="f8962-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f8962-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="f8962-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="f8962-131">destinationId</span></span>|<span data-ttu-id="f8962-132">String</span><span class="sxs-lookup"><span data-stu-id="f8962-132">String</span></span>|<span data-ttu-id="f8962-133">Идентификатор папки, или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="f8962-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="f8962-134">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f8962-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="f8962-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8962-135">Response</span></span>

<span data-ttu-id="f8962-136">Успешно завершена, этот метод возвращает `200 OK` код ответа и ресурсов [mailFolder](../resources/mailfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f8962-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8962-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f8962-137">Example</span></span>

<span data-ttu-id="f8962-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f8962-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f8962-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8962-139">Request</span></span>
<span data-ttu-id="f8962-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8962-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="f8962-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8962-141">Response</span></span>

<span data-ttu-id="f8962-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f8962-142">Here is an example of the response.</span></span>

> <span data-ttu-id="f8962-143">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="f8962-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f8962-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8962-144">All the properties will be returned from an actual call.</span></span>
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
