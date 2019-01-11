---
title: Создание объекта windowsInformationProtectionNetworkLearningSummary
description: Создание объекта windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 57cfde950bc4152c605e41e0caff8d18d919eb46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876463"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="f0433-103">Создание объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="f0433-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="f0433-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0433-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0433-105">Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f0433-105">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0433-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0433-106">Prerequisites</span></span>
<span data-ttu-id="f0433-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0433-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0433-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0433-109">Permission type</span></span>|<span data-ttu-id="f0433-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0433-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0433-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0433-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0433-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0433-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0433-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0433-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0433-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0433-114">Not supported.</span></span>|
|<span data-ttu-id="f0433-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0433-115">Application</span></span>|<span data-ttu-id="f0433-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0433-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0433-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0433-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f0433-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0433-118">Request headers</span></span>
|<span data-ttu-id="f0433-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0433-119">Header</span></span>|<span data-ttu-id="f0433-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f0433-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0433-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0433-121">Authorization</span></span>|<span data-ttu-id="f0433-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f0433-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0433-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f0433-123">Accept</span></span>|<span data-ttu-id="f0433-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f0433-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0433-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0433-125">Request body</span></span>
<span data-ttu-id="f0433-126">В теле запроса добавьте представление объекта windowsInformationProtectionNetworkLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0433-126">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="f0433-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="f0433-127">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="f0433-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0433-128">Property</span></span>|<span data-ttu-id="f0433-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f0433-129">Type</span></span>|<span data-ttu-id="f0433-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f0433-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0433-131">id</span><span class="sxs-lookup"><span data-stu-id="f0433-131">id</span></span>|<span data-ttu-id="f0433-132">String</span><span class="sxs-lookup"><span data-stu-id="f0433-132">String</span></span>|<span data-ttu-id="f0433-133">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="f0433-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="f0433-134">url</span><span class="sxs-lookup"><span data-stu-id="f0433-134">url</span></span>|<span data-ttu-id="f0433-135">String</span><span class="sxs-lookup"><span data-stu-id="f0433-135">String</span></span>|<span data-ttu-id="f0433-136">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="f0433-136">Website url</span></span>|
|<span data-ttu-id="f0433-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="f0433-137">deviceCount</span></span>|<span data-ttu-id="f0433-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f0433-138">Int32</span></span>|<span data-ttu-id="f0433-139">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="f0433-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="f0433-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0433-140">Response</span></span>
<span data-ttu-id="f0433-141">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0433-141">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0433-142">Пример</span><span class="sxs-lookup"><span data-stu-id="f0433-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0433-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0433-143">Request</span></span>
<span data-ttu-id="f0433-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0433-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="f0433-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0433-145">Response</span></span>
<span data-ttu-id="f0433-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0433-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



