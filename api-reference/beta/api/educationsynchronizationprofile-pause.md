---
title: Приостановка синхронизации на educationSynchronizationProfile
description: Приостановка синхронизации в конкретных школа профиль синхронизации данных клиента.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4979ed19c9a01d6a7ff2d43f7f3755d03b4b070c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950685"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="03221-103">Приостановка синхронизации на educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="03221-103">Pause sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="03221-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03221-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03221-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03221-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03221-106">Приостановка синхронизации данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="03221-106">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="03221-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03221-107">Permissions</span></span>
<span data-ttu-id="03221-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03221-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03221-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03221-110">Permission type</span></span> | <span data-ttu-id="03221-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03221-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="03221-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03221-112">Delegated (work or school account)</span></span> | <span data-ttu-id="03221-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03221-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="03221-114">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="03221-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="03221-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03221-115">Not supported.</span></span>|
|<span data-ttu-id="03221-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03221-116">Application</span></span>|<span data-ttu-id="03221-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03221-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03221-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03221-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="03221-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03221-119">Request headers</span></span>
| <span data-ttu-id="03221-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03221-120">Name</span></span>       | <span data-ttu-id="03221-121">Тип</span><span class="sxs-lookup"><span data-stu-id="03221-121">Type</span></span> | <span data-ttu-id="03221-122">Описание</span><span class="sxs-lookup"><span data-stu-id="03221-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="03221-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03221-123">Authorization</span></span>  | <span data-ttu-id="03221-124">строка</span><span class="sxs-lookup"><span data-stu-id="03221-124">string</span></span>  | <span data-ttu-id="03221-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03221-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03221-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03221-127">Request body</span></span>
<span data-ttu-id="03221-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03221-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="03221-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="03221-129">Response</span></span>
<span data-ttu-id="03221-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="03221-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="03221-131">Пример</span><span class="sxs-lookup"><span data-stu-id="03221-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03221-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="03221-132">Request</span></span>
<span data-ttu-id="03221-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03221-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="03221-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="03221-134">Response</span></span>

<span data-ttu-id="03221-135">Нет тело ответа отсутствует.</span><span class="sxs-lookup"><span data-stu-id="03221-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
