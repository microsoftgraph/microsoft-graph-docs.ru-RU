---
title: Обновление teamsApp
description: 'Обновление приложения, ранее опубликованного в каталоге приложений Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ca0bb22bf8be1898c376807a5df2e727f282b30d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472015"
---
# <a name="update-teamsapp"></a><span data-ttu-id="c4849-103">Обновление teamsApp</span><span class="sxs-lookup"><span data-stu-id="c4849-103">Update teamsApp</span></span>

<span data-ttu-id="c4849-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4849-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4849-105">Обновление [приложения,](../resources/teamsapp.md) ранее опубликованного в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c4849-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="c4849-106">Чтобы обновить приложение, необходимо задать свойство **distributionMethod** для `organization` приложения.</span><span class="sxs-lookup"><span data-stu-id="c4849-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="c4849-107">Этот API специально обновляет приложение, опубликованное в каталоге приложений организации (каталоге приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="c4849-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4849-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4849-108">Permissions</span></span>

<span data-ttu-id="c4849-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4849-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="c4849-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c4849-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="c4849-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4849-112">Permission Type</span></span>                        | <span data-ttu-id="c4849-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4849-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="c4849-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4849-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4849-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4849-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c4849-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4849-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4849-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c4849-117">Not supported</span></span>|
| <span data-ttu-id="c4849-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4849-118">Application</span></span>                            | <span data-ttu-id="c4849-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4849-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4849-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4849-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a><span data-ttu-id="c4849-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c4849-121">Query parameters</span></span>

|<span data-ttu-id="c4849-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4849-122">Property</span></span>|<span data-ttu-id="c4849-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c4849-123">Type</span></span>|<span data-ttu-id="c4849-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c4849-124">Description</span></span>|
|----|----|----|
|<span data-ttu-id="c4849-125">requiresReview</span><span class="sxs-lookup"><span data-stu-id="c4849-125">requiresReview</span></span>| <span data-ttu-id="c4849-126">Логический</span><span class="sxs-lookup"><span data-stu-id="c4849-126">Boolean</span></span> | <span data-ttu-id="c4849-127">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="c4849-127">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="c4849-128">Пользователи с привилегиями администратора могут отправлять приложения без запуска проверки.</span><span class="sxs-lookup"><span data-stu-id="c4849-128">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="c4849-129">Если пользователи хотят запросить отзыв перед публикацией, они должны `requiresReview` задать . `true`</span><span class="sxs-lookup"><span data-stu-id="c4849-129">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="c4849-130">Пользователь, у которого есть привилегии администратора, может не устанавливать и не устанавливать значение, и приложение будет считаться утвержденным и будет `requiresReview` `false`  публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="c4849-130">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c4849-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4849-131">Request headers</span></span>

| <span data-ttu-id="c4849-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4849-132">Header</span></span>        | <span data-ttu-id="c4849-133">Значение</span><span class="sxs-lookup"><span data-stu-id="c4849-133">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="c4849-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4849-134">Authorization</span></span> | <span data-ttu-id="c4849-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4849-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c4849-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4849-137">Content-Type</span></span>  | <span data-ttu-id="c4849-138">application/zip.</span><span class="sxs-lookup"><span data-stu-id="c4849-138">application/zip.</span></span> <span data-ttu-id="c4849-139">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c4849-139">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4849-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4849-140">Request body</span></span>

<span data-ttu-id="c4849-141">В теле запроса включите полезной нагрузкой манифест Teams zip.</span><span class="sxs-lookup"><span data-stu-id="c4849-141">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="c4849-142">Дополнительные сведения см. [в материале Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="c4849-142">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="c4849-143">**Примечание:** Используйте ID, возвращенный из вызова опубликованных приложений [Списка,](./appcatalogs-list-teamsapps.md) для ссылки на приложение, которое необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c4849-143">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="c4849-144">Не используйте ID из манифеста пакета почтовых приложений.</span><span class="sxs-lookup"><span data-stu-id="c4849-144">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="c4849-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4849-145">Response</span></span>

<span data-ttu-id="c4849-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c4849-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c4849-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4849-147">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="c4849-148">Пример 1. Обновление приложения, ранее опубликованного в каталоге приложений Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c4849-148">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="c4849-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4849-149">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="c4849-150">Дополнительные сведения о почтовом файле приложения Teams см. в [материале Create app package.](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="c4849-150">For details about the Teams application zip file, see [Create app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c4849-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4849-151">Response</span></span>

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a><span data-ttu-id="c4849-152">Пример 2. Обновление новой версии существующего приложения для проверки администратора до публикации в текущем каталоге клиента</span><span class="sxs-lookup"><span data-stu-id="c4849-152">Example 2: Update a new version of an existing app for admin review prior to publication in the current tenant catalog</span></span>

#### <a name="request"></a><span data-ttu-id="c4849-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4849-153">Request</span></span>

<!-- markdownlint-disable MD034 -->

<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c4849-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4849-154">Response</span></span>

<span data-ttu-id="c4849-155">В случае успешной работы этот метод возвращает код ответа и пару `201 Created` ключей и значений: `publishingState` в `submitted` тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4849-155">If successful, this method returns a `201 Created` response code and the key/value pair `publishingState`: `submitted` in the response body.</span></span> <span data-ttu-id="c4849-156">*См.* [раздел TeamsAppdefinition](../resources/teamsappdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c4849-156">*See* [teamsappdefinition](../resources/teamsappdefinition.md).</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appDefinition",
    "@odata.etag": "158749010",
    "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
    "teamsAppId": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
    "displayName": "Test app",
    "version": "1.0.11",
    "azureADAppId": "a651cc7d-ec54-4fb2-9d0e-2c58dc830b0b",
    "requiredResourceSpecificApplicationPermissions":[
         "ChannelMessage.Read.Group",
         "Channel.Create.Group",
         "Tab.ReadWrite.Group",
         "Member.Read.Group"
    ],
    "publishingState": "submitted",
    "lastModifiedDateTime": "2020-02-10 22:48:33.841",
}
```
