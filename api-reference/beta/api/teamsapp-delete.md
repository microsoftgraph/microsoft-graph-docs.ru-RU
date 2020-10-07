---
title: Удаление teamsApp
description: 'Удаление приложения Teams из каталога приложений организации (Каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eb4704b3e4febe31271dc52f2e4905f28db9495e
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373673"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="ea12e-103">Удаление teamsApp</span><span class="sxs-lookup"><span data-stu-id="ea12e-103">Delete teamsApp</span></span>

<span data-ttu-id="ea12e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea12e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

<span data-ttu-id="ea12e-105">Удаление [приложения](../resources/teamsapp.md) из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="ea12e-105">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="ea12e-106">Чтобы удалить приложение, свойство **distributionMethod** для приложения должно иметь значение `organization` .</span><span class="sxs-lookup"><span data-stu-id="ea12e-106">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="ea12e-107">Вы также можете использовать этот API для удаления отправленного приложения из процесса проверки.</span><span class="sxs-lookup"><span data-stu-id="ea12e-107">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea12e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea12e-108">Permissions</span></span>

<span data-ttu-id="ea12e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea12e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="ea12e-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ea12e-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="ea12e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea12e-112">Permission Type</span></span>                        | <span data-ttu-id="ea12e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea12e-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="ea12e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea12e-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea12e-115">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ea12e-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="ea12e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea12e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ea12e-117">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="ea12e-117">AppCatalog.Submit</span></span> |
| <span data-ttu-id="ea12e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea12e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea12e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea12e-119">Not supported.</span></span>|
| <span data-ttu-id="ea12e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea12e-120">Application</span></span>                            | <span data-ttu-id="ea12e-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea12e-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea12e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea12e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="ea12e-123">Удаление приложения из каталога приложений:</span><span class="sxs-lookup"><span data-stu-id="ea12e-123">To delete an app from the app catalog:</span></span>

```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="ea12e-124">Чтобы удалить приложение, которое было отправлено, но еще не утверждено:</span><span class="sxs-lookup"><span data-stu-id="ea12e-124">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="ea12e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea12e-125">Request headers</span></span>

| <span data-ttu-id="ea12e-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea12e-126">Header</span></span>        | <span data-ttu-id="ea12e-127">Значение</span><span class="sxs-lookup"><span data-stu-id="ea12e-127">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="ea12e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea12e-128">Authorization</span></span> | <span data-ttu-id="ea12e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea12e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea12e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea12e-131">Request body</span></span>

<span data-ttu-id="ea12e-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea12e-132">Do not supply a request body for this method.</span></span>

><span data-ttu-id="ea12e-133">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите удалить.</span><span class="sxs-lookup"><span data-stu-id="ea12e-133">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="ea12e-134">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="ea12e-134">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="ea12e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea12e-135">Response</span></span>

<span data-ttu-id="ea12e-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ea12e-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea12e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ea12e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea12e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea12e-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ea12e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea12e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="ea12e-141">C#</span><span class="sxs-lookup"><span data-stu-id="ea12e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea12e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea12e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea12e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea12e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="ea12e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea12e-144">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
