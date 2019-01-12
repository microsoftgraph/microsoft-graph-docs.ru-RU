---
title: Permissions
description: 'Удаление приложения из каталога приложений организации (каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: bce53c91d498a36405f44ffa13827cdeb40c074e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953718"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="7cab0-103">Удаление приложения из каталога приложений организации</span><span class="sxs-lookup"><span data-stu-id="7cab0-103">Remove an app from your organization's app catalog</span></span>

> <span data-ttu-id="7cab0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7cab0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cab0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cab0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7cab0-106">Удаление [приложения](../resources/teamsapp.md) из каталога приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="7cab0-106">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="7cab0-107">Чтобы удалить приложение из каталога приложений вашей организации, укажите `organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7cab0-107">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cab0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cab0-108">Permissions</span></span>

<span data-ttu-id="7cab0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7cab0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="7cab0-111">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="7cab0-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="7cab0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cab0-112">Permission Type</span></span>                        | <span data-ttu-id="7cab0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cab0-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="7cab0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cab0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7cab0-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cab0-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="7cab0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cab0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cab0-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7cab0-117">Not supported</span></span>|
| <span data-ttu-id="7cab0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cab0-118">Application</span></span>                            | <span data-ttu-id="7cab0-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7cab0-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cab0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cab0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7cab0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cab0-121">Request headers</span></span>

| <span data-ttu-id="7cab0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7cab0-122">Header</span></span>        | <span data-ttu-id="7cab0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7cab0-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="7cab0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7cab0-124">Authorization</span></span> | <span data-ttu-id="7cab0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cab0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7cab0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7cab0-127">Request body</span></span>

<span data-ttu-id="7cab0-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="7cab0-128">None.</span></span>

><span data-ttu-id="7cab0-129">**Примечание:** Используйте код, возвращенный вызова [списка публикации приложений](./teamsapp-list.md) для ссылок на приложением, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="7cab0-129">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="7cab0-130">Не используйте код из манифеста приложения ZIP-архив.</span><span class="sxs-lookup"><span data-stu-id="7cab0-130">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="7cab0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cab0-131">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="7cab0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7cab0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cab0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cab0-133">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="7cab0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cab0-134">Response</span></span>

```http
HTTP/1.1 204 No Content
```
