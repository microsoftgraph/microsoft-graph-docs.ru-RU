---
title: Создание объекта windowsInformationProtectionNetworkLearningSummary
description: Создание объекта windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55b9561f36006b27aa3fb918a76bfb6735b5e470
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261414"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="362f6-103">Создание объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="362f6-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="362f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="362f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="362f6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="362f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="362f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="362f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="362f6-107">Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="362f6-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="362f6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="362f6-108">Prerequisites</span></span>
<span data-ttu-id="362f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="362f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="362f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="362f6-111">Permission type</span></span>|<span data-ttu-id="362f6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="362f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="362f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="362f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="362f6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="362f6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="362f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="362f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="362f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="362f6-116">Not supported.</span></span>|
|<span data-ttu-id="362f6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="362f6-117">Application</span></span>|<span data-ttu-id="362f6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="362f6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="362f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="362f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="362f6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="362f6-120">Request headers</span></span>
|<span data-ttu-id="362f6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="362f6-121">Header</span></span>|<span data-ttu-id="362f6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="362f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="362f6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="362f6-123">Authorization</span></span>|<span data-ttu-id="362f6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="362f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="362f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="362f6-125">Accept</span></span>|<span data-ttu-id="362f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="362f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="362f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="362f6-127">Request body</span></span>
<span data-ttu-id="362f6-128">В теле запроса добавьте представление объекта windowsInformationProtectionNetworkLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="362f6-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="362f6-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="362f6-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="362f6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="362f6-130">Property</span></span>|<span data-ttu-id="362f6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="362f6-131">Type</span></span>|<span data-ttu-id="362f6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="362f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="362f6-133">id</span><span class="sxs-lookup"><span data-stu-id="362f6-133">id</span></span>|<span data-ttu-id="362f6-134">String</span><span class="sxs-lookup"><span data-stu-id="362f6-134">String</span></span>|<span data-ttu-id="362f6-135">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="362f6-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="362f6-136">url</span><span class="sxs-lookup"><span data-stu-id="362f6-136">url</span></span>|<span data-ttu-id="362f6-137">String</span><span class="sxs-lookup"><span data-stu-id="362f6-137">String</span></span>|<span data-ttu-id="362f6-138">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="362f6-138">Website url</span></span>|
|<span data-ttu-id="362f6-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="362f6-139">deviceCount</span></span>|<span data-ttu-id="362f6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="362f6-140">Int32</span></span>|<span data-ttu-id="362f6-141">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="362f6-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="362f6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="362f6-142">Response</span></span>
<span data-ttu-id="362f6-143">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="362f6-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="362f6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="362f6-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="362f6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="362f6-145">Request</span></span>
<span data-ttu-id="362f6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="362f6-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="362f6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="362f6-147">Response</span></span>
<span data-ttu-id="362f6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="362f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




