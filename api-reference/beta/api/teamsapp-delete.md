---
title: Удаление teamsApp
description: 'Удаление приложения Teams из каталога приложений организации (Каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bbc8d0962a1b03d9b113fd81f8bb3ae49655dcb1
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606813"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="8b329-103">Удаление teamsApp</span><span class="sxs-lookup"><span data-stu-id="8b329-103">Delete teamsApp</span></span>

<span data-ttu-id="8b329-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b329-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

<span data-ttu-id="8b329-105">Удаление [приложения](../resources/teamsapp.md) из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="8b329-105">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="8b329-106">Чтобы удалить приложение, свойство **distributionMethod** для приложения должно иметь значение `organization` .</span><span class="sxs-lookup"><span data-stu-id="8b329-106">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="8b329-107">Вы также можете использовать этот API для удаления отправленного приложения из процесса проверки.</span><span class="sxs-lookup"><span data-stu-id="8b329-107">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b329-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b329-108">Permissions</span></span>

<span data-ttu-id="8b329-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b329-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="8b329-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8b329-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="8b329-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b329-112">Permission Type</span></span>                        | <span data-ttu-id="8b329-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b329-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="8b329-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b329-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8b329-115">CamlQuery. оправить, CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8b329-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="8b329-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b329-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b329-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b329-117">Not supported.</span></span>|
| <span data-ttu-id="8b329-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b329-118">Application</span></span>                            | <span data-ttu-id="8b329-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b329-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b329-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b329-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="8b329-121">Удаление приложения из каталога приложений:</span><span class="sxs-lookup"><span data-stu-id="8b329-121">To delete an app from the app catalog:</span></span>

```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="8b329-122">Чтобы удалить приложение, которое было отправлено, но еще не утверждено:</span><span class="sxs-lookup"><span data-stu-id="8b329-122">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="8b329-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b329-123">Request headers</span></span>

| <span data-ttu-id="8b329-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b329-124">Header</span></span>        | <span data-ttu-id="8b329-125">Значение</span><span class="sxs-lookup"><span data-stu-id="8b329-125">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="8b329-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b329-126">Authorization</span></span> | <span data-ttu-id="8b329-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b329-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b329-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b329-129">Request body</span></span>

<span data-ttu-id="8b329-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b329-130">Do not supply a request body for this method.</span></span>

><span data-ttu-id="8b329-131">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./appcatalogs-list-teamsapps.md) , для ссылки на приложение, которое вы хотите удалить.</span><span class="sxs-lookup"><span data-stu-id="8b329-131">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="8b329-132">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="8b329-132">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="8b329-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b329-133">Response</span></span>

<span data-ttu-id="8b329-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b329-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b329-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8b329-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b329-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b329-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8b329-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b329-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="8b329-139">C#</span><span class="sxs-lookup"><span data-stu-id="8b329-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b329-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b329-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b329-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b329-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b329-142">Java</span><span class="sxs-lookup"><span data-stu-id="8b329-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="8b329-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b329-143">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
