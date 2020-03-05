---
title: Удаление windows81TrustedRootCertificate
description: Удаляет объект windows81TrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1040d4b302334588c255cedbaeeb8f7ffe576a3a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42476918"
---
# <a name="delete-windows81trustedrootcertificate"></a><span data-ttu-id="0b958-103">Удаление windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0b958-103">Delete windows81TrustedRootCertificate</span></span>

<span data-ttu-id="0b958-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0b958-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b958-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b958-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b958-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b958-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b958-107">Удаляет объект [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="0b958-107">Deletes a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b958-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0b958-108">Prerequisites</span></span>
<span data-ttu-id="0b958-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b958-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b958-111">Permission type</span></span>|<span data-ttu-id="0b958-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b958-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b958-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b958-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b958-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b958-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b958-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b958-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b958-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b958-116">Not supported.</span></span>|
|<span data-ttu-id="0b958-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b958-117">Application</span></span>|<span data-ttu-id="0b958-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b958-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b958-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b958-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="0b958-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0b958-120">Request headers</span></span>
|<span data-ttu-id="0b958-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b958-121">Header</span></span>|<span data-ttu-id="0b958-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0b958-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b958-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b958-123">Authorization</span></span>|<span data-ttu-id="0b958-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b958-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b958-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b958-125">Accept</span></span>|<span data-ttu-id="0b958-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b958-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b958-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b958-127">Request body</span></span>
<span data-ttu-id="0b958-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b958-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b958-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b958-129">Response</span></span>
<span data-ttu-id="0b958-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b958-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b958-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0b958-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b958-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b958-132">Request</span></span>
<span data-ttu-id="0b958-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b958-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
```

### <a name="response"></a><span data-ttu-id="0b958-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b958-134">Response</span></span>
<span data-ttu-id="0b958-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b958-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





