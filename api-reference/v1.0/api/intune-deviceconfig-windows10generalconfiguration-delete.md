---
title: Delete windows10GeneralConfiguration
description: Удаляет объект windows10GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42065ef341ad3e44843bc13151568c4246ec5eab
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758159"
---
# <a name="delete-windows10generalconfiguration"></a><span data-ttu-id="22846-103">Delete windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="22846-103">Delete windows10GeneralConfiguration</span></span>

<span data-ttu-id="22846-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22846-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22846-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22846-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22846-106">Удаляет объект [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22846-106">Deletes a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22846-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="22846-107">Prerequisites</span></span>
<span data-ttu-id="22846-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22846-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22846-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22846-110">Permission type</span></span>|<span data-ttu-id="22846-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22846-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22846-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22846-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22846-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22846-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22846-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22846-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22846-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22846-115">Not supported.</span></span>|
|<span data-ttu-id="22846-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="22846-116">Application</span></span>|<span data-ttu-id="22846-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22846-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22846-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22846-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="22846-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="22846-119">Request headers</span></span>
|<span data-ttu-id="22846-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22846-120">Header</span></span>|<span data-ttu-id="22846-121">Значение</span><span class="sxs-lookup"><span data-stu-id="22846-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22846-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22846-122">Authorization</span></span>|<span data-ttu-id="22846-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22846-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22846-124">Accept</span><span class="sxs-lookup"><span data-stu-id="22846-124">Accept</span></span>|<span data-ttu-id="22846-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22846-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22846-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22846-126">Request body</span></span>
<span data-ttu-id="22846-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22846-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22846-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="22846-128">Response</span></span>
<span data-ttu-id="22846-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="22846-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="22846-130">Пример</span><span class="sxs-lookup"><span data-stu-id="22846-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="22846-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="22846-131">Request</span></span>
<span data-ttu-id="22846-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22846-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="22846-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="22846-133">Response</span></span>
<span data-ttu-id="22846-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22846-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




