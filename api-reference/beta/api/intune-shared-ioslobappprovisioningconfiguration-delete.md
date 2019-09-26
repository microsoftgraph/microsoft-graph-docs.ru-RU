---
title: Удаление iosLobAppProvisioningConfiguration
description: Удаляет объект iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 100f83daff0b01406c02e6ec6d5e7471d7631a86
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201034"
---
# <a name="delete-ioslobappprovisioningconfiguration"></a><span data-ttu-id="2993e-103">Удаление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2993e-103">Delete iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="2993e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2993e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2993e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2993e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2993e-106">Удаляет объект [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2993e-106">Deletes a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2993e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2993e-107">Prerequisites</span></span>
<span data-ttu-id="2993e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2993e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2993e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2993e-110">Permission type</span></span>|<span data-ttu-id="2993e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2993e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2993e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2993e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2993e-113">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="2993e-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="2993e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2993e-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2993e-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2993e-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2993e-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2993e-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2993e-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2993e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2993e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2993e-118">Not supported.</span></span>|
|<span data-ttu-id="2993e-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2993e-119">Application</span></span>||
| <span data-ttu-id="2993e-120">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="2993e-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="2993e-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2993e-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2993e-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2993e-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2993e-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2993e-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2993e-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2993e-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2993e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2993e-125">Request headers</span></span>
|<span data-ttu-id="2993e-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2993e-126">Header</span></span>|<span data-ttu-id="2993e-127">Значение</span><span class="sxs-lookup"><span data-stu-id="2993e-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2993e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2993e-128">Authorization</span></span>|<span data-ttu-id="2993e-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2993e-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2993e-130">Accept</span><span class="sxs-lookup"><span data-stu-id="2993e-130">Accept</span></span>|<span data-ttu-id="2993e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2993e-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2993e-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2993e-132">Request body</span></span>
<span data-ttu-id="2993e-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2993e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2993e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2993e-134">Response</span></span>
<span data-ttu-id="2993e-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2993e-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2993e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="2993e-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="2993e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="2993e-137">Request</span></span>
<span data-ttu-id="2993e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2993e-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2993e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2993e-139">Response</span></span>
<span data-ttu-id="2993e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2993e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




