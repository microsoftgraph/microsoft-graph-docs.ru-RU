---
title: Удаление Едукатионсинчронизатионпрофиле
description: Удалите профиль School Data Synchronization в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2aaa0d47bcc98c814ad525deb781ac7a7df28d87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457454"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="327fc-103">Удаление Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="327fc-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="327fc-104">Удалите профиль School Data [Synchronization](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="327fc-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="327fc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="327fc-105">Permissions</span></span>
<span data-ttu-id="327fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="327fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="327fc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="327fc-108">Permission type</span></span> | <span data-ttu-id="327fc-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="327fc-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="327fc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="327fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="327fc-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="327fc-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="327fc-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="327fc-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="327fc-113">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="327fc-113">Request headers</span></span>
| <span data-ttu-id="327fc-114">Имя</span><span class="sxs-lookup"><span data-stu-id="327fc-114">Name</span></span>       | <span data-ttu-id="327fc-115">Тип</span><span class="sxs-lookup"><span data-stu-id="327fc-115">Type</span></span> | <span data-ttu-id="327fc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="327fc-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="327fc-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="327fc-117">Authorization</span></span>  | <span data-ttu-id="327fc-118">string</span><span class="sxs-lookup"><span data-stu-id="327fc-118">string</span></span>  | <span data-ttu-id="327fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="327fc-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="327fc-121">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="327fc-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="327fc-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="327fc-122">Not supported.</span></span>|
|<span data-ttu-id="327fc-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="327fc-123">Application</span></span>|<span data-ttu-id="327fc-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="327fc-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="327fc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="327fc-125">Request body</span></span>
<span data-ttu-id="327fc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="327fc-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="327fc-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="327fc-127">Response</span></span>
<span data-ttu-id="327fc-128">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="327fc-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="327fc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="327fc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="327fc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="327fc-130">Request</span></span>
<span data-ttu-id="327fc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="327fc-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="327fc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="327fc-132">Response</span></span>
<span data-ttu-id="327fc-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="327fc-133">Here is an example of the response.</span></span>
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
