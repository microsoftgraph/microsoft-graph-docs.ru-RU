---
title: Создание Дефаултдевицекомплианцеполици
description: Создание нового объекта Дефаултдевицекомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06ba84a2bfcdccfc284f2e1ea4a40b337d94029d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449378"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="e603d-103">Создание Дефаултдевицекомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="e603d-103">Create defaultDeviceCompliancePolicy</span></span>

<span data-ttu-id="e603d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e603d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e603d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e603d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e603d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e603d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e603d-107">Создание нового объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e603d-107">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e603d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e603d-108">Prerequisites</span></span>
<span data-ttu-id="e603d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e603d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e603d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e603d-111">Permission type</span></span>|<span data-ttu-id="e603d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e603d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e603d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e603d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e603d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e603d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e603d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e603d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e603d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e603d-116">Not supported.</span></span>|
|<span data-ttu-id="e603d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e603d-117">Application</span></span>|<span data-ttu-id="e603d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e603d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e603d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e603d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e603d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e603d-120">Request headers</span></span>
|<span data-ttu-id="e603d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e603d-121">Header</span></span>|<span data-ttu-id="e603d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e603d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e603d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e603d-123">Authorization</span></span>|<span data-ttu-id="e603d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e603d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e603d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e603d-125">Accept</span></span>|<span data-ttu-id="e603d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e603d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e603d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e603d-127">Request body</span></span>
<span data-ttu-id="e603d-128">В тексте запроса добавьте представление объекта Дефаултдевицекомплианцеполици в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e603d-128">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="e603d-129">В следующей таблице приведены свойства, необходимые при создании Дефаултдевицекомплианцеполици.</span><span class="sxs-lookup"><span data-stu-id="e603d-129">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="e603d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e603d-130">Property</span></span>|<span data-ttu-id="e603d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e603d-131">Type</span></span>|<span data-ttu-id="e603d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e603d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e603d-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e603d-133">roleScopeTagIds</span></span>|<span data-ttu-id="e603d-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e603d-134">String collection</span></span>|<span data-ttu-id="e603d-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e603d-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e603d-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e603d-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e603d-137">id</span><span class="sxs-lookup"><span data-stu-id="e603d-137">id</span></span>|<span data-ttu-id="e603d-138">String</span><span class="sxs-lookup"><span data-stu-id="e603d-138">String</span></span>|<span data-ttu-id="e603d-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e603d-139">Key of the entity.</span></span> <span data-ttu-id="e603d-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e603d-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e603d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e603d-141">createdDateTime</span></span>|<span data-ttu-id="e603d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e603d-142">DateTimeOffset</span></span>|<span data-ttu-id="e603d-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e603d-143">DateTime the object was created.</span></span> <span data-ttu-id="e603d-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e603d-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e603d-145">description</span><span class="sxs-lookup"><span data-stu-id="e603d-145">description</span></span>|<span data-ttu-id="e603d-146">String</span><span class="sxs-lookup"><span data-stu-id="e603d-146">String</span></span>|<span data-ttu-id="e603d-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e603d-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e603d-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e603d-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e603d-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e603d-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e603d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e603d-150">DateTimeOffset</span></span>|<span data-ttu-id="e603d-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e603d-151">DateTime the object was last modified.</span></span> <span data-ttu-id="e603d-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e603d-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e603d-153">displayName</span><span class="sxs-lookup"><span data-stu-id="e603d-153">displayName</span></span>|<span data-ttu-id="e603d-154">Строка</span><span class="sxs-lookup"><span data-stu-id="e603d-154">String</span></span>|<span data-ttu-id="e603d-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e603d-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e603d-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e603d-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e603d-157">version</span><span class="sxs-lookup"><span data-stu-id="e603d-157">version</span></span>|<span data-ttu-id="e603d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e603d-158">Int32</span></span>|<span data-ttu-id="e603d-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e603d-159">Version of the device configuration.</span></span> <span data-ttu-id="e603d-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e603d-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e603d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="e603d-161">Response</span></span>
<span data-ttu-id="e603d-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e603d-162">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e603d-163">Пример</span><span class="sxs-lookup"><span data-stu-id="e603d-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="e603d-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="e603d-164">Request</span></span>
<span data-ttu-id="e603d-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e603d-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 229

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="e603d-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e603d-166">Response</span></span>
<span data-ttu-id="e603d-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e603d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 401

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a285f027-f027-a285-27f0-85a227f085a2",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```





