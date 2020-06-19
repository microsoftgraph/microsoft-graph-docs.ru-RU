---
title: Удаление Андроиддевицеовнертрустедрутцертификате
description: Удаляет объект Андроиддевицеовнертрустедрутцертификате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c8b3c411bd3af8bc38ce9a802824f1044bc5af5
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793075"
---
# <a name="delete-androiddeviceownertrustedrootcertificate"></a><span data-ttu-id="d72a9-103">Удаление Андроиддевицеовнертрустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="d72a9-103">Delete androidDeviceOwnerTrustedRootCertificate</span></span>

<span data-ttu-id="d72a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d72a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d72a9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d72a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d72a9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d72a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d72a9-107">Удаляет объект [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d72a9-107">Deletes a [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d72a9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d72a9-108">Prerequisites</span></span>
<span data-ttu-id="d72a9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d72a9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d72a9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d72a9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d72a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d72a9-111">Permission type</span></span>|<span data-ttu-id="d72a9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d72a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d72a9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d72a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d72a9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d72a9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d72a9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d72a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d72a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d72a9-116">Not supported.</span></span>|
|<span data-ttu-id="d72a9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d72a9-117">Application</span></span>|<span data-ttu-id="d72a9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d72a9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d72a9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d72a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/rootCertificateForServerValidation
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="d72a9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d72a9-120">Request headers</span></span>
|<span data-ttu-id="d72a9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d72a9-121">Header</span></span>|<span data-ttu-id="d72a9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d72a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d72a9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d72a9-123">Authorization</span></span>|<span data-ttu-id="d72a9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d72a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d72a9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d72a9-125">Accept</span></span>|<span data-ttu-id="d72a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d72a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d72a9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d72a9-127">Request body</span></span>
<span data-ttu-id="d72a9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d72a9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d72a9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d72a9-129">Response</span></span>
<span data-ttu-id="d72a9-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d72a9-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d72a9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d72a9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d72a9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d72a9-132">Request</span></span>
<span data-ttu-id="d72a9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d72a9-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

### <a name="response"></a><span data-ttu-id="d72a9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d72a9-134">Response</span></span>
<span data-ttu-id="d72a9-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d72a9-135">Here is an example of the response.</span></span> <span data-ttu-id="d72a9-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d72a9-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d72a9-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d72a9-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



