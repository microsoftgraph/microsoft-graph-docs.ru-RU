---
title: Сброс синхронизации на educationSynchronizationProfile
description: Сброс синхронизации в конкретных школа профиль синхронизации данных клиента.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 54352d29280d671aaddc152307d8669f64c11bdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808542"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="c601f-103">Сброс синхронизации на educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="c601f-103">Reset sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="c601f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c601f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c601f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c601f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c601f-106">Сброс синхронизации данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="c601f-106">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="c601f-107">**Примечание:** Эта операция приводит к сбою синхронизации перезапустить.</span><span class="sxs-lookup"><span data-stu-id="c601f-107">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="c601f-108">Будут удалены все обнаруженные ошибки.</span><span class="sxs-lookup"><span data-stu-id="c601f-108">Any errors encountered will be deleted.</span></span> <span data-ttu-id="c601f-109">Данные не будут удалены из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c601f-109">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c601f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c601f-110">Permissions</span></span>
<span data-ttu-id="c601f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c601f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c601f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c601f-113">Permission type</span></span> | <span data-ttu-id="c601f-114">Permissions</span><span class="sxs-lookup"><span data-stu-id="c601f-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c601f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c601f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c601f-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c601f-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c601f-117">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c601f-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c601f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c601f-118">Not supported.</span></span>|
|<span data-ttu-id="c601f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c601f-119">Application</span></span>|<span data-ttu-id="c601f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c601f-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c601f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c601f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="c601f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c601f-122">Request headers</span></span>
| <span data-ttu-id="c601f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c601f-123">Name</span></span>       | <span data-ttu-id="c601f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c601f-124">Type</span></span> | <span data-ttu-id="c601f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c601f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c601f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c601f-126">Authorization</span></span>  | <span data-ttu-id="c601f-127">string</span><span class="sxs-lookup"><span data-stu-id="c601f-127">string</span></span>  | <span data-ttu-id="c601f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c601f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c601f-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c601f-130">Request body</span></span>
<span data-ttu-id="c601f-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c601f-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c601f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c601f-132">Response</span></span>
<span data-ttu-id="c601f-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c601f-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c601f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c601f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c601f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c601f-135">Request</span></span>
<span data-ttu-id="c601f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c601f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="c601f-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c601f-137">Response</span></span>

<span data-ttu-id="c601f-138">Нет тело ответа отсутствует.</span><span class="sxs-lookup"><span data-stu-id="c601f-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
