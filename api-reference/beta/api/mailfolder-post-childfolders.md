---
title: Создание mailFolder
description: Используйте этот интерфейс API для создания нового дочернего mailFolder.
author: angelgolfer-ms
ms.openlocfilehash: e893f28878b14fa76d8cda16a5b37f795ed235f2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357276"
---
# <a name="create-mailfolder"></a><span data-ttu-id="52466-103">Создание mailFolder</span><span class="sxs-lookup"><span data-stu-id="52466-103">Create mailFolder</span></span>

> <span data-ttu-id="52466-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="52466-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52466-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52466-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52466-106">Используйте этот интерфейс API для создания нового дочернего [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="52466-106">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="52466-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52466-107">Permissions</span></span>

<span data-ttu-id="52466-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52466-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52466-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52466-110">Permission type</span></span> | <span data-ttu-id="52466-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52466-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="52466-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52466-112">Delegated (work or school account)</span></span> | <span data-ttu-id="52466-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52466-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="52466-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52466-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52466-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52466-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="52466-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52466-116">Application</span></span> | <span data-ttu-id="52466-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52466-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="52466-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52466-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="52466-119">Укажите родительской папки в URL-АДРЕСЕ запроса как идентификатор папки или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="52466-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="52466-120">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="52466-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="52466-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52466-121">Request headers</span></span>

| <span data-ttu-id="52466-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52466-122">Header</span></span> | <span data-ttu-id="52466-123">Значение</span><span class="sxs-lookup"><span data-stu-id="52466-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="52466-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52466-124">Authorization</span></span> | <span data-ttu-id="52466-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="52466-125"></span></span> <span data-ttu-id="52466-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52466-126">Required.</span></span> |
| <span data-ttu-id="52466-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52466-127">Content-Type</span></span> | <span data-ttu-id="52466-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="52466-128"></span></span> <span data-ttu-id="52466-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52466-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52466-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52466-130">Request body</span></span>

<span data-ttu-id="52466-p106">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="52466-p106">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="52466-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="52466-133">Parameter</span></span> | <span data-ttu-id="52466-134">Тип</span><span class="sxs-lookup"><span data-stu-id="52466-134">Type</span></span> | <span data-ttu-id="52466-135">Описание</span><span class="sxs-lookup"><span data-stu-id="52466-135">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="52466-136">displayName</span><span class="sxs-lookup"><span data-stu-id="52466-136">displayName</span></span>|<span data-ttu-id="52466-137">String</span><span class="sxs-lookup"><span data-stu-id="52466-137">String</span></span>|<span data-ttu-id="52466-138">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="52466-138">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="52466-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="52466-139">Response</span></span>

<span data-ttu-id="52466-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [mailFolder](../resources/mailfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="52466-140">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52466-141">Пример</span><span class="sxs-lookup"><span data-stu-id="52466-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="52466-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="52466-142">Request</span></span>

<span data-ttu-id="52466-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52466-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="52466-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="52466-144">Response</span></span>

<span data-ttu-id="52466-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="52466-145">The following is an example of the response.</span></span>

> <span data-ttu-id="52466-146">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="52466-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52466-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52466-147">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
