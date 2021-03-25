---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ccbdde0262fbea91383e0099e8c29abdfab14a8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159328"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="f3a5b-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="f3a5b-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="f3a5b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3a5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3a5b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3a5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3a5b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3a5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3a5b-107">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f3a5b-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3a5b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f3a5b-108">Prerequisites</span></span>
<span data-ttu-id="f3a5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3a5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3a5b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3a5b-111">Permission type</span></span>|<span data-ttu-id="f3a5b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3a5b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3a5b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3a5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3a5b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a5b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3a5b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3a5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3a5b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3a5b-116">Not supported.</span></span>|
|<span data-ttu-id="f3a5b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3a5b-117">Application</span></span>|<span data-ttu-id="f3a5b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a5b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3a5b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3a5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="f3a5b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3a5b-120">Request headers</span></span>
|<span data-ttu-id="f3a5b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3a5b-121">Header</span></span>|<span data-ttu-id="f3a5b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3a5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3a5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3a5b-123">Authorization</span></span>|<span data-ttu-id="f3a5b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3a5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3a5b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3a5b-125">Accept</span></span>|<span data-ttu-id="f3a5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3a5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3a5b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3a5b-127">Request body</span></span>
<span data-ttu-id="f3a5b-128">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3a5b-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="f3a5b-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f3a5b-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="f3a5b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3a5b-130">Property</span></span>|<span data-ttu-id="f3a5b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3a5b-131">Type</span></span>|<span data-ttu-id="f3a5b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3a5b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3a5b-133">id</span><span class="sxs-lookup"><span data-stu-id="f3a5b-133">id</span></span>|<span data-ttu-id="f3a5b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f3a5b-134">String</span></span>|<span data-ttu-id="f3a5b-135">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="f3a5b-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="f3a5b-136">url</span><span class="sxs-lookup"><span data-stu-id="f3a5b-136">url</span></span>|<span data-ttu-id="f3a5b-137">String</span><span class="sxs-lookup"><span data-stu-id="f3a5b-137">String</span></span>|<span data-ttu-id="f3a5b-138">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="f3a5b-138">Website url</span></span>|
|<span data-ttu-id="f3a5b-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="f3a5b-139">deviceCount</span></span>|<span data-ttu-id="f3a5b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f3a5b-140">Int32</span></span>|<span data-ttu-id="f3a5b-141">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="f3a5b-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="f3a5b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3a5b-142">Response</span></span>
<span data-ttu-id="f3a5b-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f3a5b-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3a5b-144">Пример</span><span class="sxs-lookup"><span data-stu-id="f3a5b-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3a5b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3a5b-145">Request</span></span>
<span data-ttu-id="f3a5b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3a5b-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3a5b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3a5b-147">Response</span></span>
<span data-ttu-id="f3a5b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3a5b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




