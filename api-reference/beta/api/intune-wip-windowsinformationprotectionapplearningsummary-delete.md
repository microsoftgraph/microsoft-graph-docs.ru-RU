---
title: Удаление объекта windowsInformationProtectionAppLearningSummary
description: Удаляет объект windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad0d8dcd509a9fce08a65f94e47cf71edd69970d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144853"
---
# <a name="delete-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="21d74-103">Удаление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="21d74-103">Delete windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="21d74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21d74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21d74-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21d74-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21d74-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21d74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21d74-107">Удаляет объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="21d74-107">Deletes a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21d74-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21d74-108">Prerequisites</span></span>
<span data-ttu-id="21d74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21d74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21d74-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21d74-111">Permission type</span></span>|<span data-ttu-id="21d74-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21d74-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21d74-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21d74-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21d74-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d74-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21d74-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21d74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21d74-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21d74-116">Not supported.</span></span>|
|<span data-ttu-id="21d74-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="21d74-117">Application</span></span>|<span data-ttu-id="21d74-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d74-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21d74-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21d74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="21d74-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="21d74-120">Request headers</span></span>
|<span data-ttu-id="21d74-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21d74-121">Header</span></span>|<span data-ttu-id="21d74-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21d74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21d74-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21d74-123">Authorization</span></span>|<span data-ttu-id="21d74-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21d74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21d74-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21d74-125">Accept</span></span>|<span data-ttu-id="21d74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21d74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21d74-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21d74-127">Request body</span></span>
<span data-ttu-id="21d74-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21d74-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21d74-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="21d74-129">Response</span></span>
<span data-ttu-id="21d74-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="21d74-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="21d74-131">Пример</span><span class="sxs-lookup"><span data-stu-id="21d74-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="21d74-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="21d74-132">Request</span></span>
<span data-ttu-id="21d74-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21d74-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="21d74-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="21d74-134">Response</span></span>
<span data-ttu-id="21d74-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21d74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




