---
title: Создание объекта MailFolder
description: С помощью этого API можно создать дочернюю папку почты.
ms.openlocfilehash: 79ed32a316a9012c33d3c08d0c95f00ad2f90725
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027882"
---
# <a name="create-mailfolder"></a><span data-ttu-id="ceeb5-103">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="ceeb5-103">Create MailFolder</span></span>

<span data-ttu-id="ceeb5-104">С помощью этого API можно создать дочернюю папку почты.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ceeb5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ceeb5-105">Permissions</span></span>

<span data-ttu-id="ceeb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceeb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ceeb5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ceeb5-108">Permission type</span></span> | <span data-ttu-id="ceeb5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ceeb5-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="ceeb5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ceeb5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ceeb5-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceeb5-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ceeb5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ceeb5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceeb5-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceeb5-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ceeb5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ceeb5-114">Application</span></span> | <span data-ttu-id="ceeb5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceeb5-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ceeb5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ceeb5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="ceeb5-117">Укажите родительской папки в URL-АДРЕСЕ запроса как идентификатор папки или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="ceeb5-118">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ceeb5-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ceeb5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ceeb5-119">Request headers</span></span>

| <span data-ttu-id="ceeb5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ceeb5-120">Header</span></span> | <span data-ttu-id="ceeb5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ceeb5-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="ceeb5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceeb5-122">Authorization</span></span> | <span data-ttu-id="ceeb5-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-123"></span></span> <span data-ttu-id="ceeb5-124">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-124">Required.</span></span> |
| <span data-ttu-id="ceeb5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ceeb5-125">Content-Type</span></span> | <span data-ttu-id="ceeb5-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-126"></span></span> <span data-ttu-id="ceeb5-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ceeb5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ceeb5-128">Request body</span></span>

<span data-ttu-id="ceeb5-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="ceeb5-130">**отображаемое имя** является свойством только для записи для объекта [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="ceeb5-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="ceeb5-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="ceeb5-131">Parameter</span></span> | <span data-ttu-id="ceeb5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ceeb5-132">Type</span></span> | <span data-ttu-id="ceeb5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ceeb5-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="ceeb5-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ceeb5-134">displayName</span></span>|<span data-ttu-id="ceeb5-135">String</span><span class="sxs-lookup"><span data-stu-id="ceeb5-135">String</span></span>|<span data-ttu-id="ceeb5-136">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="ceeb5-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceeb5-137">Response</span></span>

<span data-ttu-id="ceeb5-138">Успешно завершена, этот метод возвращает `201 Created` код ответа и ресурсов [mailFolder](../resources/mailfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceeb5-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ceeb5-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ceeb5-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ceeb5-140">Request</span></span>

<span data-ttu-id="ceeb5-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ceeb5-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceeb5-142">Response</span></span>
<span data-ttu-id="ceeb5-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-143">Here is an example of the response.</span></span>

> <span data-ttu-id="ceeb5-144">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ceeb5-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ceeb5-145">All the properties will be returned from an actual call.</span></span>
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
