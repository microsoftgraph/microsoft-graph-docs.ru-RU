---
title: Удаление teamsApp
description: 'Удаление приложения Teams из каталога приложений организации (каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bbaf69d70a73626a550356e0ca235d693be7f3a6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471665"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="783fd-103">Удаление teamsApp</span><span class="sxs-lookup"><span data-stu-id="783fd-103">Delete teamsApp</span></span>

<span data-ttu-id="783fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="783fd-104">Namespace: microsoft.graph</span></span>

<!-- markdownlint-disable MD001 -->
### <a name="delete-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="783fd-105">Удаление приложения из каталога приложений организации</span><span class="sxs-lookup"><span data-stu-id="783fd-105">Delete an app from your organization's app catalog</span></span>

<span data-ttu-id="783fd-106">Удаление [приложения из](../resources/teamsapp.md) каталога приложений организации (каталога приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="783fd-106">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="783fd-107">Чтобы удалить приложение, необходимо задать свойство **distributionMethod** для приложения `organization` .</span><span class="sxs-lookup"><span data-stu-id="783fd-107">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="783fd-108">Этот API также можно использовать для удаления отправленного приложения из процесса проверки.</span><span class="sxs-lookup"><span data-stu-id="783fd-108">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="783fd-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="783fd-109">Permissions</span></span>

<span data-ttu-id="783fd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="783fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="783fd-112">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="783fd-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="783fd-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="783fd-113">Permission Type</span></span>                        | <span data-ttu-id="783fd-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="783fd-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="783fd-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="783fd-115">Delegated (work or school account)</span></span> | <span data-ttu-id="783fd-116">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="783fd-116">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="783fd-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="783fd-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="783fd-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="783fd-118">Not supported</span></span>|
| <span data-ttu-id="783fd-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="783fd-119">Application</span></span>                            | <span data-ttu-id="783fd-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="783fd-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="783fd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="783fd-121">HTTP request</span></span>

<span data-ttu-id="783fd-122">Удаление приложения из каталога приложений:</span><span class="sxs-lookup"><span data-stu-id="783fd-122">To delete an app from the app catalog:</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="783fd-123">Удаление приложения, которое было отправлено, но не утверждено:</span><span class="sxs-lookup"><span data-stu-id="783fd-123">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="783fd-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="783fd-124">Request headers</span></span>

| <span data-ttu-id="783fd-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="783fd-125">Header</span></span>        | <span data-ttu-id="783fd-126">Значение</span><span class="sxs-lookup"><span data-stu-id="783fd-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="783fd-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="783fd-127">Authorization</span></span> | <span data-ttu-id="783fd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="783fd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="783fd-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="783fd-130">Request body</span></span>

<span data-ttu-id="783fd-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="783fd-131">Do not supply a request body for this method.</span></span>

><span data-ttu-id="783fd-132">**Примечание:** Используйте ID, возвращенный из вызова опубликованных приложений [Списка,](./appcatalogs-list-teamsapps.md) для ссылки на приложение, которое вы хотите удалить.</span><span class="sxs-lookup"><span data-stu-id="783fd-132">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="783fd-133">Не используйте ID из манифеста пакета почтовых приложений.</span><span class="sxs-lookup"><span data-stu-id="783fd-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="783fd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="783fd-134">Response</span></span>

<span data-ttu-id="783fd-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="783fd-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="783fd-137">Пример</span><span class="sxs-lookup"><span data-stu-id="783fd-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="783fd-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="783fd-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="783fd-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="783fd-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="783fd-140">C#</span><span class="sxs-lookup"><span data-stu-id="783fd-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="783fd-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="783fd-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="783fd-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="783fd-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="783fd-143">Java</span><span class="sxs-lookup"><span data-stu-id="783fd-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="783fd-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="783fd-144">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

