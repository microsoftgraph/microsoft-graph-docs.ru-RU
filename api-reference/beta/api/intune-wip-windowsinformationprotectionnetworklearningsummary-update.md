---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d72b0db5fd59268047dc843e9a9d3eb358048cc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692599"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="05066-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="05066-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="05066-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05066-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05066-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05066-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05066-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05066-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05066-107">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="05066-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05066-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05066-108">Prerequisites</span></span>
<span data-ttu-id="05066-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05066-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05066-111">Permission type</span></span>|<span data-ttu-id="05066-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05066-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05066-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05066-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05066-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05066-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05066-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05066-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05066-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05066-116">Not supported.</span></span>|
|<span data-ttu-id="05066-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05066-117">Application</span></span>|<span data-ttu-id="05066-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05066-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05066-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05066-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="05066-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="05066-120">Request headers</span></span>
|<span data-ttu-id="05066-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05066-121">Header</span></span>|<span data-ttu-id="05066-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05066-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05066-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05066-123">Authorization</span></span>|<span data-ttu-id="05066-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05066-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05066-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05066-125">Accept</span></span>|<span data-ttu-id="05066-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05066-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05066-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05066-127">Request body</span></span>
<span data-ttu-id="05066-128">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05066-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="05066-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="05066-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="05066-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="05066-130">Property</span></span>|<span data-ttu-id="05066-131">Тип</span><span class="sxs-lookup"><span data-stu-id="05066-131">Type</span></span>|<span data-ttu-id="05066-132">Описание</span><span class="sxs-lookup"><span data-stu-id="05066-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05066-133">id</span><span class="sxs-lookup"><span data-stu-id="05066-133">id</span></span>|<span data-ttu-id="05066-134">Строка</span><span class="sxs-lookup"><span data-stu-id="05066-134">String</span></span>|<span data-ttu-id="05066-135">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="05066-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="05066-136">url</span><span class="sxs-lookup"><span data-stu-id="05066-136">url</span></span>|<span data-ttu-id="05066-137">String</span><span class="sxs-lookup"><span data-stu-id="05066-137">String</span></span>|<span data-ttu-id="05066-138">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="05066-138">Website url</span></span>|
|<span data-ttu-id="05066-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="05066-139">deviceCount</span></span>|<span data-ttu-id="05066-140">Int32</span><span class="sxs-lookup"><span data-stu-id="05066-140">Int32</span></span>|<span data-ttu-id="05066-141">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="05066-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="05066-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="05066-142">Response</span></span>
<span data-ttu-id="05066-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05066-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05066-144">Пример</span><span class="sxs-lookup"><span data-stu-id="05066-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="05066-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="05066-145">Request</span></span>
<span data-ttu-id="05066-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05066-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05066-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="05066-147">Response</span></span>
<span data-ttu-id="05066-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05066-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





