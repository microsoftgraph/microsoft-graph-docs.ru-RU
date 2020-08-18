---
title: Удаление teamsApp
description: 'Удаление приложения Teams из каталога приложений организации (Каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 432af0167562d34ca006b05901ad5fcb7529a51c
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790499"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="9787f-103">Удаление teamsApp</span><span class="sxs-lookup"><span data-stu-id="9787f-103">Delete teamsApp</span></span>

<span data-ttu-id="9787f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9787f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

<span data-ttu-id="9787f-105">Удаление [приложения](../resources/teamsapp.md) из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="9787f-105">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="9787f-106">Чтобы удалить приложение, свойство **distributionMethod** для приложения должно иметь значение `organization` .</span><span class="sxs-lookup"><span data-stu-id="9787f-106">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="9787f-107">Вы также можете использовать этот API для удаления отправленного приложения из процесса проверки.</span><span class="sxs-lookup"><span data-stu-id="9787f-107">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="9787f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9787f-108">Permissions</span></span>

<span data-ttu-id="9787f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="9787f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="9787f-111">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9787f-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="9787f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9787f-112">Permission Type</span></span>                        | <span data-ttu-id="9787f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9787f-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="9787f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9787f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="9787f-115">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9787f-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="9787f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9787f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9787f-117">CamlQuery. оправить</span><span class="sxs-lookup"><span data-stu-id="9787f-117">AppCatalog.Submit</span></span> |
| <span data-ttu-id="9787f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9787f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9787f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9787f-119">Not supported.</span></span>|
| <span data-ttu-id="9787f-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9787f-120">Application</span></span>                            | <span data-ttu-id="9787f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9787f-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9787f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9787f-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="9787f-123">Удаление приложения из каталога приложений:</span><span class="sxs-lookup"><span data-stu-id="9787f-123">To delete an app from the app catalog:</span></span>

```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="9787f-124">Чтобы удалить приложение, которое было отправлено, но еще не утверждено:</span><span class="sxs-lookup"><span data-stu-id="9787f-124">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="9787f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9787f-125">Request headers</span></span>

| <span data-ttu-id="9787f-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9787f-126">Header</span></span>        | <span data-ttu-id="9787f-127">Значение</span><span class="sxs-lookup"><span data-stu-id="9787f-127">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="9787f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9787f-128">Authorization</span></span> | <span data-ttu-id="9787f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9787f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9787f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9787f-131">Request body</span></span>

<span data-ttu-id="9787f-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9787f-132">Do not supply a request body for this method.</span></span>

><span data-ttu-id="9787f-133">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите удалить.</span><span class="sxs-lookup"><span data-stu-id="9787f-133">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="9787f-134">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="9787f-134">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="9787f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9787f-135">Response</span></span>

<span data-ttu-id="9787f-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9787f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9787f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9787f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9787f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9787f-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="9787f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9787f-140">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
