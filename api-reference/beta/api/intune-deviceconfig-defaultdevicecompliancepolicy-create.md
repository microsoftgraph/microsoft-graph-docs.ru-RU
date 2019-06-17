---
title: Создание Дефаултдевицекомплианцеполици
description: Создание нового объекта Дефаултдевицекомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3d290439234eddbc6ff570442c943e517afd09f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968723"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="ef6b2-103">Создание Дефаултдевицекомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="ef6b2-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="ef6b2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef6b2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef6b2-106">Создание нового объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ef6b2-106">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef6b2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ef6b2-107">Prerequisites</span></span>
<span data-ttu-id="ef6b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef6b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef6b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef6b2-110">Permission type</span></span>|<span data-ttu-id="ef6b2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef6b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef6b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef6b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef6b2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef6b2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef6b2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef6b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef6b2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-115">Not supported.</span></span>|
|<span data-ttu-id="ef6b2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef6b2-116">Application</span></span>|<span data-ttu-id="ef6b2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef6b2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef6b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ef6b2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef6b2-119">Request headers</span></span>
|<span data-ttu-id="ef6b2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef6b2-120">Header</span></span>|<span data-ttu-id="ef6b2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ef6b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef6b2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef6b2-122">Authorization</span></span>|<span data-ttu-id="ef6b2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef6b2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ef6b2-124">Accept</span></span>|<span data-ttu-id="ef6b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef6b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef6b2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef6b2-126">Request body</span></span>
<span data-ttu-id="ef6b2-127">В тексте запроса добавьте представление объекта Дефаултдевицекомплианцеполици в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-127">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="ef6b2-128">В следующей таблице приведены свойства, необходимые при создании Дефаултдевицекомплианцеполици.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-128">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="ef6b2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef6b2-129">Property</span></span>|<span data-ttu-id="ef6b2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ef6b2-130">Type</span></span>|<span data-ttu-id="ef6b2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ef6b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef6b2-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef6b2-132">roleScopeTagIds</span></span>|<span data-ttu-id="ef6b2-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ef6b2-133">String collection</span></span>|<span data-ttu-id="ef6b2-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef6b2-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef6b2-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef6b2-136">id</span><span class="sxs-lookup"><span data-stu-id="ef6b2-136">id</span></span>|<span data-ttu-id="ef6b2-137">String</span><span class="sxs-lookup"><span data-stu-id="ef6b2-137">String</span></span>|<span data-ttu-id="ef6b2-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-138">Key of the entity.</span></span> <span data-ttu-id="ef6b2-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef6b2-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef6b2-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef6b2-140">createdDateTime</span></span>|<span data-ttu-id="ef6b2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef6b2-141">DateTimeOffset</span></span>|<span data-ttu-id="ef6b2-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-142">DateTime the object was created.</span></span> <span data-ttu-id="ef6b2-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef6b2-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef6b2-144">description</span><span class="sxs-lookup"><span data-stu-id="ef6b2-144">description</span></span>|<span data-ttu-id="ef6b2-145">String</span><span class="sxs-lookup"><span data-stu-id="ef6b2-145">String</span></span>|<span data-ttu-id="ef6b2-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef6b2-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef6b2-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef6b2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef6b2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ef6b2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef6b2-149">DateTimeOffset</span></span>|<span data-ttu-id="ef6b2-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-150">DateTime the object was last modified.</span></span> <span data-ttu-id="ef6b2-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef6b2-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef6b2-152">displayName</span><span class="sxs-lookup"><span data-stu-id="ef6b2-152">displayName</span></span>|<span data-ttu-id="ef6b2-153">Строка</span><span class="sxs-lookup"><span data-stu-id="ef6b2-153">String</span></span>|<span data-ttu-id="ef6b2-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef6b2-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef6b2-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef6b2-156">version</span><span class="sxs-lookup"><span data-stu-id="ef6b2-156">version</span></span>|<span data-ttu-id="ef6b2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ef6b2-157">Int32</span></span>|<span data-ttu-id="ef6b2-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-158">Version of the device configuration.</span></span> <span data-ttu-id="ef6b2-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef6b2-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ef6b2-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef6b2-160">Response</span></span>
<span data-ttu-id="ef6b2-161">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-161">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef6b2-162">Пример</span><span class="sxs-lookup"><span data-stu-id="ef6b2-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef6b2-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef6b2-163">Request</span></span>
<span data-ttu-id="ef6b2-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef6b2-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef6b2-165">Response</span></span>
<span data-ttu-id="ef6b2-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef6b2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





