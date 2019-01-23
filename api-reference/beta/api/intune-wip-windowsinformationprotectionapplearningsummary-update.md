---
title: Обновление объекта windowsInformationProtectionAppLearningSummary
description: Обновление свойств объекта windowsInformationProtectionAppLearningSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05119960dd66ef28438bdcbe8bcaa5d9c64bebf2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407272"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="3c4e7-103">Обновление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="3c4e7-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="3c4e7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3c4e7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c4e7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c4e7-107">Обновление свойств объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3c4e7-107">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c4e7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3c4e7-108">Prerequisites</span></span>
<span data-ttu-id="3c4e7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3c4e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3c4e7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c4e7-111">Permission type</span></span>|<span data-ttu-id="3c4e7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c4e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c4e7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c4e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c4e7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c4e7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c4e7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c4e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c4e7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-116">Not supported.</span></span>|
|<span data-ttu-id="3c4e7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c4e7-117">Application</span></span>|<span data-ttu-id="3c4e7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c4e7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c4e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3c4e7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c4e7-120">Request headers</span></span>
|<span data-ttu-id="3c4e7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c4e7-121">Header</span></span>|<span data-ttu-id="3c4e7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3c4e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c4e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c4e7-123">Authorization</span></span>|<span data-ttu-id="3c4e7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3c4e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c4e7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c4e7-125">Accept</span></span>|<span data-ttu-id="3c4e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c4e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c4e7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c4e7-127">Request body</span></span>
<span data-ttu-id="3c4e7-128">В теле запроса укажите представление объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="3c4e7-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3c4e7-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="3c4e7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c4e7-130">Property</span></span>|<span data-ttu-id="3c4e7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3c4e7-131">Type</span></span>|<span data-ttu-id="3c4e7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3c4e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c4e7-133">id</span><span class="sxs-lookup"><span data-stu-id="3c4e7-133">id</span></span>|<span data-ttu-id="3c4e7-134">String</span><span class="sxs-lookup"><span data-stu-id="3c4e7-134">String</span></span>|<span data-ttu-id="3c4e7-135">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="3c4e7-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="3c4e7-136">applicationName</span></span>|<span data-ttu-id="3c4e7-137">String</span><span class="sxs-lookup"><span data-stu-id="3c4e7-137">String</span></span>|<span data-ttu-id="3c4e7-138">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="3c4e7-138">Application Name</span></span>|
|<span data-ttu-id="3c4e7-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="3c4e7-139">applicationType</span></span>|[<span data-ttu-id="3c4e7-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="3c4e7-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="3c4e7-141">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-141">Application Type.</span></span> <span data-ttu-id="3c4e7-142">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="3c4e7-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="3c4e7-143">deviceCount</span></span>|<span data-ttu-id="3c4e7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="3c4e7-144">Int32</span></span>|<span data-ttu-id="3c4e7-145">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="3c4e7-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="3c4e7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c4e7-146">Response</span></span>
<span data-ttu-id="3c4e7-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c4e7-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3c4e7-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c4e7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c4e7-149">Request</span></span>
<span data-ttu-id="3c4e7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="3c4e7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c4e7-151">Response</span></span>
<span data-ttu-id="3c4e7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3c4e7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




