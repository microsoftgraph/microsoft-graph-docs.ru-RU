---
title: Публикация teamsapp
description: 'Опубликуйте приложение в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 838fccb30041f61b7477bc53ced3c7d1d93e39a1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808954"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="743fe-103">Публикация teamsapp</span><span class="sxs-lookup"><span data-stu-id="743fe-103">Publish teamsapp</span></span>

<span data-ttu-id="743fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="743fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="743fe-105">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="743fe-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="743fe-106">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь значение свойства **distributionMethod** `organization` .</span><span class="sxs-lookup"><span data-stu-id="743fe-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="743fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="743fe-107">Permissions</span></span>

<span data-ttu-id="743fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="743fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="743fe-110">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="743fe-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="743fe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="743fe-111">Permission Type</span></span>                        | <span data-ttu-id="743fe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="743fe-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="743fe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="743fe-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="743fe-114">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="743fe-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="743fe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="743fe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="743fe-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="743fe-116">Not supported</span></span>|
| <span data-ttu-id="743fe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="743fe-117">Application</span></span>                            | <span data-ttu-id="743fe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="743fe-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="743fe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="743fe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```
<span data-ttu-id="743fe-120">Чтобы опубликовать приложение, для которого требуется проверка, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="743fe-120">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="743fe-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="743fe-121">Query parameters</span></span>

|<span data-ttu-id="743fe-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="743fe-122">Property</span></span>|<span data-ttu-id="743fe-123">Тип</span><span class="sxs-lookup"><span data-stu-id="743fe-123">Type</span></span>|<span data-ttu-id="743fe-124">Описание</span><span class="sxs-lookup"><span data-stu-id="743fe-124">Description</span></span>|
|----|----|----|
|<span data-ttu-id="743fe-125">рекуиресревиев</span><span class="sxs-lookup"><span data-stu-id="743fe-125">requiresReview</span></span>| <span data-ttu-id="743fe-126">Логический</span><span class="sxs-lookup"><span data-stu-id="743fe-126">Boolean</span></span> | <span data-ttu-id="743fe-127">Этот необязательный параметр запроса запускает процесс проверки приложения.</span><span class="sxs-lookup"><span data-stu-id="743fe-127">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="743fe-128">Пользователи с правами администратора могут отсылать приложения, не запуская проверку.</span><span class="sxs-lookup"><span data-stu-id="743fe-128">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="743fe-129">Если пользователям требуется предварительно запросить проверку перед публикацией, необходимо задать  `requiresReview` для них значение `true` .</span><span class="sxs-lookup"><span data-stu-id="743fe-129">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="743fe-130">Пользователь с правами администратора может не устанавливать `requiresReview` или устанавливать значение `false`  , и приложение считается утвержденным и будет публиковаться мгновенно.</span><span class="sxs-lookup"><span data-stu-id="743fe-130">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="743fe-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="743fe-131">Request headers</span></span>

| <span data-ttu-id="743fe-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="743fe-132">Header</span></span>        | <span data-ttu-id="743fe-133">Значение</span><span class="sxs-lookup"><span data-stu-id="743fe-133">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="743fe-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="743fe-134">Authorization</span></span> | <span data-ttu-id="743fe-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="743fe-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="743fe-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="743fe-137">Content-Type</span></span>  | <span data-ttu-id="743fe-138">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="743fe-138">application/zip.</span></span> <span data-ttu-id="743fe-139">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="743fe-139">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="743fe-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="743fe-140">Request body</span></span>

<span data-ttu-id="743fe-141">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="743fe-141">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="743fe-142">Дополнительные сведения см. в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="743fe-142">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="743fe-143">Каждое приложение в каталоге приложений должно иметь уникальный идентификатор манифеста.</span><span class="sxs-lookup"><span data-stu-id="743fe-143">Each app in the app catalog must have a unique manifest id.</span></span>

## <a name="response"></a><span data-ttu-id="743fe-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="743fe-144">Response</span></span>

<span data-ttu-id="743fe-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="743fe-145">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="743fe-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="743fe-146">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="743fe-147">Пример 1: Публикация приложения в каталоге приложений</span><span class="sxs-lookup"><span data-stu-id="743fe-147">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="743fe-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="743fe-148">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="743fe-149">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="743fe-149">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="743fe-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="743fe-150">Response</span></span>

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
### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="743fe-151">Пример 2: Отправка нового приложения для проверки в каталог приложений Организации</span><span class="sxs-lookup"><span data-stu-id="743fe-151">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="743fe-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="743fe-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="743fe-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="743fe-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```
# <a name="javascript"></a>[<span data-ttu-id="743fe-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="743fe-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="743fe-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="743fe-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="743fe-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="743fe-156">Response</span></span>

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
