---
title: Удаление teamsApp
description: 'Удаление приложения Teams из каталога приложений организации (Каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 29d4f2c18132288b65407bbe75b8d622edd69d96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978438"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="4da2f-103">Удаление teamsApp</span><span class="sxs-lookup"><span data-stu-id="4da2f-103">Delete teamsApp</span></span>

<span data-ttu-id="4da2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4da2f-104">Namespace: microsoft.graph</span></span>

<!-- markdownlint-disable MD001 -->
### <a name="delete-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="4da2f-105">Удаление приложения из каталога приложений Организации</span><span class="sxs-lookup"><span data-stu-id="4da2f-105">Delete an app from your organization's app catalog</span></span>

<span data-ttu-id="4da2f-106">Удаление [приложения](../resources/teamsapp.md) из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="4da2f-106">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="4da2f-107">Чтобы удалить приложение, свойство **distributionMethod** для приложения должно иметь значение `organization` .</span><span class="sxs-lookup"><span data-stu-id="4da2f-107">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="4da2f-108">Вы также можете использовать этот API для удаления отправленного приложения из процесса проверки.</span><span class="sxs-lookup"><span data-stu-id="4da2f-108">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="4da2f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4da2f-109">Permissions</span></span>

<span data-ttu-id="4da2f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4da2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="4da2f-112">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4da2f-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="4da2f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4da2f-113">Permission Type</span></span>                        | <span data-ttu-id="4da2f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4da2f-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="4da2f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4da2f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="4da2f-116">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4da2f-116">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="4da2f-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4da2f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4da2f-118">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="4da2f-118">AppCatalog.Submit</span></span> |
| <span data-ttu-id="4da2f-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4da2f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4da2f-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4da2f-120">Not supported</span></span>|
| <span data-ttu-id="4da2f-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4da2f-121">Application</span></span>                            | <span data-ttu-id="4da2f-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da2f-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4da2f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4da2f-123">HTTP request</span></span>

<span data-ttu-id="4da2f-124">Удаление приложения из каталога приложений:</span><span class="sxs-lookup"><span data-stu-id="4da2f-124">To delete an app from the app catalog:</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="4da2f-125">Чтобы удалить приложение, которое было отправлено, но еще не утверждено:</span><span class="sxs-lookup"><span data-stu-id="4da2f-125">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="4da2f-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4da2f-126">Request headers</span></span>

| <span data-ttu-id="4da2f-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4da2f-127">Header</span></span>        | <span data-ttu-id="4da2f-128">Значение</span><span class="sxs-lookup"><span data-stu-id="4da2f-128">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="4da2f-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4da2f-129">Authorization</span></span> | <span data-ttu-id="4da2f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4da2f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4da2f-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4da2f-132">Request body</span></span>

<span data-ttu-id="4da2f-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4da2f-133">Do not supply a request body for this method.</span></span>

><span data-ttu-id="4da2f-134">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="4da2f-134">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="4da2f-135">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="4da2f-135">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="4da2f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4da2f-136">Response</span></span>

<span data-ttu-id="4da2f-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4da2f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4da2f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="4da2f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="4da2f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4da2f-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4da2f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="4da2f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="4da2f-142">C#</span><span class="sxs-lookup"><span data-stu-id="4da2f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4da2f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4da2f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4da2f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4da2f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4da2f-145">Java</span><span class="sxs-lookup"><span data-stu-id="4da2f-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="4da2f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4da2f-146">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

