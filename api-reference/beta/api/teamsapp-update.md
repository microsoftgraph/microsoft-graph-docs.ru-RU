---
title: Разрешения
description: 'Обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 02822690d18076ee5ce2535c06e2856afe89e3c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977554"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="4680e-103">Обновление приложений, опубликованных в каталоге приложений вашей организации</span><span class="sxs-lookup"><span data-stu-id="4680e-103">Update apps published to your organization's app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4680e-104">Обновление [приложения](../resources/teamsapp.md) , опубликованного ранее в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4680e-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="4680e-105">Этот API-интерфейс специально обновляет приложение, опубликованное в каталоге приложений вашей организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="4680e-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="4680e-106">Чтобы опубликовать в каталоге приложений вашей организации, укажите `organization` в качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="4680e-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="4680e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4680e-107">Permissions</span></span>

<span data-ttu-id="4680e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="4680e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="4680e-110">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4680e-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="4680e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4680e-111">Permission Type</span></span>                        | <span data-ttu-id="4680e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4680e-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="4680e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4680e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4680e-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4680e-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="4680e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4680e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4680e-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4680e-116">Not supported</span></span>|
| <span data-ttu-id="4680e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4680e-117">Application</span></span>                            | <span data-ttu-id="4680e-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4680e-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="4680e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4680e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4680e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4680e-120">Request headers</span></span>

| <span data-ttu-id="4680e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4680e-121">Header</span></span>        | <span data-ttu-id="4680e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4680e-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="4680e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4680e-123">Authorization</span></span> | <span data-ttu-id="4680e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4680e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4680e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4680e-126">Content-Type</span></span>  | <span data-ttu-id="4680e-127">приложение/ZIP-индекс</span><span class="sxs-lookup"><span data-stu-id="4680e-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="4680e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4680e-128">Request body</span></span>

<span data-ttu-id="4680e-129">Полезные данные манифеста ZIP для teams: в ZIP-файле приложения Teams [см. Создание пакета приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="4680e-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="4680e-130">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="4680e-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="4680e-131">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="4680e-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="4680e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4680e-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="4680e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4680e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4680e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4680e-134">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="4680e-135">Для ZIP-файла приложения Teams [см. Создание пакета приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="4680e-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="4680e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4680e-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
