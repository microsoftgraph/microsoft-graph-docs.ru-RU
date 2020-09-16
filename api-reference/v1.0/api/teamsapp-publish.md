---
title: Публикация teamsapp
description: 'Опубликуйте приложение в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6aeef8c0faf1ab89b48d086839688e9ebe120efd
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843172"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="f70a1-103">Публикация teamsapp</span><span class="sxs-lookup"><span data-stu-id="f70a1-103">Publish teamsapp</span></span>

<span data-ttu-id="f70a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f70a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f70a1-105">Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f70a1-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="f70a1-106">В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь значение свойства **distributionMethod** `organization` .</span><span class="sxs-lookup"><span data-stu-id="f70a1-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="f70a1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f70a1-107">Permissions</span></span>

<span data-ttu-id="f70a1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="f70a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="f70a1-110">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f70a1-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="f70a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f70a1-111">Permission Type</span></span>                        | <span data-ttu-id="f70a1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f70a1-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="f70a1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f70a1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f70a1-114">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f70a1-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="f70a1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f70a1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f70a1-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f70a1-116">Not supported</span></span>|
| <span data-ttu-id="f70a1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f70a1-117">Application</span></span>                            | <span data-ttu-id="f70a1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f70a1-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f70a1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f70a1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="f70a1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f70a1-120">Request headers</span></span>

| <span data-ttu-id="f70a1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f70a1-121">Header</span></span>        | <span data-ttu-id="f70a1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f70a1-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="f70a1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f70a1-123">Authorization</span></span> | <span data-ttu-id="f70a1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f70a1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f70a1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f70a1-126">Content-Type</span></span>  | <span data-ttu-id="f70a1-127">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="f70a1-127">application/zip.</span></span> <span data-ttu-id="f70a1-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f70a1-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f70a1-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f70a1-129">Request body</span></span>

<span data-ttu-id="f70a1-130">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="f70a1-130">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="f70a1-131">Дополнительные сведения см. в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f70a1-131">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="f70a1-132">Каждое приложение в каталоге приложений должно иметь уникальный идентификатор манифеста.</span><span class="sxs-lookup"><span data-stu-id="f70a1-132">Each app in the app catalog must have a unique manifest id.</span></span>

## <a name="response"></a><span data-ttu-id="f70a1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f70a1-133">Response</span></span>

<span data-ttu-id="f70a1-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [teamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f70a1-134">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="f70a1-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="f70a1-135">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="f70a1-136">Пример 1: Публикация приложения в каталоге приложений</span><span class="sxs-lookup"><span data-stu-id="f70a1-136">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="f70a1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f70a1-137">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="f70a1-138">Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="f70a1-138">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="f70a1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f70a1-139">Response</span></span>

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
