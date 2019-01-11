---
title: Удаление educationSynchronizationProfile
description: Удаление профиля синхронизации данных school в клиентов на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 09cc19b22cfa433cef39c81a6cbeadeddcf52ace
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870366"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="4252b-103">Удаление educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="4252b-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="4252b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4252b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4252b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4252b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4252b-106">Удаление данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="4252b-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="4252b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4252b-107">Permissions</span></span>
<span data-ttu-id="4252b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4252b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4252b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4252b-110">Permission type</span></span> | <span data-ttu-id="4252b-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="4252b-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4252b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4252b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4252b-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4252b-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4252b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4252b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4252b-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4252b-115">Request headers</span></span>
| <span data-ttu-id="4252b-116">Имя</span><span class="sxs-lookup"><span data-stu-id="4252b-116">Name</span></span>       | <span data-ttu-id="4252b-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4252b-117">Type</span></span> | <span data-ttu-id="4252b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4252b-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4252b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4252b-119">Authorization</span></span>  | <span data-ttu-id="4252b-120">string</span><span class="sxs-lookup"><span data-stu-id="4252b-120">string</span></span>  | <span data-ttu-id="4252b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4252b-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="4252b-123">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="4252b-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4252b-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4252b-124">Not supported.</span></span>|
|<span data-ttu-id="4252b-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4252b-125">Application</span></span>|<span data-ttu-id="4252b-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4252b-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4252b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4252b-127">Request body</span></span>
<span data-ttu-id="4252b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4252b-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4252b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4252b-129">Response</span></span>
<span data-ttu-id="4252b-130">При успешном выполнении этот метод возвращает код отклика `202 Accepted` и не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="4252b-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="4252b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4252b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4252b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4252b-132">Request</span></span>
<span data-ttu-id="4252b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4252b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="4252b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4252b-134">Response</span></span>
<span data-ttu-id="4252b-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4252b-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
