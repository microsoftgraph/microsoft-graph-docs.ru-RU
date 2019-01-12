---
title: Разрешения
description: 'Удаление приложения из каталога приложений организации (каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 58984044ea59bd38f0232bfa9407c01f97f22708
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943608"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="e9c1e-103">Удаление приложения из каталога приложений организации</span><span class="sxs-lookup"><span data-stu-id="e9c1e-103">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="e9c1e-104">Удаление [приложения](../resources/teamsapp.md) из каталога приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="e9c1e-104">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="e9c1e-105">Чтобы удалить приложение из каталога приложений вашей организации, укажите `organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e9c1e-105">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9c1e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9c1e-106">Permissions</span></span>

<span data-ttu-id="e9c1e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="e9c1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="e9c1e-109">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="e9c1e-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="e9c1e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9c1e-110">Permission Type</span></span>                        | <span data-ttu-id="e9c1e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9c1e-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="e9c1e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9c1e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9c1e-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9c1e-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="e9c1e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9c1e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9c1e-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9c1e-115">Not supported</span></span>|
| <span data-ttu-id="e9c1e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9c1e-116">Application</span></span>                            | <span data-ttu-id="e9c1e-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9c1e-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9c1e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9c1e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e9c1e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9c1e-119">Request headers</span></span>

| <span data-ttu-id="e9c1e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9c1e-120">Header</span></span>        | <span data-ttu-id="e9c1e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e9c1e-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="e9c1e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9c1e-122">Authorization</span></span> | <span data-ttu-id="e9c1e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9c1e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9c1e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9c1e-125">Request body</span></span>

<span data-ttu-id="e9c1e-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9c1e-126">None.</span></span>

><span data-ttu-id="e9c1e-127">**Примечание:** Используйте код, возвращенный вызова [списка публикации приложений](./teamsapp-list.md) для ссылок на приложением, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="e9c1e-127">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="e9c1e-128">Не используйте код из манифеста приложения ZIP-архив.</span><span class="sxs-lookup"><span data-stu-id="e9c1e-128">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="e9c1e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9c1e-129">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="e9c1e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e9c1e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9c1e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9c1e-131">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="e9c1e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9c1e-132">Response</span></span>

```http
HTTP/1.1 204 No Content
```
