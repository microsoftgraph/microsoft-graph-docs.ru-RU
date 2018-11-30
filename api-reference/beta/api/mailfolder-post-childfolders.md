---
title: Создание mailFolder
description: Используйте этот интерфейс API для создания нового дочернего mailFolder.
ms.openlocfilehash: 44d9e9ebfd721a68734376342500ad1e2a182cda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079199"
---
# <a name="create-mailfolder"></a><span data-ttu-id="a8011-103">Создание mailFolder</span><span class="sxs-lookup"><span data-stu-id="a8011-103">Create mailFolder</span></span>

> <span data-ttu-id="a8011-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8011-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8011-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8011-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8011-106">Используйте этот интерфейс API для создания нового дочернего [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a8011-106">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8011-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8011-107">Permissions</span></span>

<span data-ttu-id="a8011-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8011-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8011-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8011-110">Permission type</span></span> | <span data-ttu-id="a8011-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8011-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="a8011-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8011-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a8011-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8011-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a8011-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8011-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8011-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8011-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a8011-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8011-116">Application</span></span> | <span data-ttu-id="a8011-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8011-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8011-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8011-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="a8011-119">Укажите родительской папки в URL-АДРЕСЕ запроса как идентификатор папки или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="a8011-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="a8011-120">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a8011-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8011-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8011-121">Request headers</span></span>

| <span data-ttu-id="a8011-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8011-122">Header</span></span> | <span data-ttu-id="a8011-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a8011-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="a8011-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8011-124">Authorization</span></span> | <span data-ttu-id="a8011-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="a8011-125"></span></span> <span data-ttu-id="a8011-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="a8011-126">Required.</span></span> |
| <span data-ttu-id="a8011-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8011-127">Content-Type</span></span> | <span data-ttu-id="a8011-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="a8011-128"></span></span> <span data-ttu-id="a8011-129">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="a8011-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8011-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8011-130">Request body</span></span>

<span data-ttu-id="a8011-p106">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a8011-p106">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="a8011-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="a8011-133">Parameter</span></span> | <span data-ttu-id="a8011-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a8011-134">Type</span></span> | <span data-ttu-id="a8011-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a8011-135">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="a8011-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a8011-136">displayName</span></span>|<span data-ttu-id="a8011-137">String</span><span class="sxs-lookup"><span data-stu-id="a8011-137">String</span></span>|<span data-ttu-id="a8011-138">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="a8011-138">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="a8011-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8011-139">Response</span></span>

<span data-ttu-id="a8011-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [mailFolder](../resources/mailfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a8011-140">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8011-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a8011-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a8011-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8011-142">Request</span></span>

<span data-ttu-id="a8011-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8011-143">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="a8011-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8011-144">Response</span></span>

<span data-ttu-id="a8011-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a8011-145">The following is an example of the response.</span></span>

> <span data-ttu-id="a8011-146">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="a8011-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a8011-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8011-147">All the properties will be returned from an actual call.</span></span>
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
