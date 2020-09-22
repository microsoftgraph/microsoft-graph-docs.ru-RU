---
title: Обновление teamsApp
description: 'Обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e47ca7c35ddd535ec9809039cc57c4be670ef85a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076622"
---
# <a name="update-teamsapp"></a><span data-ttu-id="3f96b-103">Обновление teamsApp</span><span class="sxs-lookup"><span data-stu-id="3f96b-103">Update teamsApp</span></span>

<span data-ttu-id="3f96b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f96b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f96b-105">Обновление [приложения](../resources/teamsapp.md) , опубликованного ранее в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3f96b-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="3f96b-106">Чтобы обновить приложение, свойству **distributionMethod** для приложения необходимо присвоить значение `organization` .</span><span class="sxs-lookup"><span data-stu-id="3f96b-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="3f96b-107">Этот API-интерфейс специально обновляет приложение, опубликованное в каталоге приложений вашей организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="3f96b-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>  

## <a name="permissions"></a><span data-ttu-id="3f96b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f96b-108">Permissions</span></span>

<span data-ttu-id="3f96b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="3f96b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="3f96b-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3f96b-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="3f96b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f96b-112">Permission Type</span></span>                        | <span data-ttu-id="3f96b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f96b-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="3f96b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f96b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f96b-115">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3f96b-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3f96b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f96b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3f96b-117">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="3f96b-117">AppCatalog.Submit</span></span>|
| <span data-ttu-id="3f96b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f96b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f96b-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3f96b-119">Not supported</span></span>|
| <span data-ttu-id="3f96b-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f96b-120">Application</span></span>                            | <span data-ttu-id="3f96b-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f96b-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f96b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f96b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a><span data-ttu-id="3f96b-123">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="3f96b-123">Query parameters</span></span>

|<span data-ttu-id="3f96b-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f96b-124">Property</span></span>|<span data-ttu-id="3f96b-125">Тип</span><span class="sxs-lookup"><span data-stu-id="3f96b-125">Type</span></span>|<span data-ttu-id="3f96b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3f96b-126">Description</span></span>|
|----|----|----|
|<span data-ttu-id="3f96b-127">рекуиресревиев</span><span class="sxs-lookup"><span data-stu-id="3f96b-127">requiresReview</span></span>| <span data-ttu-id="3f96b-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f96b-128">Boolean</span></span> | <span data-ttu-id="3f96b-129">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="3f96b-129">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="3f96b-130">Пользователи с правами администратора могут отсылать приложения, не запуская проверку.</span><span class="sxs-lookup"><span data-stu-id="3f96b-130">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="3f96b-131">Если пользователям требуется предварительно запросить проверку перед публикацией, необходимо задать  `requiresReview` для них значение `true` .</span><span class="sxs-lookup"><span data-stu-id="3f96b-131">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="3f96b-132">Пользователь с правами администратора может не устанавливать `requiresReview` или устанавливать значение `false`  , и приложение считается утвержденным и будет публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="3f96b-132">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3f96b-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f96b-133">Request headers</span></span>

| <span data-ttu-id="3f96b-134">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f96b-134">Header</span></span>        | <span data-ttu-id="3f96b-135">Значение</span><span class="sxs-lookup"><span data-stu-id="3f96b-135">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="3f96b-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f96b-136">Authorization</span></span> | <span data-ttu-id="3f96b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f96b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3f96b-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3f96b-139">Content-Type</span></span>  | <span data-ttu-id="3f96b-140">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="3f96b-140">application/zip.</span></span> <span data-ttu-id="3f96b-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3f96b-141">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f96b-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f96b-142">Request body</span></span>

<span data-ttu-id="3f96b-143">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="3f96b-143">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="3f96b-144">Дополнительные сведения см. в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="3f96b-144">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

><span data-ttu-id="3f96b-145">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="3f96b-145">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="3f96b-146">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="3f96b-146">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="3f96b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f96b-147">Response</span></span>

<span data-ttu-id="3f96b-148">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3f96b-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3f96b-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="3f96b-149">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="3f96b-150">Пример 1: обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3f96b-150">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="3f96b-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f96b-151">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="3f96b-152">Подробные сведения о ZIP-файле приложения Teams приведены в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="3f96b-152">For details about the Teams application zip file, see [Create app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="3f96b-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f96b-153">Response</span></span>

<span data-ttu-id="3f96b-154">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3f96b-154">If successful, this method returns a `204 No Content` response code.</span></span>

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a><span data-ttu-id="3f96b-155">Пример 2: обновление новой версии существующего приложения для просмотра администратором до публикации в текущем каталоге клиентов</span><span class="sxs-lookup"><span data-stu-id="3f96b-155">Example 2: Update a new version of an existing app for admin review prior to publication in the current tenant catalog</span></span>

### <a name="request"></a><span data-ttu-id="3f96b-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f96b-156">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="3f96b-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f96b-157">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="3f96b-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f96b-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3f96b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f96b-159">Response</span></span>

<span data-ttu-id="3f96b-160">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и сочетание "ключ-значение" `publishingState` : `submitted` в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f96b-160">If successful, this method returns a `201 Created` response code and the key/value pair `publishingState`: `submitted` in the response body.</span></span> <span data-ttu-id="3f96b-161">*Обратитесь к разделу* [теамсаппдефинитион](../resources/teamsappdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3f96b-161">*See* [teamsappdefinition](../resources/teamsappdefinition.md).</span></span>

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


