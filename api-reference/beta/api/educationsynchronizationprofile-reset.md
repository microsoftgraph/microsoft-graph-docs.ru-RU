---
title: Сброс синхронизации на educationSynchronizationProfile
description: Сброс синхронизации в конкретных школа профиль синхронизации данных клиента.
author: mmast-msft
ms.openlocfilehash: 29d21318737ceba3bd380eaf20a9500a6a711857
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362442"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="6b331-103">Сброс синхронизации на educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="6b331-103">Reset sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="6b331-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6b331-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b331-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b331-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b331-106">Сброс синхронизации данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="6b331-106">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="6b331-107">**Примечание:** Эта операция приводит к сбою синхронизации перезапустить.</span><span class="sxs-lookup"><span data-stu-id="6b331-107">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="6b331-108">Будут удалены все обнаруженные ошибки.</span><span class="sxs-lookup"><span data-stu-id="6b331-108">Any errors encountered will be deleted.</span></span> <span data-ttu-id="6b331-109">Данные не будут удалены из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="6b331-109">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="6b331-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b331-110">Permissions</span></span>
<span data-ttu-id="6b331-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b331-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b331-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b331-113">Permission type</span></span> | <span data-ttu-id="6b331-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b331-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="6b331-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b331-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6b331-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b331-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="6b331-117">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="6b331-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6b331-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b331-118">Not supported.</span></span>|
|<span data-ttu-id="6b331-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b331-119">Application</span></span>|<span data-ttu-id="6b331-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b331-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b331-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b331-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="6b331-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b331-122">Request headers</span></span>
| <span data-ttu-id="6b331-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6b331-123">Name</span></span>       | <span data-ttu-id="6b331-124">Тип</span><span class="sxs-lookup"><span data-stu-id="6b331-124">Type</span></span> | <span data-ttu-id="6b331-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6b331-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6b331-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b331-126">Authorization</span></span>  | <span data-ttu-id="6b331-127">string</span><span class="sxs-lookup"><span data-stu-id="6b331-127">string</span></span>  | <span data-ttu-id="6b331-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b331-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b331-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b331-130">Request body</span></span>
<span data-ttu-id="6b331-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b331-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6b331-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b331-132">Response</span></span>
<span data-ttu-id="6b331-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="6b331-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6b331-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6b331-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b331-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b331-135">Request</span></span>
<span data-ttu-id="6b331-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b331-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="6b331-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b331-137">Response</span></span>

<span data-ttu-id="6b331-138">Нет тело ответа отсутствует.</span><span class="sxs-lookup"><span data-stu-id="6b331-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```