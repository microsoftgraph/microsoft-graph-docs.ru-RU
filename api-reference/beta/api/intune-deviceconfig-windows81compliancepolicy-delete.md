---
title: Delete windows81CompliancePolicy
description: Удаляет объект windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc213013a93d3f1bb1ef65d972ffff9095ac0d7e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49204455"
---
# <a name="delete-windows81compliancepolicy"></a><span data-ttu-id="fa984-103">Delete windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fa984-103">Delete windows81CompliancePolicy</span></span>

<span data-ttu-id="fa984-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa984-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa984-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa984-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa984-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa984-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa984-107">Удаляет объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa984-107">Deletes a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa984-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fa984-108">Prerequisites</span></span>
<span data-ttu-id="fa984-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa984-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa984-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa984-111">Permission type</span></span>|<span data-ttu-id="fa984-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa984-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa984-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa984-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa984-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa984-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa984-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa984-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa984-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa984-116">Not supported.</span></span>|
|<span data-ttu-id="fa984-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fa984-117">Application</span></span>|<span data-ttu-id="fa984-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa984-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa984-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa984-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="fa984-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fa984-120">Request headers</span></span>
|<span data-ttu-id="fa984-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa984-121">Header</span></span>|<span data-ttu-id="fa984-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa984-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa984-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa984-123">Authorization</span></span>|<span data-ttu-id="fa984-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa984-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa984-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa984-125">Accept</span></span>|<span data-ttu-id="fa984-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa984-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa984-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa984-127">Request body</span></span>
<span data-ttu-id="fa984-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa984-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa984-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa984-129">Response</span></span>
<span data-ttu-id="fa984-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fa984-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fa984-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fa984-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa984-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa984-132">Request</span></span>
<span data-ttu-id="fa984-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa984-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="fa984-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa984-134">Response</span></span>
<span data-ttu-id="fa984-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa984-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




