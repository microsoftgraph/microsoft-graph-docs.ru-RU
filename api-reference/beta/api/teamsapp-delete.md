---
title: Разрешения
description: 'Удалите приложение из каталога приложений организации (Каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 35a131309445f0a84bdc54690e1f88b5a0ad31f0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335236"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="9a845-103">Удаление приложения из каталога приложений Организации</span><span class="sxs-lookup"><span data-stu-id="9a845-103">Remove an app from your organization's app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a845-104">Удалите [приложение](../resources/teamsapp.md) из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="9a845-104">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="9a845-105">Чтобы удалить приложение из каталога приложений вашей организации, укажите `organization` в качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9a845-105">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a845-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a845-106">Permissions</span></span>

<span data-ttu-id="9a845-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="9a845-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="9a845-109">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9a845-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="9a845-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a845-110">Permission Type</span></span>                        | <span data-ttu-id="9a845-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a845-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="9a845-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a845-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a845-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a845-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="9a845-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a845-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a845-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9a845-115">Not supported</span></span>|
| <span data-ttu-id="9a845-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a845-116">Application</span></span>                            | <span data-ttu-id="9a845-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9a845-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a845-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a845-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9a845-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a845-119">Request headers</span></span>

| <span data-ttu-id="9a845-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a845-120">Header</span></span>        | <span data-ttu-id="9a845-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9a845-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="9a845-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a845-122">Authorization</span></span> | <span data-ttu-id="9a845-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a845-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a845-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a845-125">Request body</span></span>

<span data-ttu-id="9a845-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9a845-126">None.</span></span>

><span data-ttu-id="9a845-127">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="9a845-127">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="9a845-128">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="9a845-128">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="9a845-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a845-129">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="9a845-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9a845-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a845-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a845-131">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="9a845-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a845-132">Response</span></span>

```http
HTTP/1.1 204 No Content
```
