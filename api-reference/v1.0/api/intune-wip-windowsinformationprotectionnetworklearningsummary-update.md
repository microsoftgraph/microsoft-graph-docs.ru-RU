---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
ms.openlocfilehash: 30f5585149a1130a92c203394950c581655cc78b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329424"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="208a8-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="208a8-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="208a8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="208a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="208a8-105">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="208a8-105">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="208a8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="208a8-106">Prerequisites</span></span>
<span data-ttu-id="208a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="208a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="208a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="208a8-109">Permission type</span></span>|<span data-ttu-id="208a8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="208a8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="208a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="208a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="208a8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="208a8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="208a8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="208a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="208a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="208a8-114">Not supported.</span></span>|
|<span data-ttu-id="208a8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="208a8-115">Application</span></span>|<span data-ttu-id="208a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="208a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="208a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="208a8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="208a8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="208a8-118">Request headers</span></span>
|<span data-ttu-id="208a8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="208a8-119">Header</span></span>|<span data-ttu-id="208a8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="208a8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="208a8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="208a8-121">Authorization</span></span>|<span data-ttu-id="208a8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="208a8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="208a8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="208a8-123">Accept</span></span>|<span data-ttu-id="208a8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="208a8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="208a8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="208a8-125">Request body</span></span>
<span data-ttu-id="208a8-126">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="208a8-126">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="208a8-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="208a8-127">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="208a8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="208a8-128">Property</span></span>|<span data-ttu-id="208a8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="208a8-129">Type</span></span>|<span data-ttu-id="208a8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="208a8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="208a8-131">id</span><span class="sxs-lookup"><span data-stu-id="208a8-131">id</span></span>|<span data-ttu-id="208a8-132">String</span><span class="sxs-lookup"><span data-stu-id="208a8-132">String</span></span>|<span data-ttu-id="208a8-133">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="208a8-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="208a8-134">url</span><span class="sxs-lookup"><span data-stu-id="208a8-134">url</span></span>|<span data-ttu-id="208a8-135">String</span><span class="sxs-lookup"><span data-stu-id="208a8-135">String</span></span>|<span data-ttu-id="208a8-136">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="208a8-136">Website url</span></span>|
|<span data-ttu-id="208a8-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="208a8-137">deviceCount</span></span>|<span data-ttu-id="208a8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="208a8-138">Int32</span></span>|<span data-ttu-id="208a8-139">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="208a8-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="208a8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="208a8-140">Response</span></span>
<span data-ttu-id="208a8-141">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="208a8-141">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="208a8-142">Пример</span><span class="sxs-lookup"><span data-stu-id="208a8-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="208a8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="208a8-143">Request</span></span>
<span data-ttu-id="208a8-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="208a8-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="208a8-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="208a8-145">Response</span></span>
<span data-ttu-id="208a8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="208a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



