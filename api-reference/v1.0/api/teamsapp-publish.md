---
title: Разрешения
description: 'Опубликуйте приложение в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8076cc4ec988c311dd9a4cfde3b01a27a2a5d88e
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345767"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="7040f-103">Публикация приложений в каталоге приложений Организации</span><span class="sxs-lookup"><span data-stu-id="7040f-103">Publish apps to your organization's app catalog</span></span>

<span data-ttu-id="7040f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7040f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="7040f-105">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7040f-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="7040f-106">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь `distributionMethod`  =  `organization` .</span><span class="sxs-lookup"><span data-stu-id="7040f-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="7040f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7040f-107">Permissions</span></span>

<span data-ttu-id="7040f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7040f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="7040f-110">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="7040f-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="7040f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7040f-111">Permission Type</span></span>                        | <span data-ttu-id="7040f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7040f-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="7040f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7040f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7040f-114">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7040f-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="7040f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7040f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7040f-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7040f-116">Not supported</span></span>|
| <span data-ttu-id="7040f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7040f-117">Application</span></span>                            | <span data-ttu-id="7040f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7040f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7040f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7040f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="7040f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7040f-120">Request headers</span></span>

| <span data-ttu-id="7040f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7040f-121">Header</span></span>        | <span data-ttu-id="7040f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7040f-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="7040f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7040f-123">Authorization</span></span> | <span data-ttu-id="7040f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7040f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7040f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7040f-126">Content-Type</span></span>  | <span data-ttu-id="7040f-127">приложение/ZIP-индекс</span><span class="sxs-lookup"><span data-stu-id="7040f-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="7040f-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="7040f-128">Request body</span></span>

<span data-ttu-id="7040f-129">Полезные данные манифеста ZIP Teams.</span><span class="sxs-lookup"><span data-stu-id="7040f-129">Teams Zip Manifest Payload.</span></span>
<span data-ttu-id="7040f-130">Для ZIP-файла приложения Teams [в разделе Create a App Package](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="7040f-130">For Teams application zip file [see Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<span data-ttu-id="7040f-131">Вы не можете создать приложение для Организации с таким же ИДЕНТИФИКАТОРом манифеста, что и у другого приложения в этой Организации.</span><span class="sxs-lookup"><span data-stu-id="7040f-131">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="7040f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7040f-132">Response</span></span>

<span data-ttu-id="7040f-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7040f-133">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="7040f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7040f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7040f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7040f-135">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="7040f-136">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="7040f-136">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

### <a name="response"></a><span data-ttu-id="7040f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7040f-137">Response</span></span>

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
