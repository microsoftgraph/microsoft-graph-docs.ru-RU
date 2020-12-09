---
title: Обновление teamsApp
description: 'Обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8c2d105a03e8818ab9f8877df9dc84e77ae85964
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606806"
---
# <a name="update-teamsapp"></a><span data-ttu-id="f82a0-103">Обновление teamsApp</span><span class="sxs-lookup"><span data-stu-id="f82a0-103">Update teamsApp</span></span>

<span data-ttu-id="f82a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f82a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f82a0-105">Обновление [приложения](../resources/teamsapp.md) , опубликованного ранее в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f82a0-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="f82a0-106">Чтобы обновить приложение, свойству **distributionMethod** для приложения необходимо присвоить значение `organization` .</span><span class="sxs-lookup"><span data-stu-id="f82a0-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="f82a0-107">Этот API-интерфейс специально обновляет приложение, опубликованное в каталоге приложений вашей организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="f82a0-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>  

## <a name="permissions"></a><span data-ttu-id="f82a0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f82a0-108">Permissions</span></span>

<span data-ttu-id="f82a0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f82a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f82a0-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f82a0-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="f82a0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f82a0-112">Permission Type</span></span>                        | <span data-ttu-id="f82a0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f82a0-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="f82a0-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f82a0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f82a0-115">CamlQuery. оправить, CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f82a0-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="f82a0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f82a0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f82a0-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f82a0-117">Not supported</span></span>|
| <span data-ttu-id="f82a0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f82a0-118">Application</span></span>                            | <span data-ttu-id="f82a0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f82a0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f82a0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f82a0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a><span data-ttu-id="f82a0-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f82a0-121">Query parameters</span></span>

|<span data-ttu-id="f82a0-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="f82a0-122">Property</span></span>|<span data-ttu-id="f82a0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f82a0-123">Type</span></span>|<span data-ttu-id="f82a0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f82a0-124">Description</span></span>|
|----|----|----|
|<span data-ttu-id="f82a0-125">рекуиресревиев</span><span class="sxs-lookup"><span data-stu-id="f82a0-125">requiresReview</span></span>| <span data-ttu-id="f82a0-126">Логический</span><span class="sxs-lookup"><span data-stu-id="f82a0-126">Boolean</span></span> | <span data-ttu-id="f82a0-127">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="f82a0-127">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="f82a0-128">Пользователи с правами администратора могут отсылать приложения, не запуская проверку.</span><span class="sxs-lookup"><span data-stu-id="f82a0-128">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="f82a0-129">Если пользователям требуется предварительно запросить проверку перед публикацией, необходимо задать  `requiresReview` для них значение `true` .</span><span class="sxs-lookup"><span data-stu-id="f82a0-129">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="f82a0-130">Пользователь с правами администратора может не устанавливать `requiresReview` или устанавливать значение `false`  , и приложение считается утвержденным и будет публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="f82a0-130">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f82a0-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f82a0-131">Request headers</span></span>

| <span data-ttu-id="f82a0-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f82a0-132">Header</span></span>        | <span data-ttu-id="f82a0-133">Значение</span><span class="sxs-lookup"><span data-stu-id="f82a0-133">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="f82a0-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f82a0-134">Authorization</span></span> | <span data-ttu-id="f82a0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f82a0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f82a0-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f82a0-137">Content-Type</span></span>  | <span data-ttu-id="f82a0-138">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="f82a0-138">application/zip.</span></span> <span data-ttu-id="f82a0-139">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f82a0-139">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f82a0-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f82a0-140">Request body</span></span>

<span data-ttu-id="f82a0-141">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="f82a0-141">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="f82a0-142">Дополнительные сведения см. в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f82a0-142">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

><span data-ttu-id="f82a0-143">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./appcatalogs-list-teamsapps.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="f82a0-143">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="f82a0-144">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="f82a0-144">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="f82a0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f82a0-145">Response</span></span>

<span data-ttu-id="f82a0-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f82a0-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f82a0-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="f82a0-147">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="f82a0-148">Пример 1: обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f82a0-148">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="f82a0-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f82a0-149">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="f82a0-150">Подробные сведения о ZIP-файле приложения Teams приведены в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f82a0-150">For details about the Teams application zip file, see [Create app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="f82a0-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="f82a0-151">Response</span></span>

<span data-ttu-id="f82a0-152">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f82a0-152">If successful, this method returns a `204 No Content` response code.</span></span>

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a><span data-ttu-id="f82a0-153">Пример 2: обновление новой версии существующего приложения для просмотра администратором до публикации в текущем каталоге клиентов</span><span class="sxs-lookup"><span data-stu-id="f82a0-153">Example 2: Update a new version of an existing app for admin review prior to publication in the current tenant catalog</span></span>

### <a name="request"></a><span data-ttu-id="f82a0-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="f82a0-154">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="f82a0-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="f82a0-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="javascript"></a>[<span data-ttu-id="f82a0-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f82a0-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f82a0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="f82a0-157">Response</span></span>

<span data-ttu-id="f82a0-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и сочетание "ключ-значение" `publishingState` : `submitted` в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f82a0-158">If successful, this method returns a `201 Created` response code and the key/value pair `publishingState`: `submitted` in the response body.</span></span> <span data-ttu-id="f82a0-159">*Обратитесь к разделу* [теамсаппдефинитион](../resources/teamsappdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f82a0-159">*See* [teamsappdefinition](../resources/teamsappdefinition.md).</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appDefinition",
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
