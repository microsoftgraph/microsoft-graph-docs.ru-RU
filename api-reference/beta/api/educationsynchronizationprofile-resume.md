---
title: ВозОбновление синхронизации в Едукатионсинчронизатионпрофиле
description: ВозОбновление синхронизации конкретного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 50ffcb4ceab401a3041ecb69baa1de0409be94a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464854"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="0f0e9-103">ВозОбновление синхронизации в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="0f0e9-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f0e9-104">ВозОбновление синхронизации конкретного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0f0e9-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f0e9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f0e9-105">Permissions</span></span>
<span data-ttu-id="0f0e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f0e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f0e9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f0e9-108">Permission type</span></span> | <span data-ttu-id="0f0e9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f0e9-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="0f0e9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f0e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f0e9-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f0e9-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="0f0e9-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f0e9-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0f0e9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f0e9-113">Not supported.</span></span>|
|<span data-ttu-id="0f0e9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f0e9-114">Application</span></span>|<span data-ttu-id="0f0e9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f0e9-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f0e9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f0e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="0f0e9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f0e9-117">Request headers</span></span>
| <span data-ttu-id="0f0e9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0f0e9-118">Name</span></span>       | <span data-ttu-id="0f0e9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0f0e9-119">Type</span></span> | <span data-ttu-id="0f0e9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0f0e9-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0f0e9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f0e9-121">Authorization</span></span>  | <span data-ttu-id="0f0e9-122">string</span><span class="sxs-lookup"><span data-stu-id="0f0e9-122">string</span></span>  | <span data-ttu-id="0f0e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f0e9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f0e9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f0e9-125">Request body</span></span>
<span data-ttu-id="0f0e9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f0e9-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0f0e9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f0e9-127">Response</span></span>
<span data-ttu-id="0f0e9-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="0f0e9-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0f0e9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0f0e9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f0e9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f0e9-130">Request</span></span>
<span data-ttu-id="0f0e9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f0e9-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="0f0e9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f0e9-132">Response</span></span>

<span data-ttu-id="0f0e9-133">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="0f0e9-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
