---
title: Создание Дефаултдевицекомплианцеполици
description: Создание нового объекта Дефаултдевицекомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b83c040093593565d7f4d2e2b7e7cd575a48951
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534220"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="59879-103">Создание Дефаултдевицекомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="59879-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="59879-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59879-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59879-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59879-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59879-106">Создание нового объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="59879-106">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59879-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="59879-107">Prerequisites</span></span>
<span data-ttu-id="59879-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59879-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59879-110">Permission type</span></span>|<span data-ttu-id="59879-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59879-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59879-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59879-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59879-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59879-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59879-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59879-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59879-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59879-115">Not supported.</span></span>|
|<span data-ttu-id="59879-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="59879-116">Application</span></span>|<span data-ttu-id="59879-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59879-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59879-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59879-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="59879-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59879-119">Request headers</span></span>
|<span data-ttu-id="59879-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59879-120">Header</span></span>|<span data-ttu-id="59879-121">Значение</span><span class="sxs-lookup"><span data-stu-id="59879-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59879-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59879-122">Authorization</span></span>|<span data-ttu-id="59879-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59879-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59879-124">Accept</span><span class="sxs-lookup"><span data-stu-id="59879-124">Accept</span></span>|<span data-ttu-id="59879-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59879-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59879-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59879-126">Request body</span></span>
<span data-ttu-id="59879-127">В тексте запроса добавьте представление объекта Дефаултдевицекомплианцеполици в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59879-127">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="59879-128">В следующей таблице приведены свойства, необходимые при создании Дефаултдевицекомплианцеполици.</span><span class="sxs-lookup"><span data-stu-id="59879-128">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="59879-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="59879-129">Property</span></span>|<span data-ttu-id="59879-130">Тип</span><span class="sxs-lookup"><span data-stu-id="59879-130">Type</span></span>|<span data-ttu-id="59879-131">Описание</span><span class="sxs-lookup"><span data-stu-id="59879-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59879-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="59879-132">roleScopeTagIds</span></span>|<span data-ttu-id="59879-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="59879-133">String collection</span></span>|<span data-ttu-id="59879-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="59879-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="59879-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59879-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59879-136">id</span><span class="sxs-lookup"><span data-stu-id="59879-136">id</span></span>|<span data-ttu-id="59879-137">String</span><span class="sxs-lookup"><span data-stu-id="59879-137">String</span></span>|<span data-ttu-id="59879-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="59879-138">Key of the entity.</span></span> <span data-ttu-id="59879-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59879-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59879-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59879-140">createdDateTime</span></span>|<span data-ttu-id="59879-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59879-141">DateTimeOffset</span></span>|<span data-ttu-id="59879-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="59879-142">DateTime the object was created.</span></span> <span data-ttu-id="59879-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59879-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59879-144">description</span><span class="sxs-lookup"><span data-stu-id="59879-144">description</span></span>|<span data-ttu-id="59879-145">String</span><span class="sxs-lookup"><span data-stu-id="59879-145">String</span></span>|<span data-ttu-id="59879-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="59879-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="59879-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59879-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59879-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59879-148">lastModifiedDateTime</span></span>|<span data-ttu-id="59879-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59879-149">DateTimeOffset</span></span>|<span data-ttu-id="59879-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="59879-150">DateTime the object was last modified.</span></span> <span data-ttu-id="59879-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59879-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59879-152">displayName</span><span class="sxs-lookup"><span data-stu-id="59879-152">displayName</span></span>|<span data-ttu-id="59879-153">Строка</span><span class="sxs-lookup"><span data-stu-id="59879-153">String</span></span>|<span data-ttu-id="59879-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="59879-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="59879-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59879-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59879-156">version</span><span class="sxs-lookup"><span data-stu-id="59879-156">version</span></span>|<span data-ttu-id="59879-157">Int32</span><span class="sxs-lookup"><span data-stu-id="59879-157">Int32</span></span>|<span data-ttu-id="59879-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="59879-158">Version of the device configuration.</span></span> <span data-ttu-id="59879-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59879-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="59879-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="59879-160">Response</span></span>
<span data-ttu-id="59879-161">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59879-161">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59879-162">Пример</span><span class="sxs-lookup"><span data-stu-id="59879-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="59879-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="59879-163">Request</span></span>
<span data-ttu-id="59879-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59879-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59879-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="59879-165">Response</span></span>
<span data-ttu-id="59879-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59879-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






