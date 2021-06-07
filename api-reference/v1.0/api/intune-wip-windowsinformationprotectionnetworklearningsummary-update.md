---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 54a0e5b33cd8897f6b0b243baca2ebb7bb91f0f4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751428"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="37d4c-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="37d4c-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="37d4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37d4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37d4c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37d4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37d4c-106">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="37d4c-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37d4c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="37d4c-107">Prerequisites</span></span>
<span data-ttu-id="37d4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37d4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37d4c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37d4c-110">Permission type</span></span>|<span data-ttu-id="37d4c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37d4c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37d4c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37d4c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37d4c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d4c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37d4c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37d4c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37d4c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37d4c-115">Not supported.</span></span>|
|<span data-ttu-id="37d4c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="37d4c-116">Application</span></span>|<span data-ttu-id="37d4c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d4c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37d4c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37d4c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="37d4c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37d4c-119">Request headers</span></span>
|<span data-ttu-id="37d4c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37d4c-120">Header</span></span>|<span data-ttu-id="37d4c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="37d4c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37d4c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37d4c-122">Authorization</span></span>|<span data-ttu-id="37d4c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37d4c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37d4c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="37d4c-124">Accept</span></span>|<span data-ttu-id="37d4c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37d4c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37d4c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37d4c-126">Request body</span></span>
<span data-ttu-id="37d4c-127">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37d4c-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="37d4c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="37d4c-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="37d4c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="37d4c-129">Property</span></span>|<span data-ttu-id="37d4c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="37d4c-130">Type</span></span>|<span data-ttu-id="37d4c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="37d4c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37d4c-132">id</span><span class="sxs-lookup"><span data-stu-id="37d4c-132">id</span></span>|<span data-ttu-id="37d4c-133">String</span><span class="sxs-lookup"><span data-stu-id="37d4c-133">String</span></span>|<span data-ttu-id="37d4c-134">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="37d4c-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="37d4c-135">url</span><span class="sxs-lookup"><span data-stu-id="37d4c-135">url</span></span>|<span data-ttu-id="37d4c-136">String</span><span class="sxs-lookup"><span data-stu-id="37d4c-136">String</span></span>|<span data-ttu-id="37d4c-137">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="37d4c-137">Website url</span></span>|
|<span data-ttu-id="37d4c-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="37d4c-138">deviceCount</span></span>|<span data-ttu-id="37d4c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="37d4c-139">Int32</span></span>|<span data-ttu-id="37d4c-140">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="37d4c-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="37d4c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="37d4c-141">Response</span></span>
<span data-ttu-id="37d4c-142">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="37d4c-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37d4c-143">Пример</span><span class="sxs-lookup"><span data-stu-id="37d4c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="37d4c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="37d4c-144">Request</span></span>
<span data-ttu-id="37d4c-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37d4c-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="37d4c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="37d4c-146">Response</span></span>
<span data-ttu-id="37d4c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37d4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```




