---
title: Удаление iosLobAppProvisioningConfiguration
description: Удаляет iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 975774547e760f2a0b9baaa540c2a648e3a9f3f4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867709"
---
# <a name="delete-ioslobappprovisioningconfiguration"></a><span data-ttu-id="78ae8-103">Удаление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="78ae8-103">Delete iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="78ae8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78ae8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78ae8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78ae8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78ae8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78ae8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78ae8-107">Удаляет [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="78ae8-107">Deletes a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78ae8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="78ae8-108">Prerequisites</span></span>
<span data-ttu-id="78ae8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78ae8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78ae8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78ae8-111">Permission type</span></span>|<span data-ttu-id="78ae8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="78ae8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78ae8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78ae8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="78ae8-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="78ae8-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="78ae8-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78ae8-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="78ae8-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="78ae8-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="78ae8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78ae8-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="78ae8-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78ae8-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78ae8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78ae8-119">Not supported.</span></span>|
|<span data-ttu-id="78ae8-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="78ae8-120">Application</span></span>||
| <span data-ttu-id="78ae8-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="78ae8-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="78ae8-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78ae8-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="78ae8-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="78ae8-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="78ae8-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78ae8-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78ae8-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78ae8-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="78ae8-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="78ae8-126">Request headers</span></span>
|<span data-ttu-id="78ae8-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78ae8-127">Header</span></span>|<span data-ttu-id="78ae8-128">Значение</span><span class="sxs-lookup"><span data-stu-id="78ae8-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78ae8-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78ae8-129">Authorization</span></span>|<span data-ttu-id="78ae8-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78ae8-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78ae8-131">Accept</span><span class="sxs-lookup"><span data-stu-id="78ae8-131">Accept</span></span>|<span data-ttu-id="78ae8-132">application/json</span><span class="sxs-lookup"><span data-stu-id="78ae8-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78ae8-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78ae8-133">Request body</span></span>
<span data-ttu-id="78ae8-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78ae8-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78ae8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="78ae8-135">Response</span></span>
<span data-ttu-id="78ae8-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="78ae8-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="78ae8-137">Пример</span><span class="sxs-lookup"><span data-stu-id="78ae8-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="78ae8-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="78ae8-138">Request</span></span>
<span data-ttu-id="78ae8-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78ae8-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="78ae8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="78ae8-140">Response</span></span>
<span data-ttu-id="78ae8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78ae8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







