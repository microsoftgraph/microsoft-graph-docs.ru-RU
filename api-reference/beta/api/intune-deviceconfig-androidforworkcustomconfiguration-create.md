---
title: Создание androidForWorkCustomConfiguration
description: Создание нового объекта androidForWorkCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 91cb94c49bd3fd1a9a25ec6efd77fdabd669dc81
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326798"
---
# <a name="create-androidforworkcustomconfiguration"></a><span data-ttu-id="c74f0-103">Создание androidForWorkCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c74f0-103">Create androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="c74f0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c74f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c74f0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c74f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c74f0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c74f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c74f0-107">Создание нового объекта [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c74f0-107">Create a new [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c74f0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c74f0-108">Prerequisites</span></span>
<span data-ttu-id="c74f0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c74f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c74f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c74f0-111">Permission type</span></span>|<span data-ttu-id="c74f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c74f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c74f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c74f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c74f0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c74f0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c74f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c74f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c74f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c74f0-116">Not supported.</span></span>|
|<span data-ttu-id="c74f0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c74f0-117">Application</span></span>|<span data-ttu-id="c74f0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c74f0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c74f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c74f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c74f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c74f0-120">Request headers</span></span>
|<span data-ttu-id="c74f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c74f0-121">Header</span></span>|<span data-ttu-id="c74f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c74f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c74f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c74f0-123">Authorization</span></span>|<span data-ttu-id="c74f0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c74f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c74f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c74f0-125">Accept</span></span>|<span data-ttu-id="c74f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c74f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c74f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c74f0-127">Request body</span></span>
<span data-ttu-id="c74f0-128">В тексте запроса укажите представление JSON для объекта androidForWorkCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c74f0-128">In the request body, supply a JSON representation for the androidForWorkCustomConfiguration object.</span></span>

<span data-ttu-id="c74f0-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c74f0-129">The following table shows the properties that are required when you create the androidForWorkCustomConfiguration.</span></span>

|<span data-ttu-id="c74f0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c74f0-130">Property</span></span>|<span data-ttu-id="c74f0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c74f0-131">Type</span></span>|<span data-ttu-id="c74f0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c74f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c74f0-133">id</span><span class="sxs-lookup"><span data-stu-id="c74f0-133">id</span></span>|<span data-ttu-id="c74f0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c74f0-134">String</span></span>|<span data-ttu-id="c74f0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c74f0-135">Key of the entity.</span></span> <span data-ttu-id="c74f0-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c74f0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c74f0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c74f0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c74f0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c74f0-138">DateTimeOffset</span></span>|<span data-ttu-id="c74f0-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c74f0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c74f0-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c74f0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c74f0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c74f0-141">roleScopeTagIds</span></span>|<span data-ttu-id="c74f0-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c74f0-142">String collection</span></span>|<span data-ttu-id="c74f0-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c74f0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c74f0-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c74f0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c74f0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c74f0-145">supportsScopeTags</span></span>|<span data-ttu-id="c74f0-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c74f0-146">Boolean</span></span>|<span data-ttu-id="c74f0-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="c74f0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c74f0-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="c74f0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c74f0-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c74f0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c74f0-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c74f0-150">This property is read-only.</span></span> <span data-ttu-id="c74f0-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c74f0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c74f0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c74f0-152">createdDateTime</span></span>|<span data-ttu-id="c74f0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c74f0-153">DateTimeOffset</span></span>|<span data-ttu-id="c74f0-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c74f0-154">DateTime the object was created.</span></span> <span data-ttu-id="c74f0-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c74f0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c74f0-156">описание</span><span class="sxs-lookup"><span data-stu-id="c74f0-156">description</span></span>|<span data-ttu-id="c74f0-157">Строка</span><span class="sxs-lookup"><span data-stu-id="c74f0-157">String</span></span>|<span data-ttu-id="c74f0-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c74f0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c74f0-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c74f0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c74f0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c74f0-160">displayName</span></span>|<span data-ttu-id="c74f0-161">Строка</span><span class="sxs-lookup"><span data-stu-id="c74f0-161">String</span></span>|<span data-ttu-id="c74f0-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c74f0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c74f0-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c74f0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c74f0-164">version</span><span class="sxs-lookup"><span data-stu-id="c74f0-164">version</span></span>|<span data-ttu-id="c74f0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c74f0-165">Int32</span></span>|<span data-ttu-id="c74f0-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c74f0-166">Version of the device configuration.</span></span> <span data-ttu-id="c74f0-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c74f0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c74f0-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="c74f0-168">omaSettings</span></span>|<span data-ttu-id="c74f0-169">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c74f0-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="c74f0-170">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="c74f0-170">OMA settings.</span></span> <span data-ttu-id="c74f0-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c74f0-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c74f0-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="c74f0-172">Response</span></span>
<span data-ttu-id="c74f0-173">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c74f0-173">If successful, this method returns a `201 Created` response code and a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c74f0-174">Пример</span><span class="sxs-lookup"><span data-stu-id="c74f0-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="c74f0-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="c74f0-175">Request</span></span>
<span data-ttu-id="c74f0-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c74f0-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="c74f0-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="c74f0-177">Response</span></span>
<span data-ttu-id="c74f0-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c74f0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
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





