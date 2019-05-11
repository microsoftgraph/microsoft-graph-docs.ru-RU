---
title: Создание объекта windowsInformationProtectionAppLearningSummary
description: Создание объекта windowsInformationProtectionAppLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2751000742487fd3b88e2e7b054edfd2cfd13c48
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33897830"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="c6d89-103">Создание объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="c6d89-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="c6d89-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6d89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6d89-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6d89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6d89-106">Создание объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c6d89-106">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6d89-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c6d89-107">Prerequisites</span></span>
<span data-ttu-id="c6d89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6d89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6d89-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6d89-110">Permission type</span></span>|<span data-ttu-id="c6d89-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6d89-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6d89-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6d89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6d89-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6d89-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6d89-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6d89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6d89-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6d89-115">Not supported.</span></span>|
|<span data-ttu-id="c6d89-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6d89-116">Application</span></span>|<span data-ttu-id="c6d89-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6d89-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6d89-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6d89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="c6d89-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6d89-119">Request headers</span></span>
|<span data-ttu-id="c6d89-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6d89-120">Header</span></span>|<span data-ttu-id="c6d89-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c6d89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6d89-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6d89-122">Authorization</span></span>|<span data-ttu-id="c6d89-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6d89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6d89-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c6d89-124">Accept</span></span>|<span data-ttu-id="c6d89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6d89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6d89-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6d89-126">Request body</span></span>
<span data-ttu-id="c6d89-127">В теле запроса укажите представление объекта windowsInformationProtectionAppLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6d89-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="c6d89-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="c6d89-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="c6d89-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6d89-129">Property</span></span>|<span data-ttu-id="c6d89-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c6d89-130">Type</span></span>|<span data-ttu-id="c6d89-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c6d89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6d89-132">id</span><span class="sxs-lookup"><span data-stu-id="c6d89-132">id</span></span>|<span data-ttu-id="c6d89-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c6d89-133">String</span></span>|<span data-ttu-id="c6d89-134">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="c6d89-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="c6d89-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="c6d89-135">applicationName</span></span>|<span data-ttu-id="c6d89-136">String</span><span class="sxs-lookup"><span data-stu-id="c6d89-136">String</span></span>|<span data-ttu-id="c6d89-137">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="c6d89-137">Application Name</span></span>|
|<span data-ttu-id="c6d89-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="c6d89-138">applicationType</span></span>|[<span data-ttu-id="c6d89-139">Аппликатионтипе</span><span class="sxs-lookup"><span data-stu-id="c6d89-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="c6d89-140">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="c6d89-140">Application Type.</span></span> <span data-ttu-id="c6d89-141">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="c6d89-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="c6d89-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="c6d89-142">deviceCount</span></span>|<span data-ttu-id="c6d89-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c6d89-143">Int32</span></span>|<span data-ttu-id="c6d89-144">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="c6d89-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="c6d89-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6d89-145">Response</span></span>
<span data-ttu-id="c6d89-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c6d89-146">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6d89-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c6d89-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6d89-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6d89-148">Request</span></span>
<span data-ttu-id="c6d89-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6d89-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="c6d89-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6d89-150">Response</span></span>
<span data-ttu-id="c6d89-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6d89-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




