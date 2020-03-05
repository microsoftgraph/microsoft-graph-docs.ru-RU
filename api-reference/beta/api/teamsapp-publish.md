---
title: Разрешения
description: 'Опубликуйте приложение в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0083a0006028198bd15d4abb50aaf27a16b26d40
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452538"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="3cf04-103">Публикация приложений в каталоге приложений Организации</span><span class="sxs-lookup"><span data-stu-id="3cf04-103">Publish apps to your organization's app catalog</span></span>

<span data-ttu-id="3cf04-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3cf04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cf04-105">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3cf04-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="3cf04-106">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь `distributionMethod`  =  `organization`.</span><span class="sxs-lookup"><span data-stu-id="3cf04-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cf04-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cf04-107">Permissions</span></span>

<span data-ttu-id="3cf04-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="3cf04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="3cf04-110">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3cf04-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="3cf04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cf04-111">Permission Type</span></span>                        | <span data-ttu-id="3cf04-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cf04-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="3cf04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cf04-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cf04-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cf04-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="3cf04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cf04-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cf04-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3cf04-116">Not supported</span></span>|
| <span data-ttu-id="3cf04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cf04-117">Application</span></span>                            | <span data-ttu-id="3cf04-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3cf04-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cf04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cf04-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="3cf04-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cf04-120">Request headers</span></span>

| <span data-ttu-id="3cf04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cf04-121">Header</span></span>        | <span data-ttu-id="3cf04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3cf04-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="3cf04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cf04-123">Authorization</span></span> | <span data-ttu-id="3cf04-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cf04-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3cf04-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3cf04-126">Content-Type</span></span>  | <span data-ttu-id="3cf04-127">приложение/ZIP-индекс</span><span class="sxs-lookup"><span data-stu-id="3cf04-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cf04-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cf04-128">Request body</span></span>

<span data-ttu-id="3cf04-129">Полезные данные манифеста ZIP Teams.</span><span class="sxs-lookup"><span data-stu-id="3cf04-129">Teams Zip Manifest Payload.</span></span>
<span data-ttu-id="3cf04-130">Для ZIP-файла приложения Teams [в разделе Create a App Package](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="3cf04-130">For Teams application zip file [see Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<span data-ttu-id="3cf04-131">Вы не можете создать приложение для Организации с таким же ИДЕНТИФИКАТОРом манифеста, что и у другого приложения в этой Организации.</span><span class="sxs-lookup"><span data-stu-id="3cf04-131">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="3cf04-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cf04-132">Response</span></span>

<span data-ttu-id="3cf04-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3cf04-133">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="3cf04-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3cf04-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cf04-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cf04-135">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="3cf04-136">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="3cf04-136">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

### <a name="response"></a><span data-ttu-id="3cf04-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cf04-137">Response</span></span>

```
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
