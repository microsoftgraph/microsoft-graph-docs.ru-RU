---
title: Публикация teamsapp
description: 'Опубликуйте приложение в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 86a63997b9408cd4155a180d7919e54e99d8ad27
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607170"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="bf420-103">Публикация teamsapp</span><span class="sxs-lookup"><span data-stu-id="bf420-103">Publish teamsapp</span></span>

<span data-ttu-id="bf420-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf420-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf420-105">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bf420-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="bf420-106">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь значение свойства **distributionMethod** `organization` .</span><span class="sxs-lookup"><span data-stu-id="bf420-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf420-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf420-107">Permissions</span></span>

<span data-ttu-id="bf420-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf420-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="bf420-110">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bf420-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="bf420-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf420-111">Permission Type</span></span>                        | <span data-ttu-id="bf420-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf420-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="bf420-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf420-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf420-114">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bf420-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="bf420-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf420-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf420-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf420-116">Not supported</span></span>|
| <span data-ttu-id="bf420-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf420-117">Application</span></span>                            | <span data-ttu-id="bf420-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf420-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf420-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf420-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="bf420-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf420-120">Request headers</span></span>

| <span data-ttu-id="bf420-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf420-121">Header</span></span>        | <span data-ttu-id="bf420-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bf420-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="bf420-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf420-123">Authorization</span></span> | <span data-ttu-id="bf420-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf420-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf420-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf420-126">Content-Type</span></span>  | <span data-ttu-id="bf420-127">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="bf420-127">application/zip.</span></span> <span data-ttu-id="bf420-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bf420-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf420-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf420-129">Request body</span></span>

<span data-ttu-id="bf420-130">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="bf420-130">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="bf420-131">Дополнительные сведения см. в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="bf420-131">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="bf420-132">Каждое приложение в каталоге приложений должно иметь уникальный идентификатор манифеста.</span><span class="sxs-lookup"><span data-stu-id="bf420-132">Each app in the app catalog must have a unique manifest ID.</span></span>

## <a name="response"></a><span data-ttu-id="bf420-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf420-133">Response</span></span>

<span data-ttu-id="bf420-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bf420-134">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="bf420-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="bf420-135">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="bf420-136">Пример 1: Публикация приложения в каталоге приложений</span><span class="sxs-lookup"><span data-stu-id="bf420-136">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="bf420-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf420-137">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="bf420-138">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="bf420-138">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="bf420-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf420-139">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
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
