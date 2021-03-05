---
title: Публикация teamsapp
description: 'Публикация приложения в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1984ed7226da71ba1baf1bf15a7d83df4e6609a0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471651"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="af635-103">Публикация teamsapp</span><span class="sxs-lookup"><span data-stu-id="af635-103">Publish teamsapp</span></span>

<span data-ttu-id="af635-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af635-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af635-105">Публикация приложения [в](../resources/teamsapp.md) каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="af635-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="af635-106">В частности, этот API публикует приложение в каталог организации (каталог приложений клиента); созданный ресурс будет иметь **значение свойства distributionMethod** `organization` в .</span><span class="sxs-lookup"><span data-stu-id="af635-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

<span data-ttu-id="af635-107">Свойство **requiresReview** позволяет любому пользователю отправлять приложение для проверки администратором.</span><span class="sxs-lookup"><span data-stu-id="af635-107">The **requiresReview** property allows any user to submit an app for review by an administrator.</span></span> <span data-ttu-id="af635-108">Администраторы могут утверждать или отклонить эти приложения с помощью этого API или центра администрирования Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="af635-108">Admins can approve or reject these apps via this API or the Microsoft Teams admin center.</span></span>

## <a name="permissions"></a><span data-ttu-id="af635-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af635-109">Permissions</span></span>

<span data-ttu-id="af635-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af635-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="af635-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af635-112">Permission Type</span></span>                        | <span data-ttu-id="af635-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af635-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="af635-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af635-114">Delegated (work or school account)</span></span> | <span data-ttu-id="af635-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af635-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="af635-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af635-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af635-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af635-117">Not supported</span></span>|
| <span data-ttu-id="af635-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af635-118">Application</span></span>                            | <span data-ttu-id="af635-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af635-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af635-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af635-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="af635-121">Публикация приложения, требуемая для проверки:</span><span class="sxs-lookup"><span data-stu-id="af635-121">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="af635-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="af635-122">Query parameters</span></span>

|<span data-ttu-id="af635-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="af635-123">Property</span></span>|<span data-ttu-id="af635-124">Тип</span><span class="sxs-lookup"><span data-stu-id="af635-124">Type</span></span>|<span data-ttu-id="af635-125">Описание</span><span class="sxs-lookup"><span data-stu-id="af635-125">Description</span></span>|
|----|----|----|
|<span data-ttu-id="af635-126">requiresReview</span><span class="sxs-lookup"><span data-stu-id="af635-126">requiresReview</span></span>| <span data-ttu-id="af635-127">Логический</span><span class="sxs-lookup"><span data-stu-id="af635-127">Boolean</span></span> | <span data-ttu-id="af635-128">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="af635-128">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="af635-129">Пользователи с привилегиями администратора могут отправлять приложения без запуска проверки.</span><span class="sxs-lookup"><span data-stu-id="af635-129">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="af635-130">Если пользователи хотят запросить отзыв перед публикацией, они должны `requiresReview` задать . `true`</span><span class="sxs-lookup"><span data-stu-id="af635-130">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="af635-131">Пользователь, у которого есть привилегии администратора, может не устанавливать и не устанавливать значение, и приложение будет считаться утвержденным и будет `requiresReview` `false`  публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="af635-131">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="af635-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af635-132">Request headers</span></span>

| <span data-ttu-id="af635-133">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af635-133">Header</span></span>        | <span data-ttu-id="af635-134">Значение</span><span class="sxs-lookup"><span data-stu-id="af635-134">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="af635-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af635-135">Authorization</span></span> | <span data-ttu-id="af635-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af635-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af635-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af635-138">Content-Type</span></span>  | <span data-ttu-id="af635-139">application/zip.</span><span class="sxs-lookup"><span data-stu-id="af635-139">application/zip.</span></span> <span data-ttu-id="af635-140">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="af635-140">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af635-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af635-141">Request body</span></span>

<span data-ttu-id="af635-142">В теле запроса включите полезной нагрузкой манифест Teams zip.</span><span class="sxs-lookup"><span data-stu-id="af635-142">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="af635-143">Дополнительные сведения см. [в материале Create an app package.](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="af635-143">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="af635-144">Каждое приложение в каталоге приложений должно иметь уникальный ID манифеста.</span><span class="sxs-lookup"><span data-stu-id="af635-144">Each app in the app catalog must have a unique manifest ID.</span></span>

## <a name="response"></a><span data-ttu-id="af635-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="af635-145">Response</span></span>

<span data-ttu-id="af635-146">В случае успешной работы этот метод возвращает код `200 OK` ответа и [объект teamsApp.](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="af635-146">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="af635-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="af635-147">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="af635-148">Пример 1. Публикация приложения в каталоге приложений</span><span class="sxs-lookup"><span data-stu-id="af635-148">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="af635-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="af635-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

---
<span data-ttu-id="af635-150">Сведения о создании почтового файла приложения Microsoft Teams см. в статью [Создание пакета приложений.](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="af635-150">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="af635-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="af635-151">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="af635-152">Пример 2. Отправка нового приложения для проверки в каталог приложений организации</span><span class="sxs-lookup"><span data-stu-id="af635-152">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="af635-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="af635-153">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

---

#### <a name="response"></a><span data-ttu-id="af635-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="af635-154">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps/$entity",
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-3-approve-or-reject-an-app-pending-review"></a><span data-ttu-id="af635-155">Пример 3. Утверждение или отклонение приложения до рассмотрения</span><span class="sxs-lookup"><span data-stu-id="af635-155">Example 3: Approve or reject an app pending review</span></span>

#### <a name="request"></a><span data-ttu-id="af635-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="af635-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/a761ad07-22ef-4a53-9feb-2837c8ad4a84/appDefinitions/YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjU3VibWl0dGVk
Content-type: application/json
If-Match: InFtSStsNVJHVWdzWUJRU2ZVWGp4RWc9PSI=

{
  "publishingState":"published"
}
```

---

#### <a name="response"></a><span data-ttu-id="af635-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="af635-157">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps('a761ad07-22ef-4a53-9feb-2837c8ad4a84')/appDefinitions/$entity",
    "id": "YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjUHVibGlzaGVk",
    "teamsAppId": "a761ad07-22ef-4a53-9feb-2837c8ad4a84",
    "azureADAppId": null,
    "displayName": "Ducks",
    "version": "1.1.8",
    "requiredResourceSpecificApplicationPermissions": [],
    "publishingState": "published",
    "shortDescription": "quaerat quasi magnam. slight change. 5",
    "description": "Aliquid placeat animi debitis accusamus. Non perferendis ullam. Quis est consequuntur vitae provident. Sunt laudantium id aut. slight change 5",
    "lastModifiedDateTime": null,
    "createdBy": null
}
```