---
title: Публикация teamsapp
description: Опубликуйте приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 78ff984bfec1e72a5fd480a9dd61d268beea7689
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993985"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="636e6-103">Публикация teamsApp</span><span class="sxs-lookup"><span data-stu-id="636e6-103">Publish teamsApp</span></span>

<span data-ttu-id="636e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="636e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="636e6-105">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="636e6-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="636e6-106">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь значение свойства **distributionMethod** `organization` .</span><span class="sxs-lookup"><span data-stu-id="636e6-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="636e6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="636e6-107">Permissions</span></span>

<span data-ttu-id="636e6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="636e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="636e6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="636e6-110">Permission Type</span></span>                        | <span data-ttu-id="636e6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="636e6-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="636e6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="636e6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="636e6-113">CamlQuery. оправить, CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="636e6-113">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="636e6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="636e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="636e6-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="636e6-115">Not supported</span></span>|
| <span data-ttu-id="636e6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="636e6-116">Application</span></span>                            | <span data-ttu-id="636e6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="636e6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="636e6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="636e6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="636e6-119">Чтобы опубликовать приложение, для которого требуется проверка, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="636e6-119">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="636e6-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="636e6-120">Query parameters</span></span>

|<span data-ttu-id="636e6-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="636e6-121">Property</span></span>|<span data-ttu-id="636e6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="636e6-122">Type</span></span>|<span data-ttu-id="636e6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="636e6-123">Description</span></span>|
|----|----|----|
|<span data-ttu-id="636e6-124">рекуиресревиев</span><span class="sxs-lookup"><span data-stu-id="636e6-124">requiresReview</span></span>| <span data-ttu-id="636e6-125">Логический</span><span class="sxs-lookup"><span data-stu-id="636e6-125">Boolean</span></span> | <span data-ttu-id="636e6-126">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="636e6-126">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="636e6-127">Пользователи с правами администратора могут отсылать приложения, не запуская проверку.</span><span class="sxs-lookup"><span data-stu-id="636e6-127">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="636e6-128">Если пользователям требуется предварительно запросить проверку перед публикацией, необходимо задать  `requiresReview` для них значение `true` .</span><span class="sxs-lookup"><span data-stu-id="636e6-128">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="636e6-129">Пользователь с правами администратора может не устанавливать `requiresReview` или устанавливать значение `false`  , и приложение считается утвержденным и будет публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="636e6-129">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="636e6-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="636e6-130">Request headers</span></span>

| <span data-ttu-id="636e6-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="636e6-131">Header</span></span>        | <span data-ttu-id="636e6-132">Значение</span><span class="sxs-lookup"><span data-stu-id="636e6-132">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="636e6-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="636e6-133">Authorization</span></span> | <span data-ttu-id="636e6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="636e6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="636e6-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="636e6-136">Content-Type</span></span>  | <span data-ttu-id="636e6-137">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="636e6-137">application/zip.</span></span> <span data-ttu-id="636e6-138">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="636e6-138">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="636e6-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="636e6-139">Request body</span></span>

<span data-ttu-id="636e6-140">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="636e6-140">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="636e6-141">Дополнительные сведения см. в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="636e6-141">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>  

<span data-ttu-id="636e6-142">Каждое приложение в каталоге приложений должно иметь уникальный манифест `id` .</span><span class="sxs-lookup"><span data-stu-id="636e6-142">Each app in the app catalog must have a unique manifest `id`.</span></span>

## <a name="response"></a><span data-ttu-id="636e6-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="636e6-143">Response</span></span>

<span data-ttu-id="636e6-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="636e6-144">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="636e6-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="636e6-145">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="636e6-146">Пример 1: Публикация приложения в каталоге приложений</span><span class="sxs-lookup"><span data-stu-id="636e6-146">Example 1: Publish an app to the app catalog</span></span>
#### <a name="request"></a><span data-ttu-id="636e6-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="636e6-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="636e6-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="636e6-148">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="636e6-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="636e6-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="636e6-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="636e6-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="636e6-151">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="636e6-151">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="636e6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="636e6-152">Response</span></span>

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

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="636e6-153">Пример 2: Отправка нового приложения для проверки в каталог приложений Организации</span><span class="sxs-lookup"><span data-stu-id="636e6-153">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="636e6-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="636e6-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="636e6-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="636e6-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```
# <a name="javascript"></a>[<span data-ttu-id="636e6-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="636e6-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="636e6-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="636e6-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="636e6-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="636e6-158">Response</span></span>

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
