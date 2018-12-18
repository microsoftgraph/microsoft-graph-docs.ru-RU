---
title: Удаление educationSynchronizationProfile
description: Удаление профиля синхронизации данных school в клиентов на основе идентификатора.
author: mmast-msft
ms.openlocfilehash: b0287133d579915279e0f9a02bf49dd981ccf419
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343304"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="b9908-103">Удаление educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="b9908-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="b9908-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9908-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9908-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9908-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9908-106">Удаление данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="b9908-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9908-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9908-107">Permissions</span></span>
<span data-ttu-id="b9908-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9908-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9908-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9908-110">Permission type</span></span> | <span data-ttu-id="b9908-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9908-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="b9908-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9908-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9908-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9908-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9908-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9908-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b9908-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9908-115">Request headers</span></span>
| <span data-ttu-id="b9908-116">Имя</span><span class="sxs-lookup"><span data-stu-id="b9908-116">Name</span></span>       | <span data-ttu-id="b9908-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b9908-117">Type</span></span> | <span data-ttu-id="b9908-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b9908-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b9908-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9908-119">Authorization</span></span>  | <span data-ttu-id="b9908-120">string</span><span class="sxs-lookup"><span data-stu-id="b9908-120">string</span></span>  | <span data-ttu-id="b9908-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9908-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="b9908-123">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="b9908-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b9908-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9908-124">Not supported.</span></span>|
|<span data-ttu-id="b9908-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9908-125">Application</span></span>|<span data-ttu-id="b9908-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9908-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9908-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9908-127">Request body</span></span>
<span data-ttu-id="b9908-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9908-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b9908-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9908-129">Response</span></span>
<span data-ttu-id="b9908-130">При успешном выполнении этот метод возвращает код отклика `202 Accepted` и не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="b9908-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9908-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b9908-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9908-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9908-132">Request</span></span>
<span data-ttu-id="b9908-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9908-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="b9908-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9908-134">Response</span></span>
<span data-ttu-id="b9908-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9908-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
