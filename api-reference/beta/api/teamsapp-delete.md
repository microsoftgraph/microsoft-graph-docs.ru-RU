---
title: Удаление teamsApp
description: 'Удалите Teams приложения из каталога приложений организации (каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 34e9e7a1f8e98eda66bf34950c9d7f0b9cac7d6e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786701"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="c3677-103">Удаление teamsApp</span><span class="sxs-lookup"><span data-stu-id="c3677-103">Delete teamsApp</span></span>

<span data-ttu-id="c3677-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3677-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

<span data-ttu-id="c3677-105">Удаление [приложения из](../resources/teamsapp.md) каталога приложений организации (каталога приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="c3677-105">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="c3677-106">Чтобы удалить приложение, необходимо задать свойство **distributionMethod** для приложения `organization` .</span><span class="sxs-lookup"><span data-stu-id="c3677-106">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="c3677-107">Этот API также можно использовать для удаления отправленного приложения из процесса проверки.</span><span class="sxs-lookup"><span data-stu-id="c3677-107">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3677-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3677-108">Permissions</span></span>

<span data-ttu-id="c3677-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3677-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="c3677-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c3677-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="c3677-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3677-112">Permission Type</span></span>                        | <span data-ttu-id="c3677-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3677-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="c3677-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3677-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c3677-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3677-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c3677-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3677-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3677-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3677-117">Not supported.</span></span>|
| <span data-ttu-id="c3677-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3677-118">Application</span></span>                            | <span data-ttu-id="c3677-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3677-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3677-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3677-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="c3677-121">Удаление приложения из каталога приложений:</span><span class="sxs-lookup"><span data-stu-id="c3677-121">To delete an app from the app catalog:</span></span>

```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="c3677-122">Удаление приложения, которое было отправлено, но не утверждено:</span><span class="sxs-lookup"><span data-stu-id="c3677-122">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="c3677-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3677-123">Request headers</span></span>

| <span data-ttu-id="c3677-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3677-124">Header</span></span>        | <span data-ttu-id="c3677-125">Значение</span><span class="sxs-lookup"><span data-stu-id="c3677-125">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="c3677-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3677-126">Authorization</span></span> | <span data-ttu-id="c3677-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3677-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3677-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3677-129">Request body</span></span>

<span data-ttu-id="c3677-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3677-130">Do not supply a request body for this method.</span></span>

><span data-ttu-id="c3677-131">**Примечание:** Используйте ID, возвращенный из вызова опубликованных приложений [Списка,](./appcatalogs-list-teamsapps.md) для ссылки на приложение, которое вы хотите удалить.</span><span class="sxs-lookup"><span data-stu-id="c3677-131">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="c3677-132">Не используйте ID из манифеста пакета почтовых приложений.</span><span class="sxs-lookup"><span data-stu-id="c3677-132">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="c3677-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3677-133">Response</span></span>

<span data-ttu-id="c3677-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c3677-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3677-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c3677-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3677-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3677-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c3677-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3677-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="c3677-139">C#</span><span class="sxs-lookup"><span data-stu-id="c3677-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3677-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3677-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3677-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3677-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3677-142">Java</span><span class="sxs-lookup"><span data-stu-id="c3677-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="c3677-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3677-143">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
