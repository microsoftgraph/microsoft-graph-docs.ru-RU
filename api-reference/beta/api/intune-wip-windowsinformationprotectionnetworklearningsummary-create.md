---
title: Создание объекта windowsInformationProtectionNetworkLearningSummary
description: Создание объекта windowsInformationProtectionNetworkLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 567d6ceb8cd197cd60cbee4eff7e6886a7cae01b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898892"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="968db-103">Создание объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="968db-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="968db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="968db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="968db-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="968db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="968db-106">Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="968db-106">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="968db-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="968db-107">Prerequisites</span></span>
<span data-ttu-id="968db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="968db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="968db-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="968db-110">Permission type</span></span>|<span data-ttu-id="968db-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="968db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="968db-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="968db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="968db-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="968db-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="968db-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="968db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="968db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="968db-115">Not supported.</span></span>|
|<span data-ttu-id="968db-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="968db-116">Application</span></span>|<span data-ttu-id="968db-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="968db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="968db-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="968db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="968db-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="968db-119">Request headers</span></span>
|<span data-ttu-id="968db-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="968db-120">Header</span></span>|<span data-ttu-id="968db-121">Значение</span><span class="sxs-lookup"><span data-stu-id="968db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="968db-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="968db-122">Authorization</span></span>|<span data-ttu-id="968db-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="968db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="968db-124">Accept</span><span class="sxs-lookup"><span data-stu-id="968db-124">Accept</span></span>|<span data-ttu-id="968db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="968db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="968db-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="968db-126">Request body</span></span>
<span data-ttu-id="968db-127">В теле запроса добавьте представление объекта windowsInformationProtectionNetworkLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="968db-127">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="968db-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="968db-128">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="968db-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="968db-129">Property</span></span>|<span data-ttu-id="968db-130">Тип</span><span class="sxs-lookup"><span data-stu-id="968db-130">Type</span></span>|<span data-ttu-id="968db-131">Описание</span><span class="sxs-lookup"><span data-stu-id="968db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="968db-132">id</span><span class="sxs-lookup"><span data-stu-id="968db-132">id</span></span>|<span data-ttu-id="968db-133">Строка</span><span class="sxs-lookup"><span data-stu-id="968db-133">String</span></span>|<span data-ttu-id="968db-134">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="968db-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="968db-135">url</span><span class="sxs-lookup"><span data-stu-id="968db-135">url</span></span>|<span data-ttu-id="968db-136">String</span><span class="sxs-lookup"><span data-stu-id="968db-136">String</span></span>|<span data-ttu-id="968db-137">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="968db-137">Website url</span></span>|
|<span data-ttu-id="968db-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="968db-138">deviceCount</span></span>|<span data-ttu-id="968db-139">Int32</span><span class="sxs-lookup"><span data-stu-id="968db-139">Int32</span></span>|<span data-ttu-id="968db-140">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="968db-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="968db-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="968db-141">Response</span></span>
<span data-ttu-id="968db-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="968db-142">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="968db-143">Пример</span><span class="sxs-lookup"><span data-stu-id="968db-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="968db-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="968db-144">Request</span></span>
<span data-ttu-id="968db-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="968db-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="968db-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="968db-146">Response</span></span>
<span data-ttu-id="968db-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="968db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




