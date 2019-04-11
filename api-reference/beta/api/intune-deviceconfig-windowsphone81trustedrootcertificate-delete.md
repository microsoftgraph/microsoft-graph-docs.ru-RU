---
title: Удаление windowsPhone81TrustedRootCertificate
description: Удаляет объект windowsPhone81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5581ae7de4cadefafb768bc5920e6c48565b3b46
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778189"
---
# <a name="delete-windowsphone81trustedrootcertificate"></a><span data-ttu-id="e6399-103">Удаление windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="e6399-103">Delete windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="e6399-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6399-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6399-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6399-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6399-106">Удаляет объект [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e6399-106">Deletes a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6399-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e6399-107">Prerequisites</span></span>
<span data-ttu-id="e6399-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6399-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6399-110">Permission type</span></span>|<span data-ttu-id="e6399-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6399-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6399-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6399-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6399-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6399-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6399-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6399-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6399-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6399-115">Not supported.</span></span>|
|<span data-ttu-id="e6399-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6399-116">Application</span></span>|<span data-ttu-id="e6399-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6399-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6399-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6399-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="e6399-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6399-119">Request headers</span></span>
|<span data-ttu-id="e6399-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6399-120">Header</span></span>|<span data-ttu-id="e6399-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e6399-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6399-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6399-122">Authorization</span></span>|<span data-ttu-id="e6399-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6399-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6399-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e6399-124">Accept</span></span>|<span data-ttu-id="e6399-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6399-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6399-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6399-126">Request body</span></span>
<span data-ttu-id="e6399-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6399-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6399-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6399-128">Response</span></span>
<span data-ttu-id="e6399-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6399-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6399-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e6399-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6399-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6399-131">Request</span></span>
<span data-ttu-id="e6399-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6399-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="e6399-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6399-133">Response</span></span>
<span data-ttu-id="e6399-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6399-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





