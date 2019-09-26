---
title: Создание объекта windowsInformationProtectionNetworkLearningSummary
description: Создание объекта windowsInformationProtectionNetworkLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3384a6f048d49ddf65898a23acd0e513230b2f6a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195106"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="19ed3-103">Создание объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="19ed3-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="19ed3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19ed3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19ed3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19ed3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19ed3-106">Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="19ed3-106">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19ed3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="19ed3-107">Prerequisites</span></span>
<span data-ttu-id="19ed3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19ed3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19ed3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19ed3-110">Permission type</span></span>|<span data-ttu-id="19ed3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19ed3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19ed3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19ed3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19ed3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19ed3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19ed3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19ed3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19ed3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19ed3-115">Not supported.</span></span>|
|<span data-ttu-id="19ed3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19ed3-116">Application</span></span>|<span data-ttu-id="19ed3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19ed3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19ed3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19ed3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="19ed3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19ed3-119">Request headers</span></span>
|<span data-ttu-id="19ed3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19ed3-120">Header</span></span>|<span data-ttu-id="19ed3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="19ed3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19ed3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19ed3-122">Authorization</span></span>|<span data-ttu-id="19ed3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19ed3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19ed3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="19ed3-124">Accept</span></span>|<span data-ttu-id="19ed3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19ed3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19ed3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19ed3-126">Request body</span></span>
<span data-ttu-id="19ed3-127">В теле запроса добавьте представление объекта windowsInformationProtectionNetworkLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19ed3-127">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="19ed3-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="19ed3-128">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="19ed3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="19ed3-129">Property</span></span>|<span data-ttu-id="19ed3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="19ed3-130">Type</span></span>|<span data-ttu-id="19ed3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="19ed3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19ed3-132">id</span><span class="sxs-lookup"><span data-stu-id="19ed3-132">id</span></span>|<span data-ttu-id="19ed3-133">String</span><span class="sxs-lookup"><span data-stu-id="19ed3-133">String</span></span>|<span data-ttu-id="19ed3-134">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="19ed3-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="19ed3-135">url</span><span class="sxs-lookup"><span data-stu-id="19ed3-135">url</span></span>|<span data-ttu-id="19ed3-136">String</span><span class="sxs-lookup"><span data-stu-id="19ed3-136">String</span></span>|<span data-ttu-id="19ed3-137">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="19ed3-137">Website url</span></span>|
|<span data-ttu-id="19ed3-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="19ed3-138">deviceCount</span></span>|<span data-ttu-id="19ed3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="19ed3-139">Int32</span></span>|<span data-ttu-id="19ed3-140">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="19ed3-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="19ed3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="19ed3-141">Response</span></span>
<span data-ttu-id="19ed3-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="19ed3-142">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19ed3-143">Пример</span><span class="sxs-lookup"><span data-stu-id="19ed3-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="19ed3-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="19ed3-144">Request</span></span>
<span data-ttu-id="19ed3-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19ed3-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19ed3-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="19ed3-146">Response</span></span>
<span data-ttu-id="19ed3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19ed3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




