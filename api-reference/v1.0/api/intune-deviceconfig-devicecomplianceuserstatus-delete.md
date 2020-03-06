---
title: Удаление объекта deviceComplianceUserStatus
description: Удаляет объект deviceComplianceUserStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be203df6bc6f2a87ac93357d2ba9f7f0c02467e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514889"
---
# <a name="delete-devicecomplianceuserstatus"></a><span data-ttu-id="da826-103">Удаление объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="da826-103">Delete deviceComplianceUserStatus</span></span>

<span data-ttu-id="da826-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da826-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da826-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da826-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da826-106">Удаляет объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="da826-106">Deletes a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da826-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="da826-107">Prerequisites</span></span>
<span data-ttu-id="da826-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da826-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da826-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da826-110">Permission type</span></span>|<span data-ttu-id="da826-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="da826-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da826-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da826-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da826-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da826-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da826-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da826-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da826-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da826-115">Not supported.</span></span>|
|<span data-ttu-id="da826-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da826-116">Application</span></span>|<span data-ttu-id="da826-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da826-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da826-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da826-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="da826-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="da826-119">Request headers</span></span>
|<span data-ttu-id="da826-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da826-120">Header</span></span>|<span data-ttu-id="da826-121">Значение</span><span class="sxs-lookup"><span data-stu-id="da826-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da826-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da826-122">Authorization</span></span>|<span data-ttu-id="da826-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da826-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da826-124">Accept</span><span class="sxs-lookup"><span data-stu-id="da826-124">Accept</span></span>|<span data-ttu-id="da826-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da826-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da826-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da826-126">Request body</span></span>
<span data-ttu-id="da826-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da826-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da826-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="da826-128">Response</span></span>
<span data-ttu-id="da826-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="da826-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="da826-130">Пример</span><span class="sxs-lookup"><span data-stu-id="da826-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="da826-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="da826-131">Request</span></span>
<span data-ttu-id="da826-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da826-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

### <a name="response"></a><span data-ttu-id="da826-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="da826-133">Response</span></span>
<span data-ttu-id="da826-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da826-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




