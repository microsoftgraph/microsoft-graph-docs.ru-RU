---
title: Создание объекта windowsInformationProtectionAppLearningSummary
description: Создание объекта windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 66658cdd601ec7ea1af60a29a9302ca100debfaf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940584"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="2f7f5-103">Создание объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="2f7f5-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="2f7f5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f7f5-105">Создание объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2f7f5-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f7f5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f7f5-106">Prerequisites</span></span>
<span data-ttu-id="2f7f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f7f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f7f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f7f5-109">Permission type</span></span>|<span data-ttu-id="2f7f5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f7f5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f7f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f7f5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f7f5-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f5-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f7f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f7f5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f7f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-114">Not supported.</span></span>|
|<span data-ttu-id="2f7f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f7f5-115">Application</span></span>|<span data-ttu-id="2f7f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f7f5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f7f5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2f7f5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f7f5-118">Request headers</span></span>
|<span data-ttu-id="2f7f5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f7f5-119">Header</span></span>|<span data-ttu-id="2f7f5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2f7f5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f7f5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f7f5-121">Authorization</span></span>|<span data-ttu-id="2f7f5-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f7f5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f7f5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2f7f5-123">Accept</span></span>|<span data-ttu-id="2f7f5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f7f5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f7f5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f7f5-125">Request body</span></span>
<span data-ttu-id="2f7f5-126">В теле запроса укажите представление объекта windowsInformationProtectionAppLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="2f7f5-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="2f7f5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f7f5-128">Property</span></span>|<span data-ttu-id="2f7f5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2f7f5-129">Type</span></span>|<span data-ttu-id="2f7f5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2f7f5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f7f5-131">id</span><span class="sxs-lookup"><span data-stu-id="2f7f5-131">id</span></span>|<span data-ttu-id="2f7f5-132">String</span><span class="sxs-lookup"><span data-stu-id="2f7f5-132">String</span></span>|<span data-ttu-id="2f7f5-133">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="2f7f5-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="2f7f5-134">applicationName</span></span>|<span data-ttu-id="2f7f5-135">String</span><span class="sxs-lookup"><span data-stu-id="2f7f5-135">String</span></span>|<span data-ttu-id="2f7f5-136">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="2f7f5-136">Application Name</span></span>|
|<span data-ttu-id="2f7f5-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="2f7f5-137">applicationType</span></span>|[<span data-ttu-id="2f7f5-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="2f7f5-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="2f7f5-139">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-139">Application Type.</span></span> <span data-ttu-id="2f7f5-140">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="2f7f5-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2f7f5-141">deviceCount</span></span>|<span data-ttu-id="2f7f5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2f7f5-142">Int32</span></span>|<span data-ttu-id="2f7f5-143">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="2f7f5-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="2f7f5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f7f5-144">Response</span></span>
<span data-ttu-id="2f7f5-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f7f5-146">Пример</span><span class="sxs-lookup"><span data-stu-id="2f7f5-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f7f5-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f7f5-147">Request</span></span>
<span data-ttu-id="2f7f5-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="2f7f5-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f7f5-149">Response</span></span>
<span data-ttu-id="2f7f5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2f7f5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```



