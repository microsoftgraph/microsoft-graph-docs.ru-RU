---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6faf25df55e7a4e920a27402395a66d9b0e4267
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025577"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="8bb36-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="8bb36-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="8bb36-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bb36-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bb36-105">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="8bb36-105">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bb36-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8bb36-106">Prerequisites</span></span>
<span data-ttu-id="8bb36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bb36-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb36-109">Permission type</span></span>|<span data-ttu-id="8bb36-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bb36-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bb36-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bb36-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8bb36-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb36-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8bb36-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bb36-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bb36-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb36-114">Not supported.</span></span>|
|<span data-ttu-id="8bb36-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bb36-115">Application</span></span>|<span data-ttu-id="8bb36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb36-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bb36-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bb36-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="8bb36-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bb36-118">Request headers</span></span>
|<span data-ttu-id="8bb36-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bb36-119">Header</span></span>|<span data-ttu-id="8bb36-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8bb36-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bb36-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bb36-121">Authorization</span></span>|<span data-ttu-id="8bb36-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bb36-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bb36-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8bb36-123">Accept</span></span>|<span data-ttu-id="8bb36-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8bb36-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bb36-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8bb36-125">Request body</span></span>
<span data-ttu-id="8bb36-126">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bb36-126">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="8bb36-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="8bb36-127">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="8bb36-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bb36-128">Property</span></span>|<span data-ttu-id="8bb36-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8bb36-129">Type</span></span>|<span data-ttu-id="8bb36-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb36-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bb36-131">id</span><span class="sxs-lookup"><span data-stu-id="8bb36-131">id</span></span>|<span data-ttu-id="8bb36-132">String</span><span class="sxs-lookup"><span data-stu-id="8bb36-132">String</span></span>|<span data-ttu-id="8bb36-133">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="8bb36-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="8bb36-134">url</span><span class="sxs-lookup"><span data-stu-id="8bb36-134">url</span></span>|<span data-ttu-id="8bb36-135">String</span><span class="sxs-lookup"><span data-stu-id="8bb36-135">String</span></span>|<span data-ttu-id="8bb36-136">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="8bb36-136">Website url</span></span>|
|<span data-ttu-id="8bb36-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8bb36-137">deviceCount</span></span>|<span data-ttu-id="8bb36-138">Int32</span><span class="sxs-lookup"><span data-stu-id="8bb36-138">Int32</span></span>|<span data-ttu-id="8bb36-139">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="8bb36-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="8bb36-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb36-140">Response</span></span>
<span data-ttu-id="8bb36-141">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8bb36-141">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bb36-142">Пример</span><span class="sxs-lookup"><span data-stu-id="8bb36-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bb36-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bb36-143">Request</span></span>
<span data-ttu-id="8bb36-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bb36-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8bb36-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb36-145">Response</span></span>
<span data-ttu-id="8bb36-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bb36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



