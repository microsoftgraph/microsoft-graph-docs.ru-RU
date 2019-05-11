---
title: Удаление Макострустедрутцертификате
description: Удаляет объект Макострустедрутцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e6ae506b5f4327162936b8f3c9dd9ee2d29facf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922292"
---
# <a name="delete-macostrustedrootcertificate"></a><span data-ttu-id="88184-103">Удаление Макострустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="88184-103">Delete macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="88184-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88184-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88184-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88184-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88184-106">Удаляет объект [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="88184-106">Deletes a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88184-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88184-107">Prerequisites</span></span>
<span data-ttu-id="88184-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88184-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88184-110">Permission type</span></span>|<span data-ttu-id="88184-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88184-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88184-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88184-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88184-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88184-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88184-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88184-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88184-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88184-115">Not supported.</span></span>|
|<span data-ttu-id="88184-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88184-116">Application</span></span>|<span data-ttu-id="88184-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88184-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88184-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88184-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="88184-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88184-119">Request headers</span></span>
|<span data-ttu-id="88184-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88184-120">Header</span></span>|<span data-ttu-id="88184-121">Значение</span><span class="sxs-lookup"><span data-stu-id="88184-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88184-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88184-122">Authorization</span></span>|<span data-ttu-id="88184-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88184-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88184-124">Accept</span><span class="sxs-lookup"><span data-stu-id="88184-124">Accept</span></span>|<span data-ttu-id="88184-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88184-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88184-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88184-126">Request body</span></span>
<span data-ttu-id="88184-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88184-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88184-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="88184-128">Response</span></span>
<span data-ttu-id="88184-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="88184-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88184-130">Пример</span><span class="sxs-lookup"><span data-stu-id="88184-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="88184-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="88184-131">Request</span></span>
<span data-ttu-id="88184-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88184-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="88184-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="88184-133">Response</span></span>
<span data-ttu-id="88184-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88184-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




