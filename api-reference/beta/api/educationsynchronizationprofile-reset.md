---
title: Сброс синхронизации для Едукатионсинчронизатионпрофиле
description: Сбросьте синхронизацию определенного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 502eb8d7afdc61926a024b7ddfbac5383a146622
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457506"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="53a1a-103">Сброс синхронизации для Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="53a1a-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53a1a-104">Сбросьте синхронизацию определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="53a1a-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="53a1a-105">**Примечание:** Эта операция приведет к перезапуску синхронизации.</span><span class="sxs-lookup"><span data-stu-id="53a1a-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="53a1a-106">Все обнаруженные ошибки будут удалены.</span><span class="sxs-lookup"><span data-stu-id="53a1a-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="53a1a-107">Данные не будут удалены из Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="53a1a-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="53a1a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53a1a-108">Permissions</span></span>
<span data-ttu-id="53a1a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53a1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53a1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53a1a-111">Permission type</span></span> | <span data-ttu-id="53a1a-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53a1a-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="53a1a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53a1a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="53a1a-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53a1a-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="53a1a-115">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53a1a-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="53a1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53a1a-116">Not supported.</span></span>|
|<span data-ttu-id="53a1a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53a1a-117">Application</span></span>|<span data-ttu-id="53a1a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53a1a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53a1a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53a1a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="53a1a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53a1a-120">Request headers</span></span>
| <span data-ttu-id="53a1a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="53a1a-121">Name</span></span>       | <span data-ttu-id="53a1a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="53a1a-122">Type</span></span> | <span data-ttu-id="53a1a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="53a1a-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53a1a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="53a1a-124">Authorization</span></span>  | <span data-ttu-id="53a1a-125">string</span><span class="sxs-lookup"><span data-stu-id="53a1a-125">string</span></span>  | <span data-ttu-id="53a1a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53a1a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53a1a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53a1a-128">Request body</span></span>
<span data-ttu-id="53a1a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53a1a-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="53a1a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="53a1a-130">Response</span></span>
<span data-ttu-id="53a1a-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="53a1a-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="53a1a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="53a1a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53a1a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="53a1a-133">Request</span></span>
<span data-ttu-id="53a1a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53a1a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="53a1a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="53a1a-135">Response</span></span>

<span data-ttu-id="53a1a-136">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="53a1a-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
