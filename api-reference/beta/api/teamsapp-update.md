---
title: Разрешения
description: 'Обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 16b3f5ef05a982b1ad54a36f2beacbe7afc3652a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452536"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="68233-103">Обновление приложений, опубликованных в каталоге приложений вашей организации</span><span class="sxs-lookup"><span data-stu-id="68233-103">Update apps published to your organization's app catalog</span></span>

<span data-ttu-id="68233-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68233-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68233-105">Обновление [приложения](../resources/teamsapp.md) , опубликованного ранее в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="68233-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="68233-106">Этот API-интерфейс специально обновляет приложение, опубликованное в каталоге приложений вашей организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="68233-106">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>
<span data-ttu-id="68233-107">Чтобы опубликовать в каталоге приложений вашей организации, укажите `organization` в качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="68233-107">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="68233-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68233-108">Permissions</span></span>

<span data-ttu-id="68233-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="68233-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="68233-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="68233-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="68233-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68233-112">Permission Type</span></span>                        | <span data-ttu-id="68233-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68233-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="68233-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68233-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="68233-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68233-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="68233-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68233-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68233-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="68233-117">Not supported</span></span>|
| <span data-ttu-id="68233-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68233-118">Application</span></span>                            | <span data-ttu-id="68233-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="68233-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="68233-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68233-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="68233-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68233-121">Request headers</span></span>

| <span data-ttu-id="68233-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68233-122">Header</span></span>        | <span data-ttu-id="68233-123">Значение</span><span class="sxs-lookup"><span data-stu-id="68233-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="68233-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68233-124">Authorization</span></span> | <span data-ttu-id="68233-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68233-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="68233-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68233-127">Content-Type</span></span>  | <span data-ttu-id="68233-128">приложение/ZIP-индекс</span><span class="sxs-lookup"><span data-stu-id="68233-128">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="68233-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="68233-129">Request body</span></span>

<span data-ttu-id="68233-130">Полезные данные манифеста ZIP для teams: в ZIP-файле приложения Teams [см. Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="68233-130">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="68233-131">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="68233-131">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span>
<span data-ttu-id="68233-132">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="68233-132">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="68233-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="68233-133">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="68233-134">Пример</span><span class="sxs-lookup"><span data-stu-id="68233-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="68233-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="68233-135">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="68233-136">Для ZIP-файла приложения Teams [см. Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="68233-136">For Teams application zip file [see Create app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="68233-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="68233-137">Response</span></span>

```
HTTP/1.1 204 No Content
```
