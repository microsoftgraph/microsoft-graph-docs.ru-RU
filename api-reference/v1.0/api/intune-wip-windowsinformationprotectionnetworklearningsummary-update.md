---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd0579d21430891b1b912968eed8389d4a67d7b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025685"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="6b9d4-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="6b9d4-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="6b9d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b9d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b9d4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b9d4-106">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b9d4-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b9d4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6b9d4-107">Prerequisites</span></span>
<span data-ttu-id="6b9d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b9d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b9d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b9d4-110">Permission type</span></span>|<span data-ttu-id="6b9d4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b9d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b9d4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b9d4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6b9d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b9d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-115">Not supported.</span></span>|
|<span data-ttu-id="6b9d4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b9d4-116">Application</span></span>|<span data-ttu-id="6b9d4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b9d4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b9d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="6b9d4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6b9d4-119">Request headers</span></span>
|<span data-ttu-id="6b9d4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b9d4-120">Header</span></span>|<span data-ttu-id="6b9d4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6b9d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b9d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b9d4-122">Authorization</span></span>|<span data-ttu-id="6b9d4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b9d4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6b9d4-124">Accept</span></span>|<span data-ttu-id="6b9d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b9d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b9d4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6b9d4-126">Request body</span></span>
<span data-ttu-id="6b9d4-127">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="6b9d4-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b9d4-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="6b9d4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b9d4-129">Property</span></span>|<span data-ttu-id="6b9d4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6b9d4-130">Type</span></span>|<span data-ttu-id="6b9d4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6b9d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b9d4-132">id</span><span class="sxs-lookup"><span data-stu-id="6b9d4-132">id</span></span>|<span data-ttu-id="6b9d4-133">String</span><span class="sxs-lookup"><span data-stu-id="6b9d4-133">String</span></span>|<span data-ttu-id="6b9d4-134">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="6b9d4-135">url</span><span class="sxs-lookup"><span data-stu-id="6b9d4-135">url</span></span>|<span data-ttu-id="6b9d4-136">String</span><span class="sxs-lookup"><span data-stu-id="6b9d4-136">String</span></span>|<span data-ttu-id="6b9d4-137">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="6b9d4-137">Website url</span></span>|
|<span data-ttu-id="6b9d4-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="6b9d4-138">deviceCount</span></span>|<span data-ttu-id="6b9d4-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6b9d4-139">Int32</span></span>|<span data-ttu-id="6b9d4-140">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="6b9d4-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="6b9d4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b9d4-141">Response</span></span>
<span data-ttu-id="6b9d4-142">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b9d4-143">Пример</span><span class="sxs-lookup"><span data-stu-id="6b9d4-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b9d4-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b9d4-144">Request</span></span>
<span data-ttu-id="6b9d4-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b9d4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b9d4-146">Response</span></span>
<span data-ttu-id="6b9d4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









