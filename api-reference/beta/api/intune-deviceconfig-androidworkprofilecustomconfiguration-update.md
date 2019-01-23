---
title: Обновление androidWorkProfileCustomConfiguration
description: Обновление свойства объекта androidWorkProfileCustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aa040b346adcaafadf5781b60c930011fea51ef7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414664"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="05dbe-103">Обновление androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="05dbe-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="05dbe-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05dbe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="05dbe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05dbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05dbe-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05dbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05dbe-107">Обновление свойства объекта [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="05dbe-107">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05dbe-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="05dbe-108">Prerequisites</span></span>
<span data-ttu-id="05dbe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="05dbe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05dbe-111">Permission type</span></span>|<span data-ttu-id="05dbe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05dbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05dbe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05dbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05dbe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05dbe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05dbe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05dbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05dbe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05dbe-116">Not supported.</span></span>|
|<span data-ttu-id="05dbe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05dbe-117">Application</span></span>|<span data-ttu-id="05dbe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05dbe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05dbe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05dbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="05dbe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05dbe-120">Request headers</span></span>
|<span data-ttu-id="05dbe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05dbe-121">Header</span></span>|<span data-ttu-id="05dbe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05dbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05dbe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05dbe-123">Authorization</span></span>|<span data-ttu-id="05dbe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="05dbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05dbe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05dbe-125">Accept</span></span>|<span data-ttu-id="05dbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05dbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05dbe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05dbe-127">Request body</span></span>
<span data-ttu-id="05dbe-128">В тексте запроса укажите представление JSON для объекта [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="05dbe-128">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="05dbe-129">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-129">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="05dbe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="05dbe-130">Property</span></span>|<span data-ttu-id="05dbe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="05dbe-131">Type</span></span>|<span data-ttu-id="05dbe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="05dbe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05dbe-133">id</span><span class="sxs-lookup"><span data-stu-id="05dbe-133">id</span></span>|<span data-ttu-id="05dbe-134">String</span><span class="sxs-lookup"><span data-stu-id="05dbe-134">String</span></span>|<span data-ttu-id="05dbe-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="05dbe-135">Key of the entity.</span></span> <span data-ttu-id="05dbe-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05dbe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05dbe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="05dbe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05dbe-138">DateTimeOffset</span></span>|<span data-ttu-id="05dbe-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="05dbe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="05dbe-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05dbe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="05dbe-141">roleScopeTagIds</span></span>|<span data-ttu-id="05dbe-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="05dbe-142">String collection</span></span>|<span data-ttu-id="05dbe-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="05dbe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="05dbe-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05dbe-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="05dbe-145">supportsScopeTags</span></span>|<span data-ttu-id="05dbe-146">Логический</span><span class="sxs-lookup"><span data-stu-id="05dbe-146">Boolean</span></span>|<span data-ttu-id="05dbe-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="05dbe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="05dbe-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="05dbe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="05dbe-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="05dbe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="05dbe-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05dbe-150">This property is read-only.</span></span> <span data-ttu-id="05dbe-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05dbe-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05dbe-152">createdDateTime</span></span>|<span data-ttu-id="05dbe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05dbe-153">DateTimeOffset</span></span>|<span data-ttu-id="05dbe-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="05dbe-154">DateTime the object was created.</span></span> <span data-ttu-id="05dbe-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05dbe-156">description</span><span class="sxs-lookup"><span data-stu-id="05dbe-156">description</span></span>|<span data-ttu-id="05dbe-157">String</span><span class="sxs-lookup"><span data-stu-id="05dbe-157">String</span></span>|<span data-ttu-id="05dbe-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="05dbe-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="05dbe-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05dbe-160">displayName</span><span class="sxs-lookup"><span data-stu-id="05dbe-160">displayName</span></span>|<span data-ttu-id="05dbe-161">String</span><span class="sxs-lookup"><span data-stu-id="05dbe-161">String</span></span>|<span data-ttu-id="05dbe-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="05dbe-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="05dbe-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05dbe-164">version</span><span class="sxs-lookup"><span data-stu-id="05dbe-164">version</span></span>|<span data-ttu-id="05dbe-165">Int32</span><span class="sxs-lookup"><span data-stu-id="05dbe-165">Int32</span></span>|<span data-ttu-id="05dbe-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="05dbe-166">Version of the device configuration.</span></span> <span data-ttu-id="05dbe-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05dbe-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05dbe-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="05dbe-168">omaSettings</span></span>|<span data-ttu-id="05dbe-169">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05dbe-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="05dbe-170">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="05dbe-170">OMA settings.</span></span> <span data-ttu-id="05dbe-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="05dbe-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="05dbe-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="05dbe-172">Response</span></span>
<span data-ttu-id="05dbe-173">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="05dbe-173">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05dbe-174">Пример</span><span class="sxs-lookup"><span data-stu-id="05dbe-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="05dbe-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="05dbe-175">Request</span></span>
<span data-ttu-id="05dbe-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05dbe-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 505

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="05dbe-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="05dbe-177">Response</span></span>
<span data-ttu-id="05dbe-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="05dbe-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 677

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




