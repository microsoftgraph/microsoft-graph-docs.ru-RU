---
title: Публикация teamsapp
description: Опубликуйте приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cf5dde98d9f21249a23d6806b4f79dd6ae824572
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741938"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="848b0-103">Публикация teamsApp</span><span class="sxs-lookup"><span data-stu-id="848b0-103">Publish teamsApp</span></span>

<span data-ttu-id="848b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="848b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="848b0-105">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="848b0-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="848b0-106">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь значение свойства **distributionMethod** `organization` .</span><span class="sxs-lookup"><span data-stu-id="848b0-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="848b0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="848b0-107">Permissions</span></span>

<span data-ttu-id="848b0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="848b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="848b0-110">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="848b0-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="848b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="848b0-111">Permission Type</span></span>                        | <span data-ttu-id="848b0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="848b0-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="848b0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="848b0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="848b0-114">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="848b0-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="848b0-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="848b0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="848b0-116">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="848b0-116">AppCatalog.Submit</span></span>|
| <span data-ttu-id="848b0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="848b0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="848b0-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="848b0-118">Not supported</span></span>|
| <span data-ttu-id="848b0-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="848b0-119">Application</span></span>                            | <span data-ttu-id="848b0-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="848b0-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="848b0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="848b0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="848b0-122">Чтобы опубликовать приложение, для которого требуется проверка, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="848b0-122">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="848b0-123">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="848b0-123">Query parameters</span></span>

|<span data-ttu-id="848b0-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="848b0-124">Property</span></span>|<span data-ttu-id="848b0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="848b0-125">Type</span></span>|<span data-ttu-id="848b0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="848b0-126">Description</span></span>|
|----|----|----|
|<span data-ttu-id="848b0-127">рекуиресревиев</span><span class="sxs-lookup"><span data-stu-id="848b0-127">requiresReview</span></span>| <span data-ttu-id="848b0-128">Логический</span><span class="sxs-lookup"><span data-stu-id="848b0-128">Boolean</span></span> | <span data-ttu-id="848b0-129">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="848b0-129">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="848b0-130">Пользователи с правами администратора могут отсылать приложения, не запуская проверку.</span><span class="sxs-lookup"><span data-stu-id="848b0-130">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="848b0-131">Если пользователям требуется предварительно запросить проверку перед публикацией, необходимо задать  `requiresReview` для них значение `true` .</span><span class="sxs-lookup"><span data-stu-id="848b0-131">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="848b0-132">Пользователь с правами администратора может не устанавливать `requiresReview` или устанавливать значение `false`  , и приложение считается утвержденным и будет публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="848b0-132">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="848b0-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="848b0-133">Request headers</span></span>

| <span data-ttu-id="848b0-134">Заголовок</span><span class="sxs-lookup"><span data-stu-id="848b0-134">Header</span></span>        | <span data-ttu-id="848b0-135">Значение</span><span class="sxs-lookup"><span data-stu-id="848b0-135">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="848b0-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="848b0-136">Authorization</span></span> | <span data-ttu-id="848b0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="848b0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="848b0-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="848b0-139">Content-Type</span></span>  | <span data-ttu-id="848b0-140">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="848b0-140">application/zip.</span></span> <span data-ttu-id="848b0-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="848b0-141">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="848b0-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="848b0-142">Request body</span></span>

<span data-ttu-id="848b0-143">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="848b0-143">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="848b0-144">Дополнительные сведения см. в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="848b0-144">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>  

<span data-ttu-id="848b0-145">Каждое приложение в каталоге приложений должно иметь уникальный манифест `id` .</span><span class="sxs-lookup"><span data-stu-id="848b0-145">Each app in the app catalog must have a unique manifest `id`.</span></span>

## <a name="response"></a><span data-ttu-id="848b0-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="848b0-146">Response</span></span>

<span data-ttu-id="848b0-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="848b0-147">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="848b0-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="848b0-148">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="848b0-149">Пример 1: Публикация приложения в каталоге приложений</span><span class="sxs-lookup"><span data-stu-id="848b0-149">Example 1: Publish an app to the app catalog</span></span>
#### <a name="request"></a><span data-ttu-id="848b0-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="848b0-150">Request</span></span>

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

<span data-ttu-id="848b0-151">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="848b0-151">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="848b0-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="848b0-152">Response</span></span>

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

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="848b0-153">Пример 2: Отправка нового приложения для проверки в каталог приложений Организации</span><span class="sxs-lookup"><span data-stu-id="848b0-153">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="848b0-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="848b0-154">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

#### <a name="response"></a><span data-ttu-id="848b0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="848b0-155">Response</span></span>

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
