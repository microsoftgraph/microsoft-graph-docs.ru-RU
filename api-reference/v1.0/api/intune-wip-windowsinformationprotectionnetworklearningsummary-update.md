---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a990993b8b208908a126efd7cfb058d1c0437c1b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256933"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="1cd1a-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="1cd1a-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="1cd1a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cd1a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cd1a-105">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="1cd1a-105">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cd1a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1cd1a-106">Prerequisites</span></span>
<span data-ttu-id="1cd1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1cd1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1cd1a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cd1a-109">Permission type</span></span>|<span data-ttu-id="1cd1a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cd1a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cd1a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cd1a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1cd1a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cd1a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1cd1a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cd1a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cd1a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd1a-114">Not supported.</span></span>|
|<span data-ttu-id="1cd1a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cd1a-115">Application</span></span>|<span data-ttu-id="1cd1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd1a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cd1a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cd1a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="1cd1a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cd1a-118">Request headers</span></span>
|<span data-ttu-id="1cd1a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cd1a-119">Header</span></span>|<span data-ttu-id="1cd1a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1cd1a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cd1a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cd1a-121">Authorization</span></span>|<span data-ttu-id="1cd1a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1cd1a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cd1a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1cd1a-123">Accept</span></span>|<span data-ttu-id="1cd1a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1cd1a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cd1a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1cd1a-125">Request body</span></span>
<span data-ttu-id="1cd1a-126">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cd1a-126">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="1cd1a-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="1cd1a-127">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="1cd1a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cd1a-128">Property</span></span>|<span data-ttu-id="1cd1a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1cd1a-129">Type</span></span>|<span data-ttu-id="1cd1a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1cd1a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd1a-131">id</span><span class="sxs-lookup"><span data-stu-id="1cd1a-131">id</span></span>|<span data-ttu-id="1cd1a-132">Строка</span><span class="sxs-lookup"><span data-stu-id="1cd1a-132">String</span></span>|<span data-ttu-id="1cd1a-133">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="1cd1a-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="1cd1a-134">url</span><span class="sxs-lookup"><span data-stu-id="1cd1a-134">url</span></span>|<span data-ttu-id="1cd1a-135">String</span><span class="sxs-lookup"><span data-stu-id="1cd1a-135">String</span></span>|<span data-ttu-id="1cd1a-136">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="1cd1a-136">Website url</span></span>|
|<span data-ttu-id="1cd1a-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1cd1a-137">deviceCount</span></span>|<span data-ttu-id="1cd1a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd1a-138">Int32</span></span>|<span data-ttu-id="1cd1a-139">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="1cd1a-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="1cd1a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cd1a-140">Response</span></span>
<span data-ttu-id="1cd1a-141">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1cd1a-141">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cd1a-142">Пример</span><span class="sxs-lookup"><span data-stu-id="1cd1a-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cd1a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cd1a-143">Request</span></span>
<span data-ttu-id="1cd1a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cd1a-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1cd1a-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cd1a-145">Response</span></span>
<span data-ttu-id="1cd1a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1cd1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



