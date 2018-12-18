---
title: Разрешения
description: 'Обновление приложения ранее опубликованы в каталоге приложений группами Майкрософт. '
author: nkramer
ms.openlocfilehash: 60fb80ff6400e7c1d78898b28e3b9f591c01290e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359502"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="cd9cf-103">Обновление приложений, опубликованной в каталоге приложений организации</span><span class="sxs-lookup"><span data-stu-id="cd9cf-103">Update apps published to your organization's app catalog</span></span>

> <span data-ttu-id="cd9cf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd9cf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd9cf-106">Обновление [приложения](../resources/teamsapp.md) ранее опубликованы в каталоге приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-106">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="cd9cf-107">Этот интерфейс API специально обновляет приложение, опубликованной в каталоге приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="cd9cf-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="cd9cf-108">Чтобы опубликовать в каталоге приложений организации, укажите `organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-108">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd9cf-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd9cf-109">Permissions</span></span>

<span data-ttu-id="cd9cf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="cd9cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="cd9cf-112">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="cd9cf-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd9cf-113">Permission Type</span></span>                        | <span data-ttu-id="cd9cf-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="cd9cf-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd9cf-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9cf-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="cd9cf-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd9cf-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cd9cf-118">Not supported</span></span>|
| <span data-ttu-id="cd9cf-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd9cf-119">Application</span></span>                            | <span data-ttu-id="cd9cf-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cd9cf-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd9cf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd9cf-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cd9cf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd9cf-122">Request headers</span></span>

| <span data-ttu-id="cd9cf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd9cf-123">Header</span></span>        | <span data-ttu-id="cd9cf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cd9cf-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="cd9cf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd9cf-125">Authorization</span></span> | <span data-ttu-id="cd9cf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd9cf-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd9cf-128">Content-Type</span></span>  | <span data-ttu-id="cd9cf-129">приложение/zip</span><span class="sxs-lookup"><span data-stu-id="cd9cf-129">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd9cf-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd9cf-130">Request body</span></span>

<span data-ttu-id="cd9cf-131">Zip полезных команд манифеста: Для приложения группы ZIP-файл, [перейдите в раздел Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-131">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="cd9cf-132">**Примечание:** Используйте код, возвращенный вызова [списка публикации приложений](./teamsapp-list.md) для ссылок на приложением, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-132">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="cd9cf-133">Не используйте код из манифеста приложения ZIP-архив.</span><span class="sxs-lookup"><span data-stu-id="cd9cf-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="cd9cf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd9cf-134">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="cd9cf-135">Пример</span><span class="sxs-lookup"><span data-stu-id="cd9cf-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd9cf-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd9cf-136">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="cd9cf-137">Для приложения группы ZIP-файл [видеть создать пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="cd9cf-137">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="cd9cf-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd9cf-138">Response</span></span>

```
HTTP/1.1 204 No Content
```
