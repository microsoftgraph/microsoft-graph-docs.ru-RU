---
title: Удаление educationSynchronizationProfile
description: Удаление профиля синхронизации данных school в клиентов на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d3c55cd90734fa78654baf10c940cd0debc57c50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976158"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="61319-103">Удаление educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="61319-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="61319-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="61319-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61319-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61319-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61319-106">Удаление данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="61319-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="61319-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61319-107">Permissions</span></span>
<span data-ttu-id="61319-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61319-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61319-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61319-110">Permission type</span></span> | <span data-ttu-id="61319-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61319-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="61319-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61319-112">Delegated (work or school account)</span></span> | <span data-ttu-id="61319-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61319-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="61319-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61319-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="61319-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61319-115">Request headers</span></span>
| <span data-ttu-id="61319-116">Имя</span><span class="sxs-lookup"><span data-stu-id="61319-116">Name</span></span>       | <span data-ttu-id="61319-117">Тип</span><span class="sxs-lookup"><span data-stu-id="61319-117">Type</span></span> | <span data-ttu-id="61319-118">Описание</span><span class="sxs-lookup"><span data-stu-id="61319-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="61319-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="61319-119">Authorization</span></span>  | <span data-ttu-id="61319-120">строка</span><span class="sxs-lookup"><span data-stu-id="61319-120">string</span></span>  | <span data-ttu-id="61319-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61319-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="61319-123">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="61319-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="61319-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61319-124">Not supported.</span></span>|
|<span data-ttu-id="61319-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61319-125">Application</span></span>|<span data-ttu-id="61319-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61319-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61319-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="61319-127">Request body</span></span>
<span data-ttu-id="61319-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61319-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="61319-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="61319-129">Response</span></span>
<span data-ttu-id="61319-130">При успешном выполнении этот метод возвращает код отклика `202 Accepted` и не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="61319-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="61319-131">Пример</span><span class="sxs-lookup"><span data-stu-id="61319-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61319-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="61319-132">Request</span></span>
<span data-ttu-id="61319-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61319-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="61319-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="61319-134">Response</span></span>
<span data-ttu-id="61319-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="61319-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
