---
title: Создание объекта MailFolder
description: С помощью этого API можно создать дочернюю папку почты.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 44a61fda9120faaac0d8d69590c677896796765e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860034"
---
# <a name="create-mailfolder"></a><span data-ttu-id="0ea86-103">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="0ea86-103">Create MailFolder</span></span>

<span data-ttu-id="0ea86-104">С помощью этого API можно создать дочернюю папку почты.</span><span class="sxs-lookup"><span data-stu-id="0ea86-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea86-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ea86-105">Permissions</span></span>

<span data-ttu-id="0ea86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ea86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ea86-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ea86-108">Permission type</span></span> | <span data-ttu-id="0ea86-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ea86-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="0ea86-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ea86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ea86-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ea86-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ea86-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ea86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea86-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ea86-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ea86-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ea86-114">Application</span></span> | <span data-ttu-id="0ea86-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ea86-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ea86-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ea86-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="0ea86-117">Укажите родительской папки в URL-АДРЕСЕ запроса как идентификатор папки или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="0ea86-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="0ea86-118">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="0ea86-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ea86-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ea86-119">Request headers</span></span>

| <span data-ttu-id="0ea86-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ea86-120">Header</span></span> | <span data-ttu-id="0ea86-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0ea86-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="0ea86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea86-122">Authorization</span></span> | <span data-ttu-id="0ea86-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="0ea86-123"></span></span> <span data-ttu-id="0ea86-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ea86-124">Required.</span></span> |
| <span data-ttu-id="0ea86-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ea86-125">Content-Type</span></span> | <span data-ttu-id="0ea86-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="0ea86-126"></span></span> <span data-ttu-id="0ea86-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ea86-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ea86-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ea86-128">Request body</span></span>

<span data-ttu-id="0ea86-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0ea86-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="0ea86-130">**отображаемое имя** является свойством только для записи для объекта [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="0ea86-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="0ea86-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="0ea86-131">Parameter</span></span> | <span data-ttu-id="0ea86-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0ea86-132">Type</span></span> | <span data-ttu-id="0ea86-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0ea86-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="0ea86-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0ea86-134">displayName</span></span>|<span data-ttu-id="0ea86-135">String</span><span class="sxs-lookup"><span data-stu-id="0ea86-135">String</span></span>|<span data-ttu-id="0ea86-136">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="0ea86-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="0ea86-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ea86-137">Response</span></span>

<span data-ttu-id="0ea86-138">Успешно завершена, этот метод возвращает `201 Created` код ответа и ресурсов [mailFolder](../resources/mailfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ea86-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ea86-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0ea86-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ea86-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ea86-140">Request</span></span>

<span data-ttu-id="0ea86-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ea86-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a><span data-ttu-id="0ea86-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ea86-142">Response</span></span>
<span data-ttu-id="0ea86-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ea86-143">Here is an example of the response.</span></span>

> <span data-ttu-id="0ea86-144">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="0ea86-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0ea86-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ea86-145">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
