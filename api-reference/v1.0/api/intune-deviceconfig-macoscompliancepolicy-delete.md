---
title: Delete macOSCompliancePolicy
description: Удаляет объект macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee12559dd84e4d5af1ae70e2d0c5ea83c71d82e0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747895"
---
# <a name="delete-macoscompliancepolicy"></a><span data-ttu-id="a3d76-103">Delete macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a3d76-103">Delete macOSCompliancePolicy</span></span>

<span data-ttu-id="a3d76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3d76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3d76-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3d76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3d76-106">Удаляет объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3d76-106">Deletes a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3d76-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a3d76-107">Prerequisites</span></span>
<span data-ttu-id="a3d76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3d76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3d76-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3d76-110">Permission type</span></span>|<span data-ttu-id="a3d76-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3d76-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3d76-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3d76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3d76-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3d76-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3d76-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3d76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3d76-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3d76-115">Not supported.</span></span>|
|<span data-ttu-id="a3d76-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a3d76-116">Application</span></span>|<span data-ttu-id="a3d76-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3d76-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3d76-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3d76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a3d76-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a3d76-119">Request headers</span></span>
|<span data-ttu-id="a3d76-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3d76-120">Header</span></span>|<span data-ttu-id="a3d76-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a3d76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3d76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3d76-122">Authorization</span></span>|<span data-ttu-id="a3d76-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3d76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3d76-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a3d76-124">Accept</span></span>|<span data-ttu-id="a3d76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3d76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3d76-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3d76-126">Request body</span></span>
<span data-ttu-id="a3d76-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3d76-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3d76-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3d76-128">Response</span></span>
<span data-ttu-id="a3d76-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a3d76-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a3d76-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a3d76-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3d76-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3d76-131">Request</span></span>
<span data-ttu-id="a3d76-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3d76-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a3d76-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3d76-133">Response</span></span>
<span data-ttu-id="a3d76-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3d76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




