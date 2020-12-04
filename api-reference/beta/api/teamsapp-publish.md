---
title: Публикация teamsapp
description: Опубликуйте приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9e8579bb2da482e18d2524c82bee985b9eb8ae39
ms.sourcegitcommit: c419bb8901b7766af193196f80bc1d497643fcb2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49572186"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="7f4a2-103">Публикация teamsApp</span><span class="sxs-lookup"><span data-stu-id="7f4a2-103">Publish teamsApp</span></span>

<span data-ttu-id="7f4a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f4a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f4a2-105">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="7f4a2-106">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь значение свойства **distributionMethod** `organization` .</span><span class="sxs-lookup"><span data-stu-id="7f4a2-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

<span data-ttu-id="7f4a2-107">Свойство **рекуиресревиев** позволяет любому пользователю передавать приложение для просмотра администратором.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-107">The **requiresReview** property allows any user to submit an app for review by an administrator.</span></span> <span data-ttu-id="7f4a2-108">Администраторы могут утверждать или отклонять эти приложения через этот API или центр администрирования Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-108">Admins can approve or reject these apps via this API or the Microsoft Teams admin center.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f4a2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f4a2-109">Permissions</span></span>

<span data-ttu-id="7f4a2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f4a2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f4a2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f4a2-112">Permission Type</span></span>                        | <span data-ttu-id="7f4a2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f4a2-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="7f4a2-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f4a2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7f4a2-115">CamlQuery. оправить, CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7f4a2-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="7f4a2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f4a2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f4a2-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7f4a2-117">Not supported</span></span>|
| <span data-ttu-id="7f4a2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f4a2-118">Application</span></span>                            | <span data-ttu-id="7f4a2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f4a2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f4a2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="7f4a2-121">Чтобы опубликовать приложение, для которого требуется проверка, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="7f4a2-121">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="7f4a2-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="7f4a2-122">Query parameters</span></span>

|<span data-ttu-id="7f4a2-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f4a2-123">Property</span></span>|<span data-ttu-id="7f4a2-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7f4a2-124">Type</span></span>|<span data-ttu-id="7f4a2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7f4a2-125">Description</span></span>|
|----|----|----|
|<span data-ttu-id="7f4a2-126">рекуиресревиев</span><span class="sxs-lookup"><span data-stu-id="7f4a2-126">requiresReview</span></span>| <span data-ttu-id="7f4a2-127">Логический</span><span class="sxs-lookup"><span data-stu-id="7f4a2-127">Boolean</span></span> | <span data-ttu-id="7f4a2-128">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-128">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="7f4a2-129">Пользователи с правами администратора могут отсылать приложения, не запуская проверку.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-129">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="7f4a2-130">Если пользователям требуется предварительно запросить проверку перед публикацией, необходимо задать  `requiresReview` для них значение `true` .</span><span class="sxs-lookup"><span data-stu-id="7f4a2-130">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="7f4a2-131">Пользователь с правами администратора может не устанавливать `requiresReview` или устанавливать значение `false`  , и приложение считается утвержденным и будет публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-131">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7f4a2-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f4a2-132">Request headers</span></span>

| <span data-ttu-id="7f4a2-133">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f4a2-133">Header</span></span>        | <span data-ttu-id="7f4a2-134">Значение</span><span class="sxs-lookup"><span data-stu-id="7f4a2-134">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="7f4a2-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f4a2-135">Authorization</span></span> | <span data-ttu-id="7f4a2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7f4a2-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f4a2-138">Content-Type</span></span>  | <span data-ttu-id="7f4a2-139">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-139">application/zip.</span></span> <span data-ttu-id="7f4a2-140">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-140">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f4a2-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f4a2-141">Request body</span></span>

<span data-ttu-id="7f4a2-142">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="7f4a2-142">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="7f4a2-143">Дополнительные сведения см. в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="7f4a2-143">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>  

<span data-ttu-id="7f4a2-144">Каждое приложение в каталоге приложений должно иметь уникальный манифест `id` .</span><span class="sxs-lookup"><span data-stu-id="7f4a2-144">Each app in the app catalog must have a unique manifest `id`.</span></span>

## <a name="response"></a><span data-ttu-id="7f4a2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f4a2-145">Response</span></span>

<span data-ttu-id="7f4a2-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7f4a2-146">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="7f4a2-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="7f4a2-147">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="7f4a2-148">Пример 1: Публикация приложения в каталоге приложений</span><span class="sxs-lookup"><span data-stu-id="7f4a2-148">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="7f4a2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f4a2-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7f4a2-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f4a2-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

# <a name="javascript"></a>[<span data-ttu-id="7f4a2-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f4a2-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f4a2-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f4a2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7f4a2-153">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="7f4a2-153">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="7f4a2-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f4a2-154">Response</span></span>

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

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="7f4a2-155">Пример 2: Отправка нового приложения для проверки в каталог приложений Организации</span><span class="sxs-lookup"><span data-stu-id="7f4a2-155">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="7f4a2-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f4a2-156">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7f4a2-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f4a2-157">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

# <a name="javascript"></a>[<span data-ttu-id="7f4a2-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f4a2-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f4a2-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f4a2-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7f4a2-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f4a2-160">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps/$entity",
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-3-approve-or-reject-an-app-pending-review"></a><span data-ttu-id="7f4a2-161">Пример 3: утверждение или отклонение ожидающей проверки приложения</span><span class="sxs-lookup"><span data-stu-id="7f4a2-161">Example 3: Approve or reject an app pending review</span></span>

#### <a name="request"></a><span data-ttu-id="7f4a2-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f4a2-162">Request</span></span>

<span data-ttu-id="7f4a2-163">**HTTP**</span><span class="sxs-lookup"><span data-stu-id="7f4a2-163">**HTTP**</span></span>
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
PATCH https://graph.microsoft.com/beta/appCatalogs/teamsApps/a761ad07-22ef-4a53-9feb-2837c8ad4a84/appDefinitions/YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjU3VibWl0dGVk
Content-type: application/json
If-Match: InFtSStsNVJHVWdzWUJRU2ZVWGp4RWc9PSI=

{
  "publishingState":"published"
}
```

---

#### <a name="response"></a><span data-ttu-id="7f4a2-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f4a2-164">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('a761ad07-22ef-4a53-9feb-2837c8ad4a84')/appDefinitions/$entity",
    "id": "YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjUHVibGlzaGVk",
    "teamsAppId": "a761ad07-22ef-4a53-9feb-2837c8ad4a84",
    "azureADAppId": null,
    "displayName": "Ducks",
    "version": "1.1.8",
    "requiredResourceSpecificApplicationPermissions": [],
    "publishingState": "published",
    "shortdescription": "quaerat quasi magnam. slight change. 5",
    "description": "Aliquid placeat animi debitis accusamus. Non perferendis ullam. Quis est consequuntur vitae provident. Sunt laudantium id aut. slight change 5",
    "lastModifiedDateTime": null,
    "createdBy": null
}
```
