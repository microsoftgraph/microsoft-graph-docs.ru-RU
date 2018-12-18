---
title: Возобновление синхронизации на educationSynchronizationProfile
description: Возобновление синхронизации в конкретных школа профиль синхронизации данных клиента.
author: mmast-msft
ms.openlocfilehash: fd148db59d34f6455ba01e721453972f9cf65be4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305651"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="ff35e-103">Возобновление синхронизации на educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="ff35e-103">Resume sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="ff35e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff35e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff35e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff35e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff35e-106">Возобновление синхронизации данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="ff35e-106">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff35e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff35e-107">Permissions</span></span>
<span data-ttu-id="ff35e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff35e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff35e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff35e-110">Permission type</span></span> | <span data-ttu-id="ff35e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff35e-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ff35e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff35e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff35e-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff35e-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ff35e-114">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="ff35e-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ff35e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff35e-115">Not supported.</span></span>|
|<span data-ttu-id="ff35e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff35e-116">Application</span></span>|<span data-ttu-id="ff35e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff35e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff35e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff35e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="ff35e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff35e-119">Request headers</span></span>
| <span data-ttu-id="ff35e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ff35e-120">Name</span></span>       | <span data-ttu-id="ff35e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ff35e-121">Type</span></span> | <span data-ttu-id="ff35e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ff35e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ff35e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff35e-123">Authorization</span></span>  | <span data-ttu-id="ff35e-124">string</span><span class="sxs-lookup"><span data-stu-id="ff35e-124">string</span></span>  | <span data-ttu-id="ff35e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff35e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff35e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff35e-127">Request body</span></span>
<span data-ttu-id="ff35e-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff35e-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ff35e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff35e-129">Response</span></span>
<span data-ttu-id="ff35e-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="ff35e-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff35e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ff35e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff35e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff35e-132">Request</span></span>
<span data-ttu-id="ff35e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff35e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="ff35e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff35e-134">Response</span></span>

<span data-ttu-id="ff35e-135">Нет тело ответа отсутствует.</span><span class="sxs-lookup"><span data-stu-id="ff35e-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```