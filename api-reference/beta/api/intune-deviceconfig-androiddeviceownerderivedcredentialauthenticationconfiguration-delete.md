---
title: Удаление Андроиддевицеовнердериведкредентиалаусентикатионконфигуратион
description: Удаляет объект Андроиддевицеовнердериведкредентиалаусентикатионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7bcff0882dc819d6e19ad953fa112d3cf26866b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43351419"
---
# <a name="delete-androiddeviceownerderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="a8fcb-103">Удаление Андроиддевицеовнердериведкредентиалаусентикатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a8fcb-103">Delete androidDeviceOwnerDerivedCredentialAuthenticationConfiguration</span></span>

<span data-ttu-id="a8fcb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8fcb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8fcb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8fcb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8fcb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8fcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8fcb-107">Удаляет объект [андроиддевицеовнердериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8fcb-107">Deletes a [androidDeviceOwnerDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8fcb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a8fcb-108">Prerequisites</span></span>
<span data-ttu-id="a8fcb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8fcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8fcb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8fcb-111">Permission type</span></span>|<span data-ttu-id="a8fcb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8fcb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8fcb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8fcb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8fcb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8fcb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8fcb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8fcb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8fcb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8fcb-116">Not supported.</span></span>|
|<span data-ttu-id="a8fcb-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a8fcb-117">Application</span></span>|<span data-ttu-id="a8fcb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8fcb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8fcb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8fcb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a8fcb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a8fcb-120">Request headers</span></span>
|<span data-ttu-id="a8fcb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8fcb-121">Header</span></span>|<span data-ttu-id="a8fcb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a8fcb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8fcb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8fcb-123">Authorization</span></span>|<span data-ttu-id="a8fcb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8fcb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8fcb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8fcb-125">Accept</span></span>|<span data-ttu-id="a8fcb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8fcb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8fcb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8fcb-127">Request body</span></span>
<span data-ttu-id="a8fcb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8fcb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8fcb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8fcb-129">Response</span></span>
<span data-ttu-id="a8fcb-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a8fcb-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a8fcb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a8fcb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8fcb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8fcb-132">Request</span></span>
<span data-ttu-id="a8fcb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8fcb-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a8fcb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8fcb-134">Response</span></span>
<span data-ttu-id="a8fcb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8fcb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



