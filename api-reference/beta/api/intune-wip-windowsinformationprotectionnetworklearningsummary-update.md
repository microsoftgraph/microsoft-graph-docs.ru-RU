---
title: Обновление объекта windowsInformationProtectionNetworkLearningSummary
description: Обновление свойств объекта windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
ms.openlocfilehash: 335fee7e664000584fa4542985a3b014d827f0d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344438"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="243e6-103">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="243e6-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="243e6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="243e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="243e6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="243e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="243e6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="243e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="243e6-107">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="243e6-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="243e6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="243e6-108">Prerequisites</span></span>
<span data-ttu-id="243e6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="243e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="243e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="243e6-111">Permission type</span></span>|<span data-ttu-id="243e6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="243e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="243e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="243e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="243e6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="243e6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="243e6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="243e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="243e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="243e6-116">Not supported.</span></span>|
|<span data-ttu-id="243e6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="243e6-117">Application</span></span>|<span data-ttu-id="243e6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="243e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="243e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="243e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="243e6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="243e6-120">Request headers</span></span>
|<span data-ttu-id="243e6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="243e6-121">Header</span></span>|<span data-ttu-id="243e6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="243e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="243e6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="243e6-123">Authorization</span></span>|<span data-ttu-id="243e6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="243e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="243e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="243e6-125">Accept</span></span>|<span data-ttu-id="243e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="243e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="243e6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="243e6-127">Request body</span></span>
<span data-ttu-id="243e6-128">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="243e6-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="243e6-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="243e6-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="243e6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="243e6-130">Property</span></span>|<span data-ttu-id="243e6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="243e6-131">Type</span></span>|<span data-ttu-id="243e6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="243e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="243e6-133">id</span><span class="sxs-lookup"><span data-stu-id="243e6-133">id</span></span>|<span data-ttu-id="243e6-134">String</span><span class="sxs-lookup"><span data-stu-id="243e6-134">String</span></span>|<span data-ttu-id="243e6-135">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="243e6-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="243e6-136">url</span><span class="sxs-lookup"><span data-stu-id="243e6-136">url</span></span>|<span data-ttu-id="243e6-137">String</span><span class="sxs-lookup"><span data-stu-id="243e6-137">String</span></span>|<span data-ttu-id="243e6-138">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="243e6-138">Website url</span></span>|
|<span data-ttu-id="243e6-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="243e6-139">deviceCount</span></span>|<span data-ttu-id="243e6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="243e6-140">Int32</span></span>|<span data-ttu-id="243e6-141">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="243e6-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="243e6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="243e6-142">Response</span></span>
<span data-ttu-id="243e6-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="243e6-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="243e6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="243e6-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="243e6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="243e6-145">Request</span></span>
<span data-ttu-id="243e6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="243e6-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="243e6-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="243e6-147">Response</span></span>
<span data-ttu-id="243e6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="243e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





