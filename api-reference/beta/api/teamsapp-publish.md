---
title: Permissions
description: 'Публикация приложения в каталоге приложений группами Майкрософт. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 0d6e98fc3c95485fc771a6db841021940b0c87a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864983"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="8cdf2-103">Публикация приложений в каталоге приложений организации</span><span class="sxs-lookup"><span data-stu-id="8cdf2-103">Publish apps to your organization's app catalog</span></span>

> <span data-ttu-id="8cdf2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cdf2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cdf2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cdf2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cdf2-106">Публикация [приложения](../resources/teamsapp.md) в каталог приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="8cdf2-106">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="8cdf2-107">В частности этот интерфейс API публикует приложение в каталоге организации (клиент каталога приложений); созданный ресурс будет иметь `distributionMethod`  =  `organization`.</span><span class="sxs-lookup"><span data-stu-id="8cdf2-107">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cdf2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cdf2-108">Permissions</span></span>

<span data-ttu-id="8cdf2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="8cdf2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="8cdf2-111">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="8cdf2-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="8cdf2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cdf2-112">Permission Type</span></span>                        | <span data-ttu-id="8cdf2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cdf2-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="8cdf2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cdf2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cdf2-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cdf2-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="8cdf2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cdf2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cdf2-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8cdf2-117">Not supported</span></span>|
| <span data-ttu-id="8cdf2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cdf2-118">Application</span></span>                            | <span data-ttu-id="8cdf2-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8cdf2-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cdf2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cdf2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="8cdf2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cdf2-121">Request headers</span></span>

| <span data-ttu-id="8cdf2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cdf2-122">Header</span></span>        | <span data-ttu-id="8cdf2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8cdf2-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="8cdf2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8cdf2-124">Authorization</span></span> | <span data-ttu-id="8cdf2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cdf2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8cdf2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cdf2-127">Content-Type</span></span>  | <span data-ttu-id="8cdf2-128">приложение/zip</span><span class="sxs-lookup"><span data-stu-id="8cdf2-128">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cdf2-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8cdf2-129">Request body</span></span>

<span data-ttu-id="8cdf2-130">Zip полезных команд манифеста.</span><span class="sxs-lookup"><span data-stu-id="8cdf2-130">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="8cdf2-131">Для приложения группы ZIP-файл, [перейдите в раздел Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8cdf2-131">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="8cdf2-132">Не удается создать приложения для организации, которая имеет тот же идентификатор манифеста в качестве другого приложения в организации.</span><span class="sxs-lookup"><span data-stu-id="8cdf2-132">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="8cdf2-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cdf2-133">Response</span></span>

<span data-ttu-id="8cdf2-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8cdf2-134">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="8cdf2-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8cdf2-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cdf2-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cdf2-136">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="8cdf2-137">Сведения о создании ZIP-файл приложения группами Майкрософт перейдите в раздел [Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8cdf2-137">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="8cdf2-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cdf2-138">Response</span></span>

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
