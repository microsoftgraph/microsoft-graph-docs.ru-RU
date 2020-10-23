---
title: Удаление iosLobAppProvisioningConfiguration
description: Удаляет объект iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a737a1778f5b7ef75b7216cc2413388074f8cf9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729933"
---
# <a name="delete-ioslobappprovisioningconfiguration"></a><span data-ttu-id="106b5-103">Удаление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="106b5-103">Delete iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="106b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="106b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="106b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="106b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="106b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="106b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="106b5-107">Удаляет объект [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="106b5-107">Deletes a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="106b5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="106b5-108">Prerequisites</span></span>
<span data-ttu-id="106b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="106b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="106b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="106b5-111">Permission type</span></span>|<span data-ttu-id="106b5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="106b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="106b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="106b5-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="106b5-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="106b5-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="106b5-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="106b5-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="106b5-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="106b5-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="106b5-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="106b5-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="106b5-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="106b5-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="106b5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="106b5-119">Not supported.</span></span>|
|<span data-ttu-id="106b5-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="106b5-120">Application</span></span>||
| <span data-ttu-id="106b5-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="106b5-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="106b5-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="106b5-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="106b5-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="106b5-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="106b5-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="106b5-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="106b5-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="106b5-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="106b5-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="106b5-126">Request headers</span></span>
|<span data-ttu-id="106b5-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="106b5-127">Header</span></span>|<span data-ttu-id="106b5-128">Значение</span><span class="sxs-lookup"><span data-stu-id="106b5-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="106b5-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="106b5-129">Authorization</span></span>|<span data-ttu-id="106b5-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="106b5-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="106b5-131">Accept</span><span class="sxs-lookup"><span data-stu-id="106b5-131">Accept</span></span>|<span data-ttu-id="106b5-132">application/json</span><span class="sxs-lookup"><span data-stu-id="106b5-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="106b5-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="106b5-133">Request body</span></span>
<span data-ttu-id="106b5-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="106b5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="106b5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="106b5-135">Response</span></span>
<span data-ttu-id="106b5-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="106b5-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="106b5-137">Пример</span><span class="sxs-lookup"><span data-stu-id="106b5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="106b5-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="106b5-138">Request</span></span>
<span data-ttu-id="106b5-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="106b5-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="106b5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="106b5-140">Response</span></span>
<span data-ttu-id="106b5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="106b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








