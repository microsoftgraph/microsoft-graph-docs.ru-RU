---
title: Delete windows10CompliancePolicy
description: Удаляет объект windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdf4861b7a158a829422f50512f0fa45e01c46ef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49236304"
---
# <a name="delete-windows10compliancepolicy"></a><span data-ttu-id="4f5b4-103">Delete windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4f5b4-103">Delete windows10CompliancePolicy</span></span>

<span data-ttu-id="4f5b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f5b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f5b4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f5b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f5b4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f5b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f5b4-107">Удаляет объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f5b4-107">Deletes a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f5b4-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4f5b4-108">Prerequisites</span></span>
<span data-ttu-id="4f5b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f5b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f5b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f5b4-111">Permission type</span></span>|<span data-ttu-id="4f5b4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f5b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f5b4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f5b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f5b4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f5b4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f5b4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f5b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f5b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f5b4-116">Not supported.</span></span>|
|<span data-ttu-id="4f5b4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f5b4-117">Application</span></span>|<span data-ttu-id="4f5b4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f5b4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f5b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f5b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4f5b4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f5b4-120">Request headers</span></span>
|<span data-ttu-id="4f5b4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f5b4-121">Header</span></span>|<span data-ttu-id="4f5b4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4f5b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f5b4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f5b4-123">Authorization</span></span>|<span data-ttu-id="4f5b4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f5b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f5b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f5b4-125">Accept</span></span>|<span data-ttu-id="4f5b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f5b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f5b4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f5b4-127">Request body</span></span>
<span data-ttu-id="4f5b4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f5b4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f5b4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f5b4-129">Response</span></span>
<span data-ttu-id="4f5b4-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4f5b4-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4f5b4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4f5b4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f5b4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f5b4-132">Request</span></span>
<span data-ttu-id="4f5b4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f5b4-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="4f5b4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f5b4-134">Response</span></span>
<span data-ttu-id="4f5b4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f5b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




