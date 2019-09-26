---
title: Удаление Андроиддевицеовнертрустедрутцертификате
description: Удаляет объект Андроиддевицеовнертрустедрутцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 85405346d9d22f314e6a3d59cb534aa334c2a084
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37169848"
---
# <a name="delete-androiddeviceownertrustedrootcertificate"></a><span data-ttu-id="0e208-103">Удаление Андроиддевицеовнертрустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="0e208-103">Delete androidDeviceOwnerTrustedRootCertificate</span></span>

> <span data-ttu-id="0e208-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e208-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e208-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e208-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e208-106">Удаляет объект [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="0e208-106">Deletes a [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e208-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e208-107">Prerequisites</span></span>
<span data-ttu-id="0e208-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e208-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e208-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e208-110">Permission type</span></span>|<span data-ttu-id="0e208-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e208-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e208-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e208-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e208-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e208-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e208-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e208-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e208-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e208-115">Not supported.</span></span>|
|<span data-ttu-id="0e208-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e208-116">Application</span></span>|<span data-ttu-id="0e208-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e208-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e208-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e208-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerCertificateProfileBase/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="0e208-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e208-119">Request headers</span></span>
|<span data-ttu-id="0e208-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e208-120">Header</span></span>|<span data-ttu-id="0e208-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0e208-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e208-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e208-122">Authorization</span></span>|<span data-ttu-id="0e208-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e208-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e208-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e208-124">Accept</span></span>|<span data-ttu-id="0e208-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e208-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e208-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e208-126">Request body</span></span>
<span data-ttu-id="0e208-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e208-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e208-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e208-128">Response</span></span>
<span data-ttu-id="0e208-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0e208-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e208-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0e208-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e208-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e208-131">Request</span></span>
<span data-ttu-id="0e208-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e208-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
```

### <a name="response"></a><span data-ttu-id="0e208-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e208-133">Response</span></span>
<span data-ttu-id="0e208-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e208-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




