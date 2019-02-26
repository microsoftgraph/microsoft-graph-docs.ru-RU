---
title: Создание Андроидомакпконфигуратион
description: Создание нового объекта Андроидомакпконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bed436668e2b77332f41a32dfe19f66895010249
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177821"
---
# <a name="create-androidomacpconfiguration"></a><span data-ttu-id="b172e-103">Создание Андроидомакпконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b172e-103">Create androidOmaCpConfiguration</span></span>

> <span data-ttu-id="b172e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b172e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b172e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b172e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b172e-106">Создание нового объекта [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b172e-106">Create a new [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b172e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b172e-107">Prerequisites</span></span>
<span data-ttu-id="b172e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b172e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b172e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b172e-110">Permission type</span></span>|<span data-ttu-id="b172e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b172e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b172e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b172e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b172e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b172e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b172e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b172e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b172e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b172e-115">Not supported.</span></span>|
|<span data-ttu-id="b172e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b172e-116">Application</span></span>|<span data-ttu-id="b172e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b172e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b172e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b172e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b172e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b172e-119">Request headers</span></span>
|<span data-ttu-id="b172e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b172e-120">Header</span></span>|<span data-ttu-id="b172e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b172e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b172e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b172e-122">Authorization</span></span>|<span data-ttu-id="b172e-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b172e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b172e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b172e-124">Accept</span></span>|<span data-ttu-id="b172e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b172e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b172e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b172e-126">Request body</span></span>
<span data-ttu-id="b172e-127">В тексте запроса добавьте представление объекта Андроидомакпконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b172e-127">In the request body, supply a JSON representation for the androidOmaCpConfiguration object.</span></span>

<span data-ttu-id="b172e-128">В следующей таблице приведены свойства, необходимые при создании Андроидомакпконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="b172e-128">The following table shows the properties that are required when you create the androidOmaCpConfiguration.</span></span>

|<span data-ttu-id="b172e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b172e-129">Property</span></span>|<span data-ttu-id="b172e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b172e-130">Type</span></span>|<span data-ttu-id="b172e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b172e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b172e-132">id</span><span class="sxs-lookup"><span data-stu-id="b172e-132">id</span></span>|<span data-ttu-id="b172e-133">String</span><span class="sxs-lookup"><span data-stu-id="b172e-133">String</span></span>|<span data-ttu-id="b172e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b172e-134">Key of the entity.</span></span> <span data-ttu-id="b172e-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b172e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b172e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b172e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b172e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b172e-137">DateTimeOffset</span></span>|<span data-ttu-id="b172e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b172e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b172e-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b172e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b172e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b172e-140">roleScopeTagIds</span></span>|<span data-ttu-id="b172e-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b172e-141">String collection</span></span>|<span data-ttu-id="b172e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b172e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b172e-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b172e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b172e-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b172e-144">supportsScopeTags</span></span>|<span data-ttu-id="b172e-145">Логический</span><span class="sxs-lookup"><span data-stu-id="b172e-145">Boolean</span></span>|<span data-ttu-id="b172e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b172e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b172e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b172e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b172e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b172e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b172e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b172e-149">This property is read-only.</span></span> <span data-ttu-id="b172e-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b172e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b172e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b172e-151">createdDateTime</span></span>|<span data-ttu-id="b172e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b172e-152">DateTimeOffset</span></span>|<span data-ttu-id="b172e-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b172e-153">DateTime the object was created.</span></span> <span data-ttu-id="b172e-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b172e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b172e-155">description</span><span class="sxs-lookup"><span data-stu-id="b172e-155">description</span></span>|<span data-ttu-id="b172e-156">String</span><span class="sxs-lookup"><span data-stu-id="b172e-156">String</span></span>|<span data-ttu-id="b172e-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b172e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b172e-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b172e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b172e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b172e-159">displayName</span></span>|<span data-ttu-id="b172e-160">String</span><span class="sxs-lookup"><span data-stu-id="b172e-160">String</span></span>|<span data-ttu-id="b172e-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b172e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b172e-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b172e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b172e-163">version</span><span class="sxs-lookup"><span data-stu-id="b172e-163">version</span></span>|<span data-ttu-id="b172e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b172e-164">Int32</span></span>|<span data-ttu-id="b172e-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b172e-165">Version of the device configuration.</span></span> <span data-ttu-id="b172e-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b172e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b172e-167">Конфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="b172e-167">configurationXml</span></span>|<span data-ttu-id="b172e-168">Binary</span><span class="sxs-lookup"><span data-stu-id="b172e-168">Binary</span></span>|<span data-ttu-id="b172e-169">XML-файл конфигурации, который будет применен к устройству.</span><span class="sxs-lookup"><span data-stu-id="b172e-169">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="b172e-170">При чтении она предоставляет только строку заполнителя, так как исходные данные шифруются и хранятся.</span><span class="sxs-lookup"><span data-stu-id="b172e-170">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="b172e-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="b172e-171">Response</span></span>
<span data-ttu-id="b172e-172">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b172e-172">If successful, this method returns a `201 Created` response code and a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b172e-173">Пример</span><span class="sxs-lookup"><span data-stu-id="b172e-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="b172e-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="b172e-174">Request</span></span>
<span data-ttu-id="b172e-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b172e-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="b172e-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="b172e-176">Response</span></span>
<span data-ttu-id="b172e-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b172e-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "5f682e4a-2e4a-5f68-4a2e-685f4a2e685f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```




