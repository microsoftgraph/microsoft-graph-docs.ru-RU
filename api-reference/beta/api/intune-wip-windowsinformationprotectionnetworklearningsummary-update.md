---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a22e942cd47122939050277be7a7e2661db3bf5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990430"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="41fac-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="41fac-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="41fac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41fac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41fac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41fac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41fac-106">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="41fac-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41fac-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="41fac-107">Prerequisites</span></span>
<span data-ttu-id="41fac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41fac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41fac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41fac-110">Permission type</span></span>|<span data-ttu-id="41fac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41fac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41fac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41fac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41fac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41fac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41fac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41fac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41fac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41fac-115">Not supported.</span></span>|
|<span data-ttu-id="41fac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41fac-116">Application</span></span>|<span data-ttu-id="41fac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41fac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41fac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41fac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="41fac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41fac-119">Request headers</span></span>
|<span data-ttu-id="41fac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41fac-120">Header</span></span>|<span data-ttu-id="41fac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="41fac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41fac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41fac-122">Authorization</span></span>|<span data-ttu-id="41fac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41fac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41fac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="41fac-124">Accept</span></span>|<span data-ttu-id="41fac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41fac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41fac-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41fac-126">Request body</span></span>
<span data-ttu-id="41fac-127">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41fac-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="41fac-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="41fac-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="41fac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="41fac-129">Property</span></span>|<span data-ttu-id="41fac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="41fac-130">Type</span></span>|<span data-ttu-id="41fac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="41fac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41fac-132">id</span><span class="sxs-lookup"><span data-stu-id="41fac-132">id</span></span>|<span data-ttu-id="41fac-133">String</span><span class="sxs-lookup"><span data-stu-id="41fac-133">String</span></span>|<span data-ttu-id="41fac-134">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="41fac-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="41fac-135">url</span><span class="sxs-lookup"><span data-stu-id="41fac-135">url</span></span>|<span data-ttu-id="41fac-136">String</span><span class="sxs-lookup"><span data-stu-id="41fac-136">String</span></span>|<span data-ttu-id="41fac-137">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="41fac-137">Website url</span></span>|
|<span data-ttu-id="41fac-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="41fac-138">deviceCount</span></span>|<span data-ttu-id="41fac-139">Int32</span><span class="sxs-lookup"><span data-stu-id="41fac-139">Int32</span></span>|<span data-ttu-id="41fac-140">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="41fac-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="41fac-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="41fac-141">Response</span></span>
<span data-ttu-id="41fac-142">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="41fac-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41fac-143">Пример</span><span class="sxs-lookup"><span data-stu-id="41fac-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="41fac-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="41fac-144">Request</span></span>
<span data-ttu-id="41fac-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41fac-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41fac-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="41fac-146">Response</span></span>
<span data-ttu-id="41fac-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41fac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





