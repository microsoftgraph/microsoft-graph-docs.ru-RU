---
title: Создание объекта windowsPhone81CustomConfiguration
description: Создание объекта windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fe02cc2ab54753c9825bb007f480529c17cf8210
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991995"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="01d84-103">Создание объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="01d84-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="01d84-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01d84-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01d84-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01d84-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="01d84-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01d84-107">Создание объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d84-107">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01d84-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="01d84-108">Prerequisites</span></span>
<span data-ttu-id="01d84-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01d84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d84-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01d84-111">Permission type</span></span>|<span data-ttu-id="01d84-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01d84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01d84-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01d84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01d84-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d84-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01d84-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01d84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01d84-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d84-116">Not supported.</span></span>|
|<span data-ttu-id="01d84-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01d84-117">Application</span></span>|<span data-ttu-id="01d84-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d84-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01d84-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01d84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="01d84-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01d84-120">Request headers</span></span>
|<span data-ttu-id="01d84-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01d84-121">Header</span></span>|<span data-ttu-id="01d84-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01d84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01d84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01d84-123">Authorization</span></span>|<span data-ttu-id="01d84-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="01d84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01d84-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01d84-125">Accept</span></span>|<span data-ttu-id="01d84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01d84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01d84-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01d84-127">Request body</span></span>
<span data-ttu-id="01d84-128">В теле запроса добавьте представление объекта windowsPhone81CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01d84-128">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="01d84-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="01d84-129">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="01d84-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01d84-130">Property</span></span>|<span data-ttu-id="01d84-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01d84-131">Type</span></span>|<span data-ttu-id="01d84-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01d84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d84-133">id</span><span class="sxs-lookup"><span data-stu-id="01d84-133">id</span></span>|<span data-ttu-id="01d84-134">String</span><span class="sxs-lookup"><span data-stu-id="01d84-134">String</span></span>|<span data-ttu-id="01d84-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01d84-135">Key of the entity.</span></span> <span data-ttu-id="01d84-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d84-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d84-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01d84-137">lastModifiedDateTime</span></span>|<span data-ttu-id="01d84-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d84-138">DateTimeOffset</span></span>|<span data-ttu-id="01d84-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="01d84-139">DateTime the object was last modified.</span></span> <span data-ttu-id="01d84-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d84-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d84-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="01d84-141">roleScopeTagIds</span></span>|<span data-ttu-id="01d84-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="01d84-142">String collection</span></span>|<span data-ttu-id="01d84-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="01d84-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="01d84-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d84-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d84-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="01d84-145">supportsScopeTags</span></span>|<span data-ttu-id="01d84-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d84-146">Boolean</span></span>|<span data-ttu-id="01d84-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="01d84-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="01d84-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="01d84-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="01d84-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="01d84-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="01d84-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01d84-150">This property is read-only.</span></span> <span data-ttu-id="01d84-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d84-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d84-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01d84-152">createdDateTime</span></span>|<span data-ttu-id="01d84-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d84-153">DateTimeOffset</span></span>|<span data-ttu-id="01d84-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="01d84-154">DateTime the object was created.</span></span> <span data-ttu-id="01d84-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d84-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d84-156">описание</span><span class="sxs-lookup"><span data-stu-id="01d84-156">description</span></span>|<span data-ttu-id="01d84-157">String</span><span class="sxs-lookup"><span data-stu-id="01d84-157">String</span></span>|<span data-ttu-id="01d84-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01d84-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01d84-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d84-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d84-160">displayName</span><span class="sxs-lookup"><span data-stu-id="01d84-160">displayName</span></span>|<span data-ttu-id="01d84-161">String</span><span class="sxs-lookup"><span data-stu-id="01d84-161">String</span></span>|<span data-ttu-id="01d84-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01d84-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01d84-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d84-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d84-164">version</span><span class="sxs-lookup"><span data-stu-id="01d84-164">version</span></span>|<span data-ttu-id="01d84-165">Int32</span><span class="sxs-lookup"><span data-stu-id="01d84-165">Int32</span></span>|<span data-ttu-id="01d84-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01d84-166">Version of the device configuration.</span></span> <span data-ttu-id="01d84-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d84-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d84-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="01d84-168">omaSettings</span></span>|<span data-ttu-id="01d84-169">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="01d84-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="01d84-170">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="01d84-170">OMA settings.</span></span> <span data-ttu-id="01d84-171">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="01d84-171">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="01d84-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="01d84-172">Response</span></span>
<span data-ttu-id="01d84-173">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01d84-173">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01d84-174">Пример</span><span class="sxs-lookup"><span data-stu-id="01d84-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="01d84-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="01d84-175">Request</span></span>
<span data-ttu-id="01d84-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01d84-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="01d84-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="01d84-177">Response</span></span>
<span data-ttu-id="01d84-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="01d84-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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





