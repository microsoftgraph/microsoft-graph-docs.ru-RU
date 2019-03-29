---
title: Создание объекта windowsInformationProtectionNetworkLearningSummary
description: Создание объекта windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d7946f4858dd2ee53d1411165ef23fe8ee553ea
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974939"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="7d026-103">Создание объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="7d026-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="7d026-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d026-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d026-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d026-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d026-106">Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="7d026-106">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d026-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7d026-107">Prerequisites</span></span>
<span data-ttu-id="7d026-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d026-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d026-110">Permission type</span></span>|<span data-ttu-id="7d026-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d026-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d026-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d026-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d026-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d026-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d026-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d026-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d026-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d026-115">Not supported.</span></span>|
|<span data-ttu-id="7d026-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d026-116">Application</span></span>|<span data-ttu-id="7d026-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d026-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d026-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d026-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="7d026-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d026-119">Request headers</span></span>
|<span data-ttu-id="7d026-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d026-120">Header</span></span>|<span data-ttu-id="7d026-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7d026-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d026-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d026-122">Authorization</span></span>|<span data-ttu-id="7d026-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d026-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d026-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7d026-124">Accept</span></span>|<span data-ttu-id="7d026-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d026-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d026-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d026-126">Request body</span></span>
<span data-ttu-id="7d026-127">В теле запроса добавьте представление объекта windowsInformationProtectionNetworkLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d026-127">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="7d026-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="7d026-128">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="7d026-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d026-129">Property</span></span>|<span data-ttu-id="7d026-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7d026-130">Type</span></span>|<span data-ttu-id="7d026-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7d026-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d026-132">id</span><span class="sxs-lookup"><span data-stu-id="7d026-132">id</span></span>|<span data-ttu-id="7d026-133">String</span><span class="sxs-lookup"><span data-stu-id="7d026-133">String</span></span>|<span data-ttu-id="7d026-134">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="7d026-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="7d026-135">url</span><span class="sxs-lookup"><span data-stu-id="7d026-135">url</span></span>|<span data-ttu-id="7d026-136">String</span><span class="sxs-lookup"><span data-stu-id="7d026-136">String</span></span>|<span data-ttu-id="7d026-137">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="7d026-137">Website url</span></span>|
|<span data-ttu-id="7d026-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="7d026-138">deviceCount</span></span>|<span data-ttu-id="7d026-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7d026-139">Int32</span></span>|<span data-ttu-id="7d026-140">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="7d026-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="7d026-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d026-141">Response</span></span>
<span data-ttu-id="7d026-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7d026-142">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d026-143">Пример</span><span class="sxs-lookup"><span data-stu-id="7d026-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d026-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d026-144">Request</span></span>
<span data-ttu-id="7d026-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d026-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d026-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d026-146">Response</span></span>
<span data-ttu-id="7d026-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d026-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




