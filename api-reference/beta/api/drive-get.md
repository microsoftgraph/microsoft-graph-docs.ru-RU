---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b481a99232a040334fbfbbaf7d8ef65bd12261e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976130"
---
# <a name="get-drive"></a><span data-ttu-id="d7a64-102">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="d7a64-102">Get Drive</span></span>

> <span data-ttu-id="d7a64-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7a64-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7a64-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7a64-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7a64-105">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="d7a64-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="d7a64-106">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотеки документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d7a64-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7a64-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7a64-107">Permissions</span></span>

<span data-ttu-id="d7a64-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7a64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7a64-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7a64-110">Permission type</span></span>      | <span data-ttu-id="d7a64-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7a64-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7a64-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7a64-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7a64-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7a64-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7a64-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7a64-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7a64-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7a64-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7a64-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7a64-116">Application</span></span> | <span data-ttu-id="d7a64-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7a64-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="d7a64-118">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="d7a64-118">Get current user's OneDrive</span></span>

<span data-ttu-id="d7a64-119">Доступ к объекту drive пользователя, вошедшего в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="d7a64-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="d7a64-120">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен объект drive пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="d7a64-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="d7a64-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7a64-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="d7a64-122">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="d7a64-122">Get a user's OneDrive</span></span>

<span data-ttu-id="d7a64-123">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="d7a64-123">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="d7a64-124">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен объект drive пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="d7a64-124">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="d7a64-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7a64-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="d7a64-126">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="d7a64-126">Path parameters</span></span>

| <span data-ttu-id="d7a64-127">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="d7a64-127">Parameter name</span></span> | <span data-ttu-id="d7a64-128">Значение</span><span class="sxs-lookup"><span data-stu-id="d7a64-128">Value</span></span>  | <span data-ttu-id="d7a64-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d7a64-129">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d7a64-130">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="d7a64-130">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="d7a64-131">строка</span><span class="sxs-lookup"><span data-stu-id="d7a64-131">string</span></span> | <span data-ttu-id="d7a64-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7a64-132">Required.</span></span> <span data-ttu-id="d7a64-133">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d7a64-133">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="d7a64-134">Получение библиотеки документов, сопоставленной с группой</span><span class="sxs-lookup"><span data-stu-id="d7a64-134">Get the document library associated with a group</span></span>

<span data-ttu-id="d7a64-135">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="d7a64-135">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="d7a64-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7a64-136">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="d7a64-137">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="d7a64-137">Path parameters</span></span>

| <span data-ttu-id="d7a64-138">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="d7a64-138">Parameter name</span></span> | <span data-ttu-id="d7a64-139">Значение</span><span class="sxs-lookup"><span data-stu-id="d7a64-139">Value</span></span>  | <span data-ttu-id="d7a64-140">Описание</span><span class="sxs-lookup"><span data-stu-id="d7a64-140">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d7a64-141">_groupId_</span><span class="sxs-lookup"><span data-stu-id="d7a64-141">_groupId_</span></span>      | <span data-ttu-id="d7a64-142">строка</span><span class="sxs-lookup"><span data-stu-id="d7a64-142">string</span></span> | <span data-ttu-id="d7a64-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7a64-143">Required.</span></span> <span data-ttu-id="d7a64-144">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="d7a64-144">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="d7a64-145">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="d7a64-145">Get the document library for a site</span></span>

<span data-ttu-id="d7a64-146">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="d7a64-146">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="d7a64-147">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7a64-147">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="d7a64-148">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="d7a64-148">Path parameters</span></span>

| <span data-ttu-id="d7a64-149">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="d7a64-149">Parameter name</span></span> | <span data-ttu-id="d7a64-150">Значение</span><span class="sxs-lookup"><span data-stu-id="d7a64-150">Value</span></span>  | <span data-ttu-id="d7a64-151">Описание</span><span class="sxs-lookup"><span data-stu-id="d7a64-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d7a64-152">_siteId_</span><span class="sxs-lookup"><span data-stu-id="d7a64-152">_siteId_</span></span>       | <span data-ttu-id="d7a64-153">строка</span><span class="sxs-lookup"><span data-stu-id="d7a64-153">string</span></span> | <span data-ttu-id="d7a64-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7a64-154">Required.</span></span> <span data-ttu-id="d7a64-155">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="d7a64-155">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="d7a64-156">Получение объекта drive с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="d7a64-156">Get a drive by ID</span></span>

<span data-ttu-id="d7a64-157">Если у вас есть уникальный идентификатор drive, вы можете получить доступ к этому объекту непосредственно из коллекции объектов drive верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="d7a64-157">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="d7a64-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7a64-158">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="d7a64-159">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="d7a64-159">Path parameters</span></span>

| <span data-ttu-id="d7a64-160">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="d7a64-160">Parameter name</span></span> | <span data-ttu-id="d7a64-161">Значение</span><span class="sxs-lookup"><span data-stu-id="d7a64-161">Value</span></span>  | <span data-ttu-id="d7a64-162">Описание</span><span class="sxs-lookup"><span data-stu-id="d7a64-162">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d7a64-163">_driveId_</span><span class="sxs-lookup"><span data-stu-id="d7a64-163">_driveId_</span></span>      | <span data-ttu-id="d7a64-164">строка</span><span class="sxs-lookup"><span data-stu-id="d7a64-164">string</span></span> | <span data-ttu-id="d7a64-165">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7a64-165">Required.</span></span> <span data-ttu-id="d7a64-166">Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="d7a64-166">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="d7a64-167">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7a64-167">Optional query parameters</span></span>

<span data-ttu-id="d7a64-168">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования отклика.</span><span class="sxs-lookup"><span data-stu-id="d7a64-168">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="d7a64-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7a64-169">Response</span></span>

<span data-ttu-id="d7a64-170">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего объекта drive в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7a64-170">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a><span data-ttu-id="d7a64-171">Коды откликов с ошибками</span><span class="sxs-lookup"><span data-stu-id="d7a64-171">Error response codes</span></span>

<span data-ttu-id="d7a64-172">Если объект drive не существует и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен отклик `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="d7a64-172">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
