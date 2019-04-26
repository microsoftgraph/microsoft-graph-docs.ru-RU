---
title: Создание объекта windowsInformationProtectionAppLearningSummary
description: Создание объекта windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43f36e67ea0d1ec46708bcac1e5ecdf528f35c5b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576341"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="dae35-103">Создание объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="dae35-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="dae35-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dae35-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dae35-105">Создание объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="dae35-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dae35-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dae35-106">Prerequisites</span></span>
<span data-ttu-id="dae35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dae35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dae35-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dae35-109">Permission type</span></span>|<span data-ttu-id="dae35-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dae35-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dae35-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dae35-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dae35-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae35-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dae35-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dae35-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dae35-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dae35-114">Not supported.</span></span>|
|<span data-ttu-id="dae35-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dae35-115">Application</span></span>|<span data-ttu-id="dae35-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dae35-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dae35-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dae35-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="dae35-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dae35-118">Request headers</span></span>
|<span data-ttu-id="dae35-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dae35-119">Header</span></span>|<span data-ttu-id="dae35-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dae35-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dae35-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dae35-121">Authorization</span></span>|<span data-ttu-id="dae35-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dae35-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dae35-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dae35-123">Accept</span></span>|<span data-ttu-id="dae35-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dae35-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dae35-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dae35-125">Request body</span></span>
<span data-ttu-id="dae35-126">В теле запроса укажите представление объекта windowsInformationProtectionAppLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dae35-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="dae35-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="dae35-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="dae35-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="dae35-128">Property</span></span>|<span data-ttu-id="dae35-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dae35-129">Type</span></span>|<span data-ttu-id="dae35-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dae35-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dae35-131">id</span><span class="sxs-lookup"><span data-stu-id="dae35-131">id</span></span>|<span data-ttu-id="dae35-132">String</span><span class="sxs-lookup"><span data-stu-id="dae35-132">String</span></span>|<span data-ttu-id="dae35-133">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="dae35-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="dae35-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="dae35-134">applicationName</span></span>|<span data-ttu-id="dae35-135">String</span><span class="sxs-lookup"><span data-stu-id="dae35-135">String</span></span>|<span data-ttu-id="dae35-136">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="dae35-136">Application Name</span></span>|
|<span data-ttu-id="dae35-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="dae35-137">applicationType</span></span>|[<span data-ttu-id="dae35-138">Аппликатионтипе</span><span class="sxs-lookup"><span data-stu-id="dae35-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="dae35-139">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="dae35-139">Application Type.</span></span> <span data-ttu-id="dae35-140">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="dae35-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="dae35-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="dae35-141">deviceCount</span></span>|<span data-ttu-id="dae35-142">Int32</span><span class="sxs-lookup"><span data-stu-id="dae35-142">Int32</span></span>|<span data-ttu-id="dae35-143">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="dae35-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="dae35-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dae35-144">Response</span></span>
<span data-ttu-id="dae35-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dae35-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dae35-146">Пример</span><span class="sxs-lookup"><span data-stu-id="dae35-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="dae35-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="dae35-147">Request</span></span>
<span data-ttu-id="dae35-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dae35-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dae35-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="dae35-149">Response</span></span>
<span data-ttu-id="dae35-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dae35-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



