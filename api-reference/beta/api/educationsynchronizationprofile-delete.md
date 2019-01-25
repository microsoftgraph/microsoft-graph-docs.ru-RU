---
title: Удаление educationSynchronizationProfile
description: Удаление профиля синхронизации данных school в клиентов на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2aaa0d47bcc98c814ad525deb781ac7a7df28d87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512474"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="178ab-103">Удаление educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="178ab-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="178ab-104">Удаление данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="178ab-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="178ab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="178ab-105">Permissions</span></span>
<span data-ttu-id="178ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="178ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="178ab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="178ab-108">Permission type</span></span> | <span data-ttu-id="178ab-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="178ab-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="178ab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="178ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="178ab-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="178ab-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="178ab-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="178ab-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="178ab-113">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="178ab-113">Request headers</span></span>
| <span data-ttu-id="178ab-114">Имя</span><span class="sxs-lookup"><span data-stu-id="178ab-114">Name</span></span>       | <span data-ttu-id="178ab-115">Тип</span><span class="sxs-lookup"><span data-stu-id="178ab-115">Type</span></span> | <span data-ttu-id="178ab-116">Описание</span><span class="sxs-lookup"><span data-stu-id="178ab-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="178ab-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="178ab-117">Authorization</span></span>  | <span data-ttu-id="178ab-118">string</span><span class="sxs-lookup"><span data-stu-id="178ab-118">string</span></span>  | <span data-ttu-id="178ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="178ab-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="178ab-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="178ab-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="178ab-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="178ab-122">Not supported.</span></span>|
|<span data-ttu-id="178ab-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="178ab-123">Application</span></span>|<span data-ttu-id="178ab-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="178ab-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="178ab-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="178ab-125">Request body</span></span>
<span data-ttu-id="178ab-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="178ab-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="178ab-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="178ab-127">Response</span></span>
<span data-ttu-id="178ab-128">При успешном выполнении этот метод возвращает код отклика `202 Accepted` и не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="178ab-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="178ab-129">Пример</span><span class="sxs-lookup"><span data-stu-id="178ab-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="178ab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="178ab-130">Request</span></span>
<span data-ttu-id="178ab-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="178ab-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="178ab-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="178ab-132">Response</span></span>
<span data-ttu-id="178ab-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="178ab-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
