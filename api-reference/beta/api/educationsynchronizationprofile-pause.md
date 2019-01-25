---
title: Приостановка синхронизации на educationSynchronizationProfile
description: Приостановка синхронизации в конкретных школа профиль синхронизации данных клиента.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c9ba7d2ab3f67880105d45d9d98506b8e8caaac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510934"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="11fef-103">Приостановка синхронизации на educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="11fef-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11fef-104">Приостановка синхронизации данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="11fef-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="11fef-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11fef-105">Permissions</span></span>
<span data-ttu-id="11fef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11fef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11fef-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11fef-108">Permission type</span></span> | <span data-ttu-id="11fef-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11fef-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="11fef-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11fef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="11fef-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11fef-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="11fef-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11fef-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="11fef-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11fef-113">Not supported.</span></span>|
|<span data-ttu-id="11fef-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11fef-114">Application</span></span>|<span data-ttu-id="11fef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11fef-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11fef-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11fef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="11fef-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11fef-117">Request headers</span></span>
| <span data-ttu-id="11fef-118">Имя</span><span class="sxs-lookup"><span data-stu-id="11fef-118">Name</span></span>       | <span data-ttu-id="11fef-119">Тип</span><span class="sxs-lookup"><span data-stu-id="11fef-119">Type</span></span> | <span data-ttu-id="11fef-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11fef-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="11fef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11fef-121">Authorization</span></span>  | <span data-ttu-id="11fef-122">string</span><span class="sxs-lookup"><span data-stu-id="11fef-122">string</span></span>  | <span data-ttu-id="11fef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11fef-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11fef-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11fef-125">Request body</span></span>
<span data-ttu-id="11fef-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11fef-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="11fef-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="11fef-127">Response</span></span>
<span data-ttu-id="11fef-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="11fef-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="11fef-129">Пример</span><span class="sxs-lookup"><span data-stu-id="11fef-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11fef-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="11fef-130">Request</span></span>
<span data-ttu-id="11fef-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11fef-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="11fef-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="11fef-132">Response</span></span>

<span data-ttu-id="11fef-133">Нет тело ответа отсутствует.</span><span class="sxs-lookup"><span data-stu-id="11fef-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
