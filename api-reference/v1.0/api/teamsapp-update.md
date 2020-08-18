---
title: Обновление teamsApp
description: 'Обновление приложения, опубликованного ранее в каталоге приложений Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 31f7b40b8f6c1f6de1fcaf6122c4311e5a65d016
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792144"
---
# <a name="update-teamsapp"></a><span data-ttu-id="79f33-103">Обновление teamsApp</span><span class="sxs-lookup"><span data-stu-id="79f33-103">Update teamsApp</span></span>

<span data-ttu-id="79f33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79f33-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79f33-105">Обновление [приложения](../resources/teamsapp.md) , опубликованного ранее в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="79f33-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="79f33-106">Чтобы обновить приложение, свойству **distributionMethod** для приложения необходимо присвоить значение `organization` .</span><span class="sxs-lookup"><span data-stu-id="79f33-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="79f33-107">Этот API-интерфейс специально обновляет приложение, опубликованное в каталоге приложений вашей организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="79f33-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="79f33-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79f33-108">Permissions</span></span>

<span data-ttu-id="79f33-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79f33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="79f33-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="79f33-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="79f33-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79f33-112">Permission Type</span></span>                        | <span data-ttu-id="79f33-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79f33-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="79f33-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79f33-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="79f33-115">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="79f33-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="79f33-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79f33-116">Delegated (work or school account)</span></span> | <span data-ttu-id="79f33-117">CamlQuery. оправить</span><span class="sxs-lookup"><span data-stu-id="79f33-117">AppCatalog.Submit</span></span>|
| <span data-ttu-id="79f33-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79f33-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79f33-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79f33-119">Not supported</span></span>|
| <span data-ttu-id="79f33-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79f33-120">Application</span></span>                            | <span data-ttu-id="79f33-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f33-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79f33-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79f33-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a><span data-ttu-id="79f33-123">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="79f33-123">Query parameters</span></span>

|<span data-ttu-id="79f33-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="79f33-124">Property</span></span>|<span data-ttu-id="79f33-125">Тип</span><span class="sxs-lookup"><span data-stu-id="79f33-125">Type</span></span>|<span data-ttu-id="79f33-126">Описание</span><span class="sxs-lookup"><span data-stu-id="79f33-126">Description</span></span>|
|----|----|----|
|<span data-ttu-id="79f33-127">рекуиресревиев</span><span class="sxs-lookup"><span data-stu-id="79f33-127">requiresReview</span></span>| <span data-ttu-id="79f33-128">Логический</span><span class="sxs-lookup"><span data-stu-id="79f33-128">Boolean</span></span> | <span data-ttu-id="79f33-129">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="79f33-129">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="79f33-130">Пользователи с правами администратора могут отсылать приложения, не запуская проверку.</span><span class="sxs-lookup"><span data-stu-id="79f33-130">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="79f33-131">Если пользователям требуется предварительно запросить проверку перед публикацией, необходимо задать  `requiresReview` для них значение `true` .</span><span class="sxs-lookup"><span data-stu-id="79f33-131">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="79f33-132">Пользователь с правами администратора может не устанавливать `requiresReview` или устанавливать значение `false`  , и приложение считается утвержденным и будет публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="79f33-132">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="79f33-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79f33-133">Request headers</span></span>

| <span data-ttu-id="79f33-134">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79f33-134">Header</span></span>        | <span data-ttu-id="79f33-135">Значение</span><span class="sxs-lookup"><span data-stu-id="79f33-135">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="79f33-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79f33-136">Authorization</span></span> | <span data-ttu-id="79f33-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79f33-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="79f33-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79f33-139">Content-Type</span></span>  | <span data-ttu-id="79f33-140">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="79f33-140">application/zip.</span></span> <span data-ttu-id="79f33-141">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="79f33-141">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79f33-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79f33-142">Request body</span></span>

<span data-ttu-id="79f33-143">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="79f33-143">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="79f33-144">Дополнительные сведения см. [в статье Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="79f33-144">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="79f33-145">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="79f33-145">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="79f33-146">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="79f33-146">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="79f33-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="79f33-147">Response</span></span>

<span data-ttu-id="79f33-148">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79f33-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="79f33-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="79f33-149">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="79f33-150">Пример 1: обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="79f33-150">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="79f33-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="79f33-151">Request</span></span>

<!-- markdownlint-disable MD034 -->
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="79f33-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="79f33-152">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-previously-reviewed-and-published-application-to-the-teams-app-catalog"></a><span data-ttu-id="79f33-153">Пример 2: обновление ранее проверенного и опубликованного приложения в каталоге приложений Teams</span><span class="sxs-lookup"><span data-stu-id="79f33-153">Example 2: Update a previously reviewed and published application to the Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="79f33-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="79f33-154">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="79f33-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="79f33-155">Response</span></span>

<span data-ttu-id="79f33-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и сочетание "ключ-значение" `publishingState` : `submitted` в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79f33-156">If successful, this method returns a `201 Created` response code and the key/value pair `publishingState`: `submitted` in the response body.</span></span> <span data-ttu-id="79f33-157">Дополнительные сведения см. в разделе [теамсаппдефинитион](../resources/teamsappdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="79f33-157">For details, see [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==

{
    "@odata.context": "https://graph.microsoft.com/v1/$metadata#appDefinition",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-08-08 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
