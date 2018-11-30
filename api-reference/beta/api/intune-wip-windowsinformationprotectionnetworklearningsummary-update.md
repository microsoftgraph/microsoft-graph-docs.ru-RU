---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
ms.openlocfilehash: ade11aa7dfdbe9f189923ad470d411e19a50fb51
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079549"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="d1c4d-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="d1c4d-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="d1c4d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d1c4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1c4d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1c4d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d1c4d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1c4d-107">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d1c4d-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1c4d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d1c4d-108">Prerequisites</span></span>
<span data-ttu-id="d1c4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1c4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1c4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1c4d-111">Permission type</span></span>|<span data-ttu-id="d1c4d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1c4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1c4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1c4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1c4d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1c4d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d1c4d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1c4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1c4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c4d-116">Not supported.</span></span>|
|<span data-ttu-id="d1c4d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1c4d-117">Application</span></span>|<span data-ttu-id="d1c4d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c4d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1c4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1c4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d1c4d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1c4d-120">Request headers</span></span>
|<span data-ttu-id="d1c4d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1c4d-121">Header</span></span>|<span data-ttu-id="d1c4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d1c4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1c4d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1c4d-123">Authorization</span></span>|<span data-ttu-id="d1c4d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d1c4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1c4d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1c4d-125">Accept</span></span>|<span data-ttu-id="d1c4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1c4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1c4d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1c4d-127">Request body</span></span>
<span data-ttu-id="d1c4d-128">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1c4d-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="d1c4d-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d1c4d-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="d1c4d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1c4d-130">Property</span></span>|<span data-ttu-id="d1c4d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d1c4d-131">Type</span></span>|<span data-ttu-id="d1c4d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d1c4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1c4d-133">id</span><span class="sxs-lookup"><span data-stu-id="d1c4d-133">id</span></span>|<span data-ttu-id="d1c4d-134">String</span><span class="sxs-lookup"><span data-stu-id="d1c4d-134">String</span></span>|<span data-ttu-id="d1c4d-135">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="d1c4d-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="d1c4d-136">url</span><span class="sxs-lookup"><span data-stu-id="d1c4d-136">url</span></span>|<span data-ttu-id="d1c4d-137">String</span><span class="sxs-lookup"><span data-stu-id="d1c4d-137">String</span></span>|<span data-ttu-id="d1c4d-138">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="d1c4d-138">Website url</span></span>|
|<span data-ttu-id="d1c4d-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d1c4d-139">deviceCount</span></span>|<span data-ttu-id="d1c4d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d1c4d-140">Int32</span></span>|<span data-ttu-id="d1c4d-141">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="d1c4d-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="d1c4d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1c4d-142">Response</span></span>
<span data-ttu-id="d1c4d-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d1c4d-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1c4d-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d1c4d-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1c4d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1c4d-145">Request</span></span>
<span data-ttu-id="d1c4d-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1c4d-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="d1c4d-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1c4d-147">Response</span></span>
<span data-ttu-id="d1c4d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d1c4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





