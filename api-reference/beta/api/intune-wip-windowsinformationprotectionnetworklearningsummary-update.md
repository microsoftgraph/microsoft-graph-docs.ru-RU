---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c2ea14531060f511ad90383b50eefe8c9c495f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457288"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="32460-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="32460-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="32460-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="32460-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32460-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32460-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32460-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32460-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32460-107">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="32460-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32460-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32460-108">Prerequisites</span></span>
<span data-ttu-id="32460-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32460-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32460-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32460-111">Permission type</span></span>|<span data-ttu-id="32460-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32460-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32460-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32460-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32460-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32460-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32460-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32460-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32460-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32460-116">Not supported.</span></span>|
|<span data-ttu-id="32460-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32460-117">Application</span></span>|<span data-ttu-id="32460-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32460-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32460-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32460-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="32460-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32460-120">Request headers</span></span>
|<span data-ttu-id="32460-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32460-121">Header</span></span>|<span data-ttu-id="32460-122">Значение</span><span class="sxs-lookup"><span data-stu-id="32460-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32460-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32460-123">Authorization</span></span>|<span data-ttu-id="32460-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32460-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32460-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32460-125">Accept</span></span>|<span data-ttu-id="32460-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32460-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32460-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32460-127">Request body</span></span>
<span data-ttu-id="32460-128">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32460-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="32460-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="32460-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="32460-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="32460-130">Property</span></span>|<span data-ttu-id="32460-131">Тип</span><span class="sxs-lookup"><span data-stu-id="32460-131">Type</span></span>|<span data-ttu-id="32460-132">Описание</span><span class="sxs-lookup"><span data-stu-id="32460-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32460-133">id</span><span class="sxs-lookup"><span data-stu-id="32460-133">id</span></span>|<span data-ttu-id="32460-134">String</span><span class="sxs-lookup"><span data-stu-id="32460-134">String</span></span>|<span data-ttu-id="32460-135">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="32460-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="32460-136">url</span><span class="sxs-lookup"><span data-stu-id="32460-136">url</span></span>|<span data-ttu-id="32460-137">String</span><span class="sxs-lookup"><span data-stu-id="32460-137">String</span></span>|<span data-ttu-id="32460-138">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="32460-138">Website url</span></span>|
|<span data-ttu-id="32460-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="32460-139">deviceCount</span></span>|<span data-ttu-id="32460-140">Int32</span><span class="sxs-lookup"><span data-stu-id="32460-140">Int32</span></span>|<span data-ttu-id="32460-141">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="32460-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="32460-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="32460-142">Response</span></span>
<span data-ttu-id="32460-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="32460-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32460-144">Пример</span><span class="sxs-lookup"><span data-stu-id="32460-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="32460-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="32460-145">Request</span></span>
<span data-ttu-id="32460-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32460-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="32460-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="32460-147">Response</span></span>
<span data-ttu-id="32460-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32460-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





