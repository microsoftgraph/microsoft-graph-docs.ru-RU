---
title: Удаление объекта windowsInformationProtectionAppLearningSummary
description: Удаляет объект windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d713e0826b075110dd21169347349ce8a5f68543
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576362"
---
# <a name="delete-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="738f6-103">Удаление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="738f6-103">Delete windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="738f6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="738f6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="738f6-105">Удаляет объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="738f6-105">Deletes a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="738f6-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="738f6-106">Prerequisites</span></span>
<span data-ttu-id="738f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="738f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="738f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="738f6-109">Permission type</span></span>|<span data-ttu-id="738f6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="738f6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="738f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="738f6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="738f6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="738f6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="738f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="738f6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="738f6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="738f6-114">Not supported.</span></span>|
|<span data-ttu-id="738f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="738f6-115">Application</span></span>|<span data-ttu-id="738f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="738f6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="738f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="738f6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="738f6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="738f6-118">Request headers</span></span>
|<span data-ttu-id="738f6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="738f6-119">Header</span></span>|<span data-ttu-id="738f6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="738f6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="738f6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="738f6-121">Authorization</span></span>|<span data-ttu-id="738f6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="738f6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="738f6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="738f6-123">Accept</span></span>|<span data-ttu-id="738f6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="738f6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="738f6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="738f6-125">Request body</span></span>
<span data-ttu-id="738f6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="738f6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="738f6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="738f6-127">Response</span></span>
<span data-ttu-id="738f6-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="738f6-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="738f6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="738f6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="738f6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="738f6-130">Request</span></span>
<span data-ttu-id="738f6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="738f6-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="738f6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="738f6-132">Response</span></span>
<span data-ttu-id="738f6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="738f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



