---
title: Удаление androidWorkProfileGeneralDeviceConfiguration
description: Удаляет объект androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9579e9339debe3a3ba825f704b99e30e392513e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401092"
---
# <a name="delete-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="312b5-103">Удаление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="312b5-103">Delete androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="312b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="312b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="312b5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="312b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="312b5-106">Удаляет объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="312b5-106">Deletes a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="312b5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="312b5-107">Prerequisites</span></span>
<span data-ttu-id="312b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="312b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="312b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="312b5-110">Permission type</span></span>|<span data-ttu-id="312b5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="312b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="312b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="312b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="312b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="312b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="312b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="312b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="312b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="312b5-115">Not supported.</span></span>|
|<span data-ttu-id="312b5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="312b5-116">Application</span></span>|<span data-ttu-id="312b5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="312b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="312b5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="312b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="312b5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="312b5-119">Request headers</span></span>
|<span data-ttu-id="312b5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="312b5-120">Header</span></span>|<span data-ttu-id="312b5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="312b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="312b5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="312b5-122">Authorization</span></span>|<span data-ttu-id="312b5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="312b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="312b5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="312b5-124">Accept</span></span>|<span data-ttu-id="312b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="312b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="312b5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="312b5-126">Request body</span></span>
<span data-ttu-id="312b5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="312b5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="312b5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="312b5-128">Response</span></span>
<span data-ttu-id="312b5-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="312b5-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="312b5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="312b5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="312b5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="312b5-131">Request</span></span>
<span data-ttu-id="312b5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="312b5-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="312b5-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="312b5-133">Response</span></span>
<span data-ttu-id="312b5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="312b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






