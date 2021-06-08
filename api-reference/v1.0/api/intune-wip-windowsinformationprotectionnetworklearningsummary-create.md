---
title: Создание объекта windowsInformationProtectionNetworkLearningSummary
description: Создание объекта windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bcf0b70458cc3b9dec18363209e5cd18e8dcc365
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759004"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="2025e-103">Создание объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="2025e-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="2025e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2025e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2025e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2025e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2025e-106">Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2025e-106">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2025e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2025e-107">Prerequisites</span></span>
<span data-ttu-id="2025e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2025e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2025e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2025e-110">Permission type</span></span>|<span data-ttu-id="2025e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2025e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2025e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2025e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2025e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2025e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2025e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2025e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2025e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2025e-115">Not supported.</span></span>|
|<span data-ttu-id="2025e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2025e-116">Application</span></span>|<span data-ttu-id="2025e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2025e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2025e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2025e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2025e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2025e-119">Request headers</span></span>
|<span data-ttu-id="2025e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2025e-120">Header</span></span>|<span data-ttu-id="2025e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2025e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2025e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2025e-122">Authorization</span></span>|<span data-ttu-id="2025e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2025e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2025e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2025e-124">Accept</span></span>|<span data-ttu-id="2025e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2025e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2025e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2025e-126">Request body</span></span>
<span data-ttu-id="2025e-127">В теле запроса добавьте представление объекта windowsInformationProtectionNetworkLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2025e-127">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="2025e-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2025e-128">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="2025e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2025e-129">Property</span></span>|<span data-ttu-id="2025e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2025e-130">Type</span></span>|<span data-ttu-id="2025e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2025e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2025e-132">id</span><span class="sxs-lookup"><span data-stu-id="2025e-132">id</span></span>|<span data-ttu-id="2025e-133">String</span><span class="sxs-lookup"><span data-stu-id="2025e-133">String</span></span>|<span data-ttu-id="2025e-134">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2025e-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="2025e-135">url</span><span class="sxs-lookup"><span data-stu-id="2025e-135">url</span></span>|<span data-ttu-id="2025e-136">String</span><span class="sxs-lookup"><span data-stu-id="2025e-136">String</span></span>|<span data-ttu-id="2025e-137">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="2025e-137">Website url</span></span>|
|<span data-ttu-id="2025e-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2025e-138">deviceCount</span></span>|<span data-ttu-id="2025e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2025e-139">Int32</span></span>|<span data-ttu-id="2025e-140">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="2025e-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="2025e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2025e-141">Response</span></span>
<span data-ttu-id="2025e-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2025e-142">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2025e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2025e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2025e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2025e-144">Request</span></span>
<span data-ttu-id="2025e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2025e-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="2025e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2025e-146">Response</span></span>
<span data-ttu-id="2025e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2025e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```




