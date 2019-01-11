---
title: Возобновление синхронизации на educationSynchronizationProfile
description: Возобновление синхронизации в конкретных школа профиль синхронизации данных клиента.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: c68fb6d042d92fd0f1334dc498b175c27cbc4ced
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894210"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="e173a-103">Возобновление синхронизации на educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="e173a-103">Resume sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="e173a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e173a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e173a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e173a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e173a-106">Возобновление синхронизации данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="e173a-106">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e173a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e173a-107">Permissions</span></span>
<span data-ttu-id="e173a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e173a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e173a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e173a-110">Permission type</span></span> | <span data-ttu-id="e173a-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e173a-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e173a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e173a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e173a-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e173a-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e173a-114">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="e173a-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e173a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e173a-115">Not supported.</span></span>|
|<span data-ttu-id="e173a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e173a-116">Application</span></span>|<span data-ttu-id="e173a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e173a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e173a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e173a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="e173a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e173a-119">Request headers</span></span>
| <span data-ttu-id="e173a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e173a-120">Name</span></span>       | <span data-ttu-id="e173a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e173a-121">Type</span></span> | <span data-ttu-id="e173a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e173a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e173a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e173a-123">Authorization</span></span>  | <span data-ttu-id="e173a-124">string</span><span class="sxs-lookup"><span data-stu-id="e173a-124">string</span></span>  | <span data-ttu-id="e173a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e173a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e173a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e173a-127">Request body</span></span>
<span data-ttu-id="e173a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e173a-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e173a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e173a-129">Response</span></span>
<span data-ttu-id="e173a-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e173a-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e173a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e173a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e173a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e173a-132">Request</span></span>
<span data-ttu-id="e173a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e173a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="e173a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e173a-134">Response</span></span>

<span data-ttu-id="e173a-135">Нет тело ответа отсутствует.</span><span class="sxs-lookup"><span data-stu-id="e173a-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
