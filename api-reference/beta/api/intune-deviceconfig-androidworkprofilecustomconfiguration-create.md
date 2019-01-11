---
title: Создание androidWorkProfileCustomConfiguration
description: Создание нового объекта androidWorkProfileCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b4e053e3c9d291c2e6c6edf965eee4bd95788e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870212"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="d8736-103">Создание androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8736-103">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="d8736-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8736-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8736-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8736-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8736-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d8736-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8736-107">Создание нового объекта [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8736-107">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8736-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d8736-108">Prerequisites</span></span>
<span data-ttu-id="d8736-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8736-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8736-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8736-111">Permission type</span></span>|<span data-ttu-id="d8736-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8736-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8736-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8736-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8736-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8736-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8736-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8736-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8736-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8736-116">Not supported.</span></span>|
|<span data-ttu-id="d8736-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8736-117">Application</span></span>|<span data-ttu-id="d8736-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8736-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8736-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8736-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d8736-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8736-120">Request headers</span></span>
|<span data-ttu-id="d8736-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8736-121">Header</span></span>|<span data-ttu-id="d8736-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d8736-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8736-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8736-123">Authorization</span></span>|<span data-ttu-id="d8736-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d8736-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8736-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8736-125">Accept</span></span>|<span data-ttu-id="d8736-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8736-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8736-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8736-127">Request body</span></span>
<span data-ttu-id="d8736-128">В тексте запроса укажите представление JSON для объекта androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d8736-128">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="d8736-129">В следующей таблице показаны свойства, которые необходимы для создания androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d8736-129">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="d8736-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8736-130">Property</span></span>|<span data-ttu-id="d8736-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d8736-131">Type</span></span>|<span data-ttu-id="d8736-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d8736-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8736-133">id</span><span class="sxs-lookup"><span data-stu-id="d8736-133">id</span></span>|<span data-ttu-id="d8736-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d8736-134">String</span></span>|<span data-ttu-id="d8736-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8736-135">Key of the entity.</span></span> <span data-ttu-id="d8736-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8736-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8736-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8736-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d8736-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8736-138">DateTimeOffset</span></span>|<span data-ttu-id="d8736-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d8736-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d8736-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8736-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8736-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8736-141">roleScopeTagIds</span></span>|<span data-ttu-id="d8736-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d8736-142">String collection</span></span>|<span data-ttu-id="d8736-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d8736-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d8736-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8736-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8736-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d8736-145">supportsScopeTags</span></span>|<span data-ttu-id="d8736-146">Логический</span><span class="sxs-lookup"><span data-stu-id="d8736-146">Boolean</span></span>|<span data-ttu-id="d8736-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="d8736-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d8736-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="d8736-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d8736-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d8736-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d8736-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8736-150">This property is read-only.</span></span> <span data-ttu-id="d8736-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8736-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8736-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8736-152">createdDateTime</span></span>|<span data-ttu-id="d8736-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8736-153">DateTimeOffset</span></span>|<span data-ttu-id="d8736-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d8736-154">DateTime the object was created.</span></span> <span data-ttu-id="d8736-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8736-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8736-156">описание</span><span class="sxs-lookup"><span data-stu-id="d8736-156">description</span></span>|<span data-ttu-id="d8736-157">Строка</span><span class="sxs-lookup"><span data-stu-id="d8736-157">String</span></span>|<span data-ttu-id="d8736-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d8736-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8736-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8736-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8736-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d8736-160">displayName</span></span>|<span data-ttu-id="d8736-161">Строка</span><span class="sxs-lookup"><span data-stu-id="d8736-161">String</span></span>|<span data-ttu-id="d8736-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d8736-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8736-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8736-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8736-164">version</span><span class="sxs-lookup"><span data-stu-id="d8736-164">version</span></span>|<span data-ttu-id="d8736-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d8736-165">Int32</span></span>|<span data-ttu-id="d8736-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d8736-166">Version of the device configuration.</span></span> <span data-ttu-id="d8736-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8736-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8736-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="d8736-168">omaSettings</span></span>|<span data-ttu-id="d8736-169">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d8736-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="d8736-170">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="d8736-170">OMA settings.</span></span> <span data-ttu-id="d8736-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d8736-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d8736-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8736-172">Response</span></span>
<span data-ttu-id="d8736-173">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d8736-173">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8736-174">Пример</span><span class="sxs-lookup"><span data-stu-id="d8736-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8736-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8736-175">Request</span></span>
<span data-ttu-id="d8736-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8736-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 569

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="d8736-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8736-177">Response</span></span>
<span data-ttu-id="d8736-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d8736-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





