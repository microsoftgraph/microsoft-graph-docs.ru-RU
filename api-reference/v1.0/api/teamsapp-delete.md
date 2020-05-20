---
title: Разрешения
description: 'Удалите приложение из каталога приложений организации (Каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3d224b0458a26b35ba330c508eeac65bea2b068f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290330"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="3ea25-103">Удаление приложения из каталога приложений Организации</span><span class="sxs-lookup"><span data-stu-id="3ea25-103">Remove an app from your organization's app catalog</span></span>

<span data-ttu-id="3ea25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ea25-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="3ea25-105">Удалите [приложение](../resources/teamsapp.md) из каталога приложений организации (Каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="3ea25-105">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="3ea25-106">Чтобы удалить приложение из каталога приложений вашей организации, укажите в `organization` качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3ea25-106">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ea25-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea25-107">Permissions</span></span>

<span data-ttu-id="3ea25-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="3ea25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="3ea25-110">**Примечание:** Только глобальные администраторы могут вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3ea25-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="3ea25-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea25-111">Permission Type</span></span>                        | <span data-ttu-id="3ea25-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ea25-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="3ea25-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ea25-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ea25-114">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3ea25-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3ea25-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ea25-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ea25-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3ea25-116">Not supported</span></span>|
| <span data-ttu-id="3ea25-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ea25-117">Application</span></span>                            | <span data-ttu-id="3ea25-118">CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3ea25-118">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ea25-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ea25-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3ea25-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ea25-120">Request headers</span></span>

| <span data-ttu-id="3ea25-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ea25-121">Header</span></span>        | <span data-ttu-id="3ea25-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3ea25-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="3ea25-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ea25-123">Authorization</span></span> | <span data-ttu-id="3ea25-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ea25-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ea25-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ea25-126">Request body</span></span>

<span data-ttu-id="3ea25-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3ea25-127">None.</span></span>

><span data-ttu-id="3ea25-128">**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="3ea25-128">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="3ea25-129">Не используйте идентификатор из манифеста пакета приложения ZIP.</span><span class="sxs-lookup"><span data-stu-id="3ea25-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="3ea25-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea25-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="3ea25-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3ea25-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ea25-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea25-132">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="3ea25-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea25-133">Response</span></span>

```http
HTTP/1.1 204 No Content
```
