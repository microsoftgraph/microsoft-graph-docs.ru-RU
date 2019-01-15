---
title: Разрешения
description: 'Обновление приложения ранее опубликованы в каталоге приложений группами Майкрософт. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b89380a423bf01f6a2bd7e56086cc9290be094cb
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016627"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="ab5c3-103">Обновление приложений, опубликованной в каталоге приложений организации</span><span class="sxs-lookup"><span data-stu-id="ab5c3-103">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="ab5c3-104">Обновление [приложения](../resources/teamsapp.md) ранее опубликованы в каталоге приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ab5c3-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="ab5c3-105">Этот интерфейс API специально обновляет приложение, опубликованной в каталоге приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="ab5c3-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="ab5c3-106">Чтобы опубликовать в каталоге приложений организации, укажите `organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ab5c3-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab5c3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab5c3-107">Permissions</span></span>

<span data-ttu-id="ab5c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="ab5c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="ab5c3-110">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="ab5c3-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="ab5c3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab5c3-111">Permission Type</span></span>                        | <span data-ttu-id="ab5c3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab5c3-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="ab5c3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab5c3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab5c3-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab5c3-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="ab5c3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab5c3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab5c3-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ab5c3-116">Not supported</span></span>|
| <span data-ttu-id="ab5c3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab5c3-117">Application</span></span>                            | <span data-ttu-id="ab5c3-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ab5c3-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab5c3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab5c3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ab5c3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab5c3-120">Request headers</span></span>

| <span data-ttu-id="ab5c3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab5c3-121">Header</span></span>        | <span data-ttu-id="ab5c3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab5c3-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="ab5c3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab5c3-123">Authorization</span></span> | <span data-ttu-id="ab5c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab5c3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab5c3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab5c3-126">Content-Type</span></span>  | <span data-ttu-id="ab5c3-127">приложение/zip</span><span class="sxs-lookup"><span data-stu-id="ab5c3-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab5c3-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab5c3-128">Request body</span></span>

<span data-ttu-id="ab5c3-129">Zip полезных команд манифеста: Для приложения группы ZIP-файл, [перейдите в раздел Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="ab5c3-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="ab5c3-130">**Примечание:** Используйте код, возвращенный вызова [списка публикации приложений](./teamsapp-list.md) для ссылок на приложением, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="ab5c3-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="ab5c3-131">Не используйте код из манифеста приложения ZIP-архив.</span><span class="sxs-lookup"><span data-stu-id="ab5c3-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="ab5c3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab5c3-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="ab5c3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ab5c3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab5c3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab5c3-134">Request</span></span>

```
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="ab5c3-135">Для приложения группы ZIP-файл [видеть создать пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="ab5c3-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="ab5c3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab5c3-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
