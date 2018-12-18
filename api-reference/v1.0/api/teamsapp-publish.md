---
title: Разрешения
description: 'Публикация приложения в каталоге приложений группами Майкрософт. '
author: nkramer
ms.openlocfilehash: 76750e385c8048c44d77064722d84c5765c2bcc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306155"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="664e0-103">Публикация приложений в каталоге приложений организации</span><span class="sxs-lookup"><span data-stu-id="664e0-103">Publish apps to your organization's app catalog</span></span>



<span data-ttu-id="664e0-104">Публикация [приложения](../resources/teamsapp.md) в каталог приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="664e0-104">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="664e0-105">В частности этот интерфейс API публикует приложение в каталоге организации (клиент каталога приложений); созданный ресурс будет иметь `distributionMethod`  =  `organization`.</span><span class="sxs-lookup"><span data-stu-id="664e0-105">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="664e0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="664e0-106">Permissions</span></span>

<span data-ttu-id="664e0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="664e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="664e0-109">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="664e0-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="664e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="664e0-110">Permission Type</span></span>                        | <span data-ttu-id="664e0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="664e0-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="664e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="664e0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="664e0-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="664e0-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="664e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="664e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="664e0-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="664e0-115">Not supported</span></span>|
| <span data-ttu-id="664e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="664e0-116">Application</span></span>                            | <span data-ttu-id="664e0-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="664e0-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="664e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="664e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="664e0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="664e0-119">Request headers</span></span>

| <span data-ttu-id="664e0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="664e0-120">Header</span></span>        | <span data-ttu-id="664e0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="664e0-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="664e0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="664e0-122">Authorization</span></span> | <span data-ttu-id="664e0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="664e0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="664e0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="664e0-125">Content-Type</span></span>  | <span data-ttu-id="664e0-126">приложение/zip</span><span class="sxs-lookup"><span data-stu-id="664e0-126">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="664e0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="664e0-127">Request body</span></span>

<span data-ttu-id="664e0-128">Zip полезных команд манифеста.</span><span class="sxs-lookup"><span data-stu-id="664e0-128">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="664e0-129">Для приложения группы ZIP-файл, [перейдите в раздел Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="664e0-129">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="664e0-130">Не удается создать приложения для организации, которая имеет тот же идентификатор манифеста в качестве другого приложения в организации.</span><span class="sxs-lookup"><span data-stu-id="664e0-130">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="664e0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="664e0-131">Response</span></span>

<span data-ttu-id="664e0-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="664e0-132">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="664e0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="664e0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="664e0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="664e0-134">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="664e0-135">Сведения о создании ZIP-файл приложения группами Майкрософт перейдите в раздел [Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="664e0-135">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="664e0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="664e0-136">Response</span></span>

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
