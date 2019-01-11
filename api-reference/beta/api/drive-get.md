---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
localization_priority: Normal
ms.openlocfilehash: d18ee7191747b2c625b62bdecec6d3bffdf0f57e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859660"
---
# <a name="get-drive"></a><span data-ttu-id="c2709-102">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="c2709-102">Get Drive</span></span>

> <span data-ttu-id="c2709-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2709-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2709-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2709-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2709-105">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="c2709-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="c2709-106">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотеки документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c2709-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2709-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2709-107">Permissions</span></span>

<span data-ttu-id="c2709-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2709-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2709-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2709-110">Permission type</span></span>      | <span data-ttu-id="c2709-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2709-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2709-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2709-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c2709-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2709-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2709-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2709-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2709-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2709-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2709-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2709-116">Application</span></span> | <span data-ttu-id="c2709-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2709-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="c2709-118">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="c2709-118">Get current user's OneDrive</span></span>

<span data-ttu-id="c2709-119">Доступ к объекту drive пользователя, вошедшего в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="c2709-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="c2709-120">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен объект drive пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="c2709-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2709-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2709-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="c2709-122">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="c2709-122">Get a user's OneDrive</span></span>

<span data-ttu-id="c2709-123">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="c2709-123">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="c2709-124">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен объект drive пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="c2709-124">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2709-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2709-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="c2709-126">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c2709-126">Path parameters</span></span>

| <span data-ttu-id="c2709-127">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c2709-127">Parameter name</span></span> | <span data-ttu-id="c2709-128">Значение</span><span class="sxs-lookup"><span data-stu-id="c2709-128">Value</span></span>  | <span data-ttu-id="c2709-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c2709-129">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c2709-130">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="c2709-130">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="c2709-131">строка</span><span class="sxs-lookup"><span data-stu-id="c2709-131">string</span></span> | <span data-ttu-id="c2709-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2709-132">Required.</span></span> <span data-ttu-id="c2709-133">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c2709-133">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="c2709-134">Получение библиотеки документов, сопоставленной с группой</span><span class="sxs-lookup"><span data-stu-id="c2709-134">Get the document library associated with a group</span></span>

<span data-ttu-id="c2709-135">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="c2709-135">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2709-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2709-136">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="c2709-137">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c2709-137">Path parameters</span></span>

| <span data-ttu-id="c2709-138">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c2709-138">Parameter name</span></span> | <span data-ttu-id="c2709-139">Значение</span><span class="sxs-lookup"><span data-stu-id="c2709-139">Value</span></span>  | <span data-ttu-id="c2709-140">Описание</span><span class="sxs-lookup"><span data-stu-id="c2709-140">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c2709-141">_groupId_</span><span class="sxs-lookup"><span data-stu-id="c2709-141">_groupId_</span></span>      | <span data-ttu-id="c2709-142">строка</span><span class="sxs-lookup"><span data-stu-id="c2709-142">string</span></span> | <span data-ttu-id="c2709-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2709-143">Required.</span></span> <span data-ttu-id="c2709-144">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="c2709-144">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="c2709-145">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="c2709-145">Get the document library for a site</span></span>

<span data-ttu-id="c2709-146">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="c2709-146">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2709-147">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2709-147">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="c2709-148">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c2709-148">Path parameters</span></span>

| <span data-ttu-id="c2709-149">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c2709-149">Parameter name</span></span> | <span data-ttu-id="c2709-150">Значение</span><span class="sxs-lookup"><span data-stu-id="c2709-150">Value</span></span>  | <span data-ttu-id="c2709-151">Описание</span><span class="sxs-lookup"><span data-stu-id="c2709-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c2709-152">_siteId_</span><span class="sxs-lookup"><span data-stu-id="c2709-152">_siteId_</span></span>       | <span data-ttu-id="c2709-153">строка</span><span class="sxs-lookup"><span data-stu-id="c2709-153">string</span></span> | <span data-ttu-id="c2709-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2709-154">Required.</span></span> <span data-ttu-id="c2709-155">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="c2709-155">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="c2709-156">Получение объекта drive с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="c2709-156">Get a drive by ID</span></span>

<span data-ttu-id="c2709-157">Если у вас есть уникальный идентификатор drive, вы можете получить доступ к этому объекту непосредственно из коллекции объектов drive верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="c2709-157">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2709-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2709-158">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="c2709-159">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c2709-159">Path parameters</span></span>

| <span data-ttu-id="c2709-160">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c2709-160">Parameter name</span></span> | <span data-ttu-id="c2709-161">Значение</span><span class="sxs-lookup"><span data-stu-id="c2709-161">Value</span></span>  | <span data-ttu-id="c2709-162">Описание</span><span class="sxs-lookup"><span data-stu-id="c2709-162">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c2709-163">_driveId_</span><span class="sxs-lookup"><span data-stu-id="c2709-163">_driveId_</span></span>      | <span data-ttu-id="c2709-164">строка</span><span class="sxs-lookup"><span data-stu-id="c2709-164">string</span></span> | <span data-ttu-id="c2709-165">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2709-165">Required.</span></span> <span data-ttu-id="c2709-166">Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="c2709-166">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="c2709-167">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2709-167">Optional query parameters</span></span>

<span data-ttu-id="c2709-168">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования отклика.</span><span class="sxs-lookup"><span data-stu-id="c2709-168">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="c2709-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2709-169">Response</span></span>

<span data-ttu-id="c2709-170">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего объекта drive в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c2709-170">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="c2709-171">Коды откликов с ошибками</span><span class="sxs-lookup"><span data-stu-id="c2709-171">Error response codes</span></span>

<span data-ttu-id="c2709-172">Если объект drive не существует и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен отклик `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="c2709-172">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
