---
title: Обновление teamsApp
description: 'Обновление приложения, опубликованного ранее в каталоге приложений Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0dc3c5f3021c5479ef3eb6f227d7fbe512e0c122
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843165"
---
# <a name="update-teamsapp"></a><span data-ttu-id="95617-103">Обновление teamsApp</span><span class="sxs-lookup"><span data-stu-id="95617-103">Update teamsApp</span></span>

<span data-ttu-id="95617-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95617-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95617-105">Обновление [приложения](../resources/teamsapp.md) , опубликованного ранее в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="95617-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="95617-106">Чтобы обновить приложение, свойству **distributionMethod** для приложения необходимо присвоить значение `organization` .</span><span class="sxs-lookup"><span data-stu-id="95617-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="95617-107">Этот API-интерфейс специально обновляет приложение, опубликованное в каталоге приложений вашей организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="95617-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="95617-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95617-108">Permissions</span></span>

<span data-ttu-id="95617-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95617-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="95617-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="95617-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="95617-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95617-112">Permission Type</span></span>                        | <span data-ttu-id="95617-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95617-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="95617-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95617-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="95617-115">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="95617-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="95617-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95617-116">Delegated (work or school account)</span></span> | <span data-ttu-id="95617-117">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="95617-117">AppCatalog.Submit</span></span>|
| <span data-ttu-id="95617-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95617-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95617-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="95617-119">Not supported</span></span>|
| <span data-ttu-id="95617-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95617-120">Application</span></span>                            | <span data-ttu-id="95617-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95617-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95617-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95617-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="95617-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95617-123">Request headers</span></span>

| <span data-ttu-id="95617-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95617-124">Header</span></span>        | <span data-ttu-id="95617-125">Значение</span><span class="sxs-lookup"><span data-stu-id="95617-125">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="95617-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95617-126">Authorization</span></span> | <span data-ttu-id="95617-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95617-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95617-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95617-129">Content-Type</span></span>  | <span data-ttu-id="95617-130">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="95617-130">application/zip.</span></span> <span data-ttu-id="95617-131">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="95617-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95617-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95617-132">Request body</span></span>

<span data-ttu-id="95617-133">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="95617-133">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="95617-134">Дополнительные сведения см. [в статье Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="95617-134">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="95617-135">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="95617-135">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="95617-136">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="95617-136">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="95617-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="95617-137">Response</span></span>

<span data-ttu-id="95617-138">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="95617-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="95617-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="95617-139">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="95617-140">Пример 1: обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="95617-140">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="95617-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="95617-141">Request</span></span>

<!-- markdownlint-disable MD034 -->
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="95617-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="95617-142">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
