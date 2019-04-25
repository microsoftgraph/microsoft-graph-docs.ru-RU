---
title: Разрешения
description: 'Опубликуйте приложение в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7acd916aa04200c626d8045e7da5a6d00be8a951
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544561"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="ef0c6-103">Публикация приложений в каталоге приложений Организации</span><span class="sxs-lookup"><span data-stu-id="ef0c6-103">Publish apps to your organization's app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef0c6-104">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ef0c6-104">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="ef0c6-105">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь `distributionMethod`  =  `organization`.</span><span class="sxs-lookup"><span data-stu-id="ef0c6-105">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef0c6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef0c6-106">Permissions</span></span>

<span data-ttu-id="ef0c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="ef0c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="ef0c6-109">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ef0c6-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="ef0c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef0c6-110">Permission Type</span></span>                        | <span data-ttu-id="ef0c6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef0c6-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="ef0c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef0c6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef0c6-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef0c6-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="ef0c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef0c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef0c6-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef0c6-115">Not supported</span></span>|
| <span data-ttu-id="ef0c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef0c6-116">Application</span></span>                            | <span data-ttu-id="ef0c6-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef0c6-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef0c6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef0c6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="ef0c6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef0c6-119">Request headers</span></span>

| <span data-ttu-id="ef0c6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef0c6-120">Header</span></span>        | <span data-ttu-id="ef0c6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ef0c6-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="ef0c6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef0c6-122">Authorization</span></span> | <span data-ttu-id="ef0c6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef0c6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ef0c6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef0c6-125">Content-Type</span></span>  | <span data-ttu-id="ef0c6-126">приложение/ZIP-индекс</span><span class="sxs-lookup"><span data-stu-id="ef0c6-126">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef0c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef0c6-127">Request body</span></span>

<span data-ttu-id="ef0c6-128">Полезные данные манифеста ZIP Teams.</span><span class="sxs-lookup"><span data-stu-id="ef0c6-128">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="ef0c6-129">Для ZIP-файла приложения Teams [в разделе Create a App Package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="ef0c6-129">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="ef0c6-130">Вы не можете создать приложение для Организации с таким же ИДЕНТИФИКАТОРом манифеста, что и у другого приложения в этой Организации.</span><span class="sxs-lookup"><span data-stu-id="ef0c6-130">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="ef0c6-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef0c6-131">Response</span></span>

<span data-ttu-id="ef0c6-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ef0c6-132">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="ef0c6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ef0c6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef0c6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef0c6-134">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="ef0c6-135">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="ef0c6-135">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="ef0c6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef0c6-136">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
