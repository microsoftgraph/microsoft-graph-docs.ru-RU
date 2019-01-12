---
title: Permissions
description: 'Обновление приложения ранее опубликованы в каталоге приложений группами Майкрософт. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 44ca5870fd585ef7cd5aa0c0282eac42d41c1a18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948524"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="d2521-103">Обновление приложений, опубликованной в каталоге приложений организации</span><span class="sxs-lookup"><span data-stu-id="d2521-103">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="d2521-104">Обновление [приложения](../resources/teamsapp.md) ранее опубликованы в каталоге приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d2521-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="d2521-105">Этот интерфейс API специально обновляет приложение, опубликованной в каталоге приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="d2521-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="d2521-106">Чтобы опубликовать в каталоге приложений организации, укажите `organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d2521-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2521-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2521-107">Permissions</span></span>

<span data-ttu-id="d2521-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="d2521-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="d2521-110">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="d2521-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="d2521-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2521-111">Permission Type</span></span>                        | <span data-ttu-id="d2521-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2521-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="d2521-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2521-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2521-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2521-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="d2521-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2521-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2521-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d2521-116">Not supported</span></span>|
| <span data-ttu-id="d2521-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2521-117">Application</span></span>                            | <span data-ttu-id="d2521-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d2521-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2521-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2521-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d2521-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2521-120">Request headers</span></span>

| <span data-ttu-id="d2521-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2521-121">Header</span></span>        | <span data-ttu-id="d2521-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d2521-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="d2521-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2521-123">Authorization</span></span> | <span data-ttu-id="d2521-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2521-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2521-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2521-126">Content-Type</span></span>  | <span data-ttu-id="d2521-127">приложение/zip</span><span class="sxs-lookup"><span data-stu-id="d2521-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2521-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2521-128">Request body</span></span>

<span data-ttu-id="d2521-129">Zip полезных команд манифеста: Для приложения группы ZIP-файл, [перейдите в раздел Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="d2521-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="d2521-130">**Примечание:** Используйте код, возвращенный вызова [списка публикации приложений](./teamsapp-list.md) для ссылок на приложением, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="d2521-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="d2521-131">Не используйте код из манифеста приложения ZIP-архив.</span><span class="sxs-lookup"><span data-stu-id="d2521-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="d2521-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2521-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="d2521-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d2521-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2521-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2521-134">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="d2521-135">Для приложения группы ZIP-файл [видеть создать пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="d2521-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="d2521-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2521-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
