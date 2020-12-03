---
title: Публикация teamsapp
description: Опубликуйте приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7694f51ff8f42f27e58fca04ec0ae87ad74e526e
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563480"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="3ea79-103">Публикация teamsApp</span><span class="sxs-lookup"><span data-stu-id="3ea79-103">Publish teamsApp</span></span>

<span data-ttu-id="3ea79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ea79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ea79-105">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3ea79-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="3ea79-106">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь значение свойства **distributionMethod** `organization` .</span><span class="sxs-lookup"><span data-stu-id="3ea79-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

<span data-ttu-id="3ea79-107">Свойство **рекуиресревиев** позволяет любому пользователю передавать приложение для просмотра администратором.</span><span class="sxs-lookup"><span data-stu-id="3ea79-107">The **requiresReview** property allows any user to submit an app for review by an administrator.</span></span> <span data-ttu-id="3ea79-108">Администраторы могут утверждать или отклонять эти приложения через этот API или центр администрирования Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3ea79-108">Admins can approve or reject these apps via this API or the Microsoft Teams admin center.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ea79-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea79-109">Permissions</span></span>

<span data-ttu-id="3ea79-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ea79-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ea79-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea79-112">Permission Type</span></span>                        | <span data-ttu-id="3ea79-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ea79-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="3ea79-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ea79-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3ea79-115">CamlQuery. оправить, CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3ea79-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3ea79-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ea79-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ea79-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3ea79-117">Not supported</span></span>|
| <span data-ttu-id="3ea79-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ea79-118">Application</span></span>                            | <span data-ttu-id="3ea79-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ea79-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ea79-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ea79-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="3ea79-121">Чтобы опубликовать приложение, для которого требуется проверка, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="3ea79-121">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="3ea79-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="3ea79-122">Query parameters</span></span>

|<span data-ttu-id="3ea79-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ea79-123">Property</span></span>|<span data-ttu-id="3ea79-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3ea79-124">Type</span></span>|<span data-ttu-id="3ea79-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3ea79-125">Description</span></span>|
|----|----|----|
|<span data-ttu-id="3ea79-126">рекуиресревиев</span><span class="sxs-lookup"><span data-stu-id="3ea79-126">requiresReview</span></span>| <span data-ttu-id="3ea79-127">Логический</span><span class="sxs-lookup"><span data-stu-id="3ea79-127">Boolean</span></span> | <span data-ttu-id="3ea79-128">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="3ea79-128">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="3ea79-129">Пользователи с правами администратора могут отсылать приложения, не запуская проверку.</span><span class="sxs-lookup"><span data-stu-id="3ea79-129">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="3ea79-130">Если пользователям требуется предварительно запросить проверку перед публикацией, необходимо задать  `requiresReview` для них значение `true` .</span><span class="sxs-lookup"><span data-stu-id="3ea79-130">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="3ea79-131">Пользователь с правами администратора может не устанавливать `requiresReview` или устанавливать значение `false`  , и приложение считается утвержденным и будет публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="3ea79-131">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3ea79-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ea79-132">Request headers</span></span>

| <span data-ttu-id="3ea79-133">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ea79-133">Header</span></span>        | <span data-ttu-id="3ea79-134">Значение</span><span class="sxs-lookup"><span data-stu-id="3ea79-134">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="3ea79-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ea79-135">Authorization</span></span> | <span data-ttu-id="3ea79-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ea79-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3ea79-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ea79-138">Content-Type</span></span>  | <span data-ttu-id="3ea79-139">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="3ea79-139">application/zip.</span></span> <span data-ttu-id="3ea79-140">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3ea79-140">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ea79-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ea79-141">Request body</span></span>

<span data-ttu-id="3ea79-142">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="3ea79-142">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="3ea79-143">Дополнительные сведения см. в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="3ea79-143">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>  

<span data-ttu-id="3ea79-144">Каждое приложение в каталоге приложений должно иметь уникальный манифест `id` .</span><span class="sxs-lookup"><span data-stu-id="3ea79-144">Each app in the app catalog must have a unique manifest `id`.</span></span>

## <a name="response"></a><span data-ttu-id="3ea79-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea79-145">Response</span></span>

<span data-ttu-id="3ea79-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3ea79-146">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="3ea79-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="3ea79-147">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="3ea79-148">Пример 1: Публикация приложения в каталоге приложений</span><span class="sxs-lookup"><span data-stu-id="3ea79-148">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="3ea79-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea79-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3ea79-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ea79-150">HTTP</span></span>](#tab/http)
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

# <a name="javascript"></a>[<span data-ttu-id="3ea79-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ea79-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ea79-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ea79-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3ea79-153">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="3ea79-153">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="3ea79-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea79-154">Response</span></span>

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

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="3ea79-155">Пример 2: Отправка нового приложения для проверки в каталог приложений Организации</span><span class="sxs-lookup"><span data-stu-id="3ea79-155">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="3ea79-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea79-156">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3ea79-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ea79-157">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

# <a name="javascript"></a>[<span data-ttu-id="3ea79-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ea79-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ea79-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ea79-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3ea79-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea79-160">Response</span></span>

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

### <a name="example-3-approve-or-reject-an-app-pending-review"></a><span data-ttu-id="3ea79-161">Пример 3: утверждение или отклонение ожидающей проверки приложения</span><span class="sxs-lookup"><span data-stu-id="3ea79-161">Example 3: Approve or reject an app pending review</span></span>

#### <a name="request"></a><span data-ttu-id="3ea79-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea79-162">Request</span></span>

<span data-ttu-id="3ea79-163">**HTTP**</span><span class="sxs-lookup"><span data-stu-id="3ea79-163">**HTTP**</span></span>
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
PATCH https://graph.microsoft.com/beta/appCatalogs/teamsApps/a761ad07-22ef-4a53-9feb-2837c8ad4a84/appDefinitions/YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjU3VibWl0dGVk
Content-type: application/json
If-Match: InFtSStsNVJHVWdzWUJRU2ZVWGp4RWc9PSI=

{
   "Body":{
      "publishingState":"published"
   }
}
```

---

#### <a name="response"></a><span data-ttu-id="3ea79-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea79-164">Response</span></span>

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
