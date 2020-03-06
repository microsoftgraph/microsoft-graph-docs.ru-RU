---
title: Удаление windowsInformationProtectionNetworkLearningSummary
description: Удаление объекта windowsInformationProtectionNetworkLearningSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c6eba96f1c0485c3ac94f66e933b5105597c01f8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511791"
---
# <a name="delete-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="0d461-103">Удаление windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="0d461-103">Delete windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="0d461-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d461-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d461-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d461-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d461-106">Удаление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0d461-106">Deletes a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d461-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d461-107">Prerequisites</span></span>
<span data-ttu-id="0d461-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d461-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d461-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d461-110">Permission type</span></span>|<span data-ttu-id="0d461-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d461-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d461-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d461-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d461-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d461-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d461-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d461-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d461-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d461-115">Not supported.</span></span>|
|<span data-ttu-id="0d461-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d461-116">Application</span></span>|<span data-ttu-id="0d461-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d461-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d461-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d461-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="0d461-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d461-119">Request headers</span></span>
|<span data-ttu-id="0d461-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d461-120">Header</span></span>|<span data-ttu-id="0d461-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d461-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d461-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d461-122">Authorization</span></span>|<span data-ttu-id="0d461-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d461-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d461-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d461-124">Accept</span></span>|<span data-ttu-id="0d461-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d461-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d461-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d461-126">Request body</span></span>
<span data-ttu-id="0d461-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d461-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d461-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d461-128">Response</span></span>
<span data-ttu-id="0d461-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d461-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d461-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0d461-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d461-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d461-131">Request</span></span>
<span data-ttu-id="0d461-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d461-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="0d461-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d461-133">Response</span></span>
<span data-ttu-id="0d461-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d461-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




