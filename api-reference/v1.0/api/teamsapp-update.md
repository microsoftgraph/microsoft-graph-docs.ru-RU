---
title: Обновление teamsApp
description: 'Обновление приложения, опубликованного ранее в каталоге приложений Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f54f7938e448d83a9ac2ff70e1dfb215e1b71d6
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849153"
---
# <a name="update-teamsapp"></a><span data-ttu-id="eb0af-103">Обновление teamsApp</span><span class="sxs-lookup"><span data-stu-id="eb0af-103">Update teamsApp</span></span>

<span data-ttu-id="eb0af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb0af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb0af-105">Обновление [приложения](../resources/teamsapp.md) , опубликованного ранее в каталоге приложений Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="eb0af-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="eb0af-106">Чтобы обновить приложение, свойству **distributionMethod** для приложения необходимо присвоить значение `organization` .</span><span class="sxs-lookup"><span data-stu-id="eb0af-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="eb0af-107">Этот API-интерфейс специально обновляет приложение, опубликованное в каталоге приложений вашей организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="eb0af-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb0af-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb0af-108">Permissions</span></span>

<span data-ttu-id="eb0af-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb0af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="eb0af-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="eb0af-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="eb0af-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb0af-112">Permission Type</span></span>                        | <span data-ttu-id="eb0af-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb0af-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="eb0af-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb0af-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb0af-115">CamlQuery. оправить, CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="eb0af-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="eb0af-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb0af-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb0af-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eb0af-117">Not supported</span></span>|
| <span data-ttu-id="eb0af-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb0af-118">Application</span></span>                            | <span data-ttu-id="eb0af-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb0af-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb0af-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb0af-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="eb0af-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb0af-121">Request headers</span></span>

| <span data-ttu-id="eb0af-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb0af-122">Header</span></span>        | <span data-ttu-id="eb0af-123">Значение</span><span class="sxs-lookup"><span data-stu-id="eb0af-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="eb0af-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb0af-124">Authorization</span></span> | <span data-ttu-id="eb0af-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb0af-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eb0af-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb0af-127">Content-Type</span></span>  | <span data-ttu-id="eb0af-128">Application/ZIP.</span><span class="sxs-lookup"><span data-stu-id="eb0af-128">application/zip.</span></span> <span data-ttu-id="eb0af-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="eb0af-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb0af-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb0af-130">Request body</span></span>

<span data-ttu-id="eb0af-131">В тексте запроса включите полезные данные манифеста ZIP для Teams.</span><span class="sxs-lookup"><span data-stu-id="eb0af-131">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="eb0af-132">Дополнительные сведения см. [в статье Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="eb0af-132">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="eb0af-133">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="eb0af-133">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="eb0af-134">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="eb0af-134">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="eb0af-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb0af-135">Response</span></span>

<span data-ttu-id="eb0af-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eb0af-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="eb0af-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="eb0af-137">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="eb0af-138">Пример 1: обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eb0af-138">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="eb0af-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb0af-139">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="eb0af-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb0af-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eb0af-141">C#</span><span class="sxs-lookup"><span data-stu-id="eb0af-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb0af-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb0af-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="eb0af-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb0af-143">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
