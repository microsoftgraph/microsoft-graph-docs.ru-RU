---
title: Создание объекта windowsInformationProtectionNetworkLearningSummary
description: Создание объекта windowsInformationProtectionNetworkLearningSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ef10a71e9e6b59c86e1450cea8e40465bc0f70af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403254"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="5fbb6-103">Создание объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="5fbb6-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="5fbb6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5fbb6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fbb6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fbb6-107">Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="5fbb6-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fbb6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5fbb6-108">Prerequisites</span></span>
<span data-ttu-id="5fbb6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5fbb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5fbb6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fbb6-111">Permission type</span></span>|<span data-ttu-id="5fbb6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fbb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fbb6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fbb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5fbb6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fbb6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5fbb6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fbb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fbb6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-116">Not supported.</span></span>|
|<span data-ttu-id="5fbb6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fbb6-117">Application</span></span>|<span data-ttu-id="5fbb6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fbb6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fbb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="5fbb6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fbb6-120">Request headers</span></span>
|<span data-ttu-id="5fbb6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5fbb6-121">Header</span></span>|<span data-ttu-id="5fbb6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5fbb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fbb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fbb6-123">Authorization</span></span>|<span data-ttu-id="5fbb6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5fbb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fbb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5fbb6-125">Accept</span></span>|<span data-ttu-id="5fbb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5fbb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fbb6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5fbb6-127">Request body</span></span>
<span data-ttu-id="5fbb6-128">В теле запроса добавьте представление объекта windowsInformationProtectionNetworkLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="5fbb6-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="5fbb6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fbb6-130">Property</span></span>|<span data-ttu-id="5fbb6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5fbb6-131">Type</span></span>|<span data-ttu-id="5fbb6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5fbb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fbb6-133">id</span><span class="sxs-lookup"><span data-stu-id="5fbb6-133">id</span></span>|<span data-ttu-id="5fbb6-134">String</span><span class="sxs-lookup"><span data-stu-id="5fbb6-134">String</span></span>|<span data-ttu-id="5fbb6-135">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="5fbb6-136">url</span><span class="sxs-lookup"><span data-stu-id="5fbb6-136">url</span></span>|<span data-ttu-id="5fbb6-137">String</span><span class="sxs-lookup"><span data-stu-id="5fbb6-137">String</span></span>|<span data-ttu-id="5fbb6-138">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="5fbb6-138">Website url</span></span>|
|<span data-ttu-id="5fbb6-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="5fbb6-139">deviceCount</span></span>|<span data-ttu-id="5fbb6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbb6-140">Int32</span></span>|<span data-ttu-id="5fbb6-141">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="5fbb6-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="5fbb6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fbb6-142">Response</span></span>
<span data-ttu-id="5fbb6-143">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fbb6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="5fbb6-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fbb6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fbb6-145">Request</span></span>
<span data-ttu-id="5fbb6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5fbb6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fbb6-147">Response</span></span>
<span data-ttu-id="5fbb6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5fbb6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




