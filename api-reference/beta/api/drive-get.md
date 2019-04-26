---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 78e642d189de09677c682607e9f83d7ea9bc482d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325419"
---
# <a name="get-drive"></a><span data-ttu-id="e932f-102">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="e932f-102">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e932f-103">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="e932f-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="e932f-104">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e932f-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="e932f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e932f-105">Permissions</span></span>

<span data-ttu-id="e932f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e932f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e932f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e932f-108">Permission type</span></span>      | <span data-ttu-id="e932f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e932f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e932f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e932f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e932f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e932f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e932f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e932f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e932f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e932f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e932f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e932f-114">Application</span></span> | <span data-ttu-id="e932f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e932f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="e932f-116">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="e932f-116">Get current user's OneDrive</span></span>

<span data-ttu-id="e932f-117">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="e932f-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="e932f-118">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="e932f-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="e932f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e932f-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="e932f-120">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="e932f-120">Get a user's OneDrive</span></span>

<span data-ttu-id="e932f-121">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="e932f-121">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="e932f-122">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="e932f-122">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="e932f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e932f-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="e932f-124">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e932f-124">Path parameters</span></span>

| <span data-ttu-id="e932f-125">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e932f-125">Parameter name</span></span> | <span data-ttu-id="e932f-126">Значение</span><span class="sxs-lookup"><span data-stu-id="e932f-126">Value</span></span>  | <span data-ttu-id="e932f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e932f-127">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e932f-128">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="e932f-128">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="e932f-129">строка</span><span class="sxs-lookup"><span data-stu-id="e932f-129">string</span></span> | <span data-ttu-id="e932f-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e932f-130">Required.</span></span> <span data-ttu-id="e932f-131">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e932f-131">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="e932f-132">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="e932f-132">Get the document library associated with a group</span></span>

<span data-ttu-id="e932f-133">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="e932f-133">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="e932f-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e932f-134">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="e932f-135">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e932f-135">Path parameters</span></span>

| <span data-ttu-id="e932f-136">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e932f-136">Parameter name</span></span> | <span data-ttu-id="e932f-137">Значение</span><span class="sxs-lookup"><span data-stu-id="e932f-137">Value</span></span>  | <span data-ttu-id="e932f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e932f-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e932f-139">_groupId_</span><span class="sxs-lookup"><span data-stu-id="e932f-139">_groupId_</span></span>      | <span data-ttu-id="e932f-140">строка</span><span class="sxs-lookup"><span data-stu-id="e932f-140">string</span></span> | <span data-ttu-id="e932f-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e932f-141">Required.</span></span> <span data-ttu-id="e932f-142">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="e932f-142">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="e932f-143">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="e932f-143">Get the document library for a site</span></span>

<span data-ttu-id="e932f-144">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="e932f-144">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="e932f-145">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e932f-145">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="e932f-146">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e932f-146">Path parameters</span></span>

| <span data-ttu-id="e932f-147">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e932f-147">Parameter name</span></span> | <span data-ttu-id="e932f-148">Значение</span><span class="sxs-lookup"><span data-stu-id="e932f-148">Value</span></span>  | <span data-ttu-id="e932f-149">Описание</span><span class="sxs-lookup"><span data-stu-id="e932f-149">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e932f-150">_siteId_</span><span class="sxs-lookup"><span data-stu-id="e932f-150">_siteId_</span></span>       | <span data-ttu-id="e932f-151">строка</span><span class="sxs-lookup"><span data-stu-id="e932f-151">string</span></span> | <span data-ttu-id="e932f-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e932f-152">Required.</span></span> <span data-ttu-id="e932f-153">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="e932f-153">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="e932f-154">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="e932f-154">Get a drive by ID</span></span>

<span data-ttu-id="e932f-155">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="e932f-155">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="e932f-156">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e932f-156">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="e932f-157">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e932f-157">Path parameters</span></span>

| <span data-ttu-id="e932f-158">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e932f-158">Parameter name</span></span> | <span data-ttu-id="e932f-159">Значение</span><span class="sxs-lookup"><span data-stu-id="e932f-159">Value</span></span>  | <span data-ttu-id="e932f-160">Описание</span><span class="sxs-lookup"><span data-stu-id="e932f-160">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e932f-161">_driveId_</span><span class="sxs-lookup"><span data-stu-id="e932f-161">_driveId_</span></span>      | <span data-ttu-id="e932f-162">string</span><span class="sxs-lookup"><span data-stu-id="e932f-162">string</span></span> | <span data-ttu-id="e932f-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="e932f-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e932f-165">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e932f-165">Optional query parameters</span></span>

<span data-ttu-id="e932f-166">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="e932f-166">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="e932f-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e932f-167">Response</span></span>

<span data-ttu-id="e932f-168">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e932f-168">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="e932f-169">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="e932f-169">Error response codes</span></span>

<span data-ttu-id="e932f-170">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="e932f-170">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive",
  "suppressions": []
}
-->
