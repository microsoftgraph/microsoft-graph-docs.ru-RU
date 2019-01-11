---
title: Создание windows10PFXImportCertificateProfile
description: Создание нового объекта windows10PFXImportCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5342d1184125497eeab39794c01c51c82327644d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822815"
---
# <a name="create-windows10pfximportcertificateprofile"></a><span data-ttu-id="35fc3-103">Создание windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="35fc3-103">Create windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="35fc3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35fc3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35fc3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35fc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35fc3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35fc3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35fc3-107">Создание нового объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="35fc3-107">Create a new [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35fc3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35fc3-108">Prerequisites</span></span>
<span data-ttu-id="35fc3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35fc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35fc3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35fc3-111">Permission type</span></span>|<span data-ttu-id="35fc3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35fc3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35fc3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35fc3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35fc3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35fc3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35fc3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35fc3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35fc3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35fc3-116">Not supported.</span></span>|
|<span data-ttu-id="35fc3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35fc3-117">Application</span></span>|<span data-ttu-id="35fc3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35fc3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35fc3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35fc3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="35fc3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35fc3-120">Request headers</span></span>
|<span data-ttu-id="35fc3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35fc3-121">Header</span></span>|<span data-ttu-id="35fc3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="35fc3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35fc3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35fc3-123">Authorization</span></span>|<span data-ttu-id="35fc3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="35fc3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35fc3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="35fc3-125">Accept</span></span>|<span data-ttu-id="35fc3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35fc3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35fc3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35fc3-127">Request body</span></span>
<span data-ttu-id="35fc3-128">В тексте запроса укажите представление JSON для объекта windows10PFXImportCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="35fc3-128">In the request body, supply a JSON representation for the windows10PFXImportCertificateProfile object.</span></span>

<span data-ttu-id="35fc3-129">В следующей таблице показаны свойства, которые необходимы для создания windows10PFXImportCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="35fc3-129">The following table shows the properties that are required when you create the windows10PFXImportCertificateProfile.</span></span>

|<span data-ttu-id="35fc3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="35fc3-130">Property</span></span>|<span data-ttu-id="35fc3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="35fc3-131">Type</span></span>|<span data-ttu-id="35fc3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="35fc3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35fc3-133">id</span><span class="sxs-lookup"><span data-stu-id="35fc3-133">id</span></span>|<span data-ttu-id="35fc3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="35fc3-134">String</span></span>|<span data-ttu-id="35fc3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="35fc3-135">Key of the entity.</span></span> <span data-ttu-id="35fc3-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35fc3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35fc3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35fc3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="35fc3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35fc3-138">DateTimeOffset</span></span>|<span data-ttu-id="35fc3-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="35fc3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="35fc3-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35fc3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35fc3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35fc3-141">roleScopeTagIds</span></span>|<span data-ttu-id="35fc3-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="35fc3-142">String collection</span></span>|<span data-ttu-id="35fc3-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="35fc3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="35fc3-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35fc3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35fc3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="35fc3-145">supportsScopeTags</span></span>|<span data-ttu-id="35fc3-146">Логический</span><span class="sxs-lookup"><span data-stu-id="35fc3-146">Boolean</span></span>|<span data-ttu-id="35fc3-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="35fc3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="35fc3-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="35fc3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="35fc3-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="35fc3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="35fc3-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35fc3-150">This property is read-only.</span></span> <span data-ttu-id="35fc3-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35fc3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35fc3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35fc3-152">createdDateTime</span></span>|<span data-ttu-id="35fc3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35fc3-153">DateTimeOffset</span></span>|<span data-ttu-id="35fc3-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="35fc3-154">DateTime the object was created.</span></span> <span data-ttu-id="35fc3-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35fc3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35fc3-156">описание</span><span class="sxs-lookup"><span data-stu-id="35fc3-156">description</span></span>|<span data-ttu-id="35fc3-157">Строка</span><span class="sxs-lookup"><span data-stu-id="35fc3-157">String</span></span>|<span data-ttu-id="35fc3-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="35fc3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="35fc3-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35fc3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35fc3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="35fc3-160">displayName</span></span>|<span data-ttu-id="35fc3-161">Строка</span><span class="sxs-lookup"><span data-stu-id="35fc3-161">String</span></span>|<span data-ttu-id="35fc3-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="35fc3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="35fc3-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35fc3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35fc3-164">version</span><span class="sxs-lookup"><span data-stu-id="35fc3-164">version</span></span>|<span data-ttu-id="35fc3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="35fc3-165">Int32</span></span>|<span data-ttu-id="35fc3-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="35fc3-166">Version of the device configuration.</span></span> <span data-ttu-id="35fc3-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35fc3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35fc3-168">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="35fc3-168">keyStorageProvider</span></span>|[<span data-ttu-id="35fc3-169">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="35fc3-169">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="35fc3-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="35fc3-170">Not yet documented.</span></span> <span data-ttu-id="35fc3-171">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="35fc3-171">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="35fc3-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="35fc3-172">Response</span></span>
<span data-ttu-id="35fc3-173">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="35fc3-173">If successful, this method returns a `201 Created` response code and a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35fc3-174">Пример</span><span class="sxs-lookup"><span data-stu-id="35fc3-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="35fc3-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="35fc3-175">Request</span></span>
<span data-ttu-id="35fc3-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35fc3-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 381

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="35fc3-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="35fc3-177">Response</span></span>
<span data-ttu-id="35fc3-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="35fc3-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```





