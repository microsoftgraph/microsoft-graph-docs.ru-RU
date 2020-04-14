---
title: Обновление Дефаултдевицекомплианцеполици
description: Обновление свойств объекта Дефаултдевицекомплианцеполици.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac0799c8065d2cc8dee12f4fe9bc5cf3a6e4932d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434291"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="9679f-103">Обновление Дефаултдевицекомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="9679f-103">Update defaultDeviceCompliancePolicy</span></span>

<span data-ttu-id="9679f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9679f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9679f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9679f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9679f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9679f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9679f-107">Обновление свойств объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9679f-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9679f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9679f-108">Prerequisites</span></span>
<span data-ttu-id="9679f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9679f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9679f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9679f-111">Permission type</span></span>|<span data-ttu-id="9679f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9679f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9679f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9679f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9679f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9679f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9679f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9679f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9679f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9679f-116">Not supported.</span></span>|
|<span data-ttu-id="9679f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9679f-117">Application</span></span>|<span data-ttu-id="9679f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9679f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9679f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9679f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9679f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9679f-120">Request headers</span></span>
|<span data-ttu-id="9679f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9679f-121">Header</span></span>|<span data-ttu-id="9679f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9679f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9679f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9679f-123">Authorization</span></span>|<span data-ttu-id="9679f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9679f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9679f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9679f-125">Accept</span></span>|<span data-ttu-id="9679f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9679f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9679f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9679f-127">Request body</span></span>
<span data-ttu-id="9679f-128">В тексте запроса добавьте представление объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9679f-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="9679f-129">В следующей таблице приведены свойства, необходимые при создании [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9679f-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="9679f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9679f-130">Property</span></span>|<span data-ttu-id="9679f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9679f-131">Type</span></span>|<span data-ttu-id="9679f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9679f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9679f-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9679f-133">roleScopeTagIds</span></span>|<span data-ttu-id="9679f-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9679f-134">String collection</span></span>|<span data-ttu-id="9679f-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9679f-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9679f-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9679f-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9679f-137">id</span><span class="sxs-lookup"><span data-stu-id="9679f-137">id</span></span>|<span data-ttu-id="9679f-138">String</span><span class="sxs-lookup"><span data-stu-id="9679f-138">String</span></span>|<span data-ttu-id="9679f-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9679f-139">Key of the entity.</span></span> <span data-ttu-id="9679f-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9679f-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9679f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9679f-141">createdDateTime</span></span>|<span data-ttu-id="9679f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9679f-142">DateTimeOffset</span></span>|<span data-ttu-id="9679f-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9679f-143">DateTime the object was created.</span></span> <span data-ttu-id="9679f-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9679f-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9679f-145">description</span><span class="sxs-lookup"><span data-stu-id="9679f-145">description</span></span>|<span data-ttu-id="9679f-146">String</span><span class="sxs-lookup"><span data-stu-id="9679f-146">String</span></span>|<span data-ttu-id="9679f-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9679f-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9679f-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9679f-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9679f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9679f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9679f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9679f-150">DateTimeOffset</span></span>|<span data-ttu-id="9679f-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9679f-151">DateTime the object was last modified.</span></span> <span data-ttu-id="9679f-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9679f-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9679f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="9679f-153">displayName</span></span>|<span data-ttu-id="9679f-154">Строка</span><span class="sxs-lookup"><span data-stu-id="9679f-154">String</span></span>|<span data-ttu-id="9679f-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9679f-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9679f-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9679f-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9679f-157">version</span><span class="sxs-lookup"><span data-stu-id="9679f-157">version</span></span>|<span data-ttu-id="9679f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9679f-158">Int32</span></span>|<span data-ttu-id="9679f-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9679f-159">Version of the device configuration.</span></span> <span data-ttu-id="9679f-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9679f-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9679f-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="9679f-161">Response</span></span>
<span data-ttu-id="9679f-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9679f-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9679f-163">Пример</span><span class="sxs-lookup"><span data-stu-id="9679f-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="9679f-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="9679f-164">Request</span></span>
<span data-ttu-id="9679f-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9679f-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="9679f-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="9679f-166">Response</span></span>
<span data-ttu-id="9679f-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9679f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



