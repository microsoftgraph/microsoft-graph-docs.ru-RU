---
title: Создание iosImportedPFXCertificateProfile
description: Создание нового объекта iosImportedPFXCertificateProfile.
author: tfitzmac
ms.openlocfilehash: cc8bad7c884b7231502d5fbf8fbab06fa896f48d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305966"
---
# <a name="create-iosimportedpfxcertificateprofile"></a><span data-ttu-id="2cfae-103">Создание iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2cfae-103">Create iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="2cfae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2cfae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cfae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cfae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cfae-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2cfae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cfae-107">Создание нового объекта [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2cfae-107">Create a new [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2cfae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2cfae-108">Prerequisites</span></span>
<span data-ttu-id="2cfae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cfae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cfae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cfae-111">Permission type</span></span>|<span data-ttu-id="2cfae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cfae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cfae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cfae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cfae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cfae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cfae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cfae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cfae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cfae-116">Not supported.</span></span>|
|<span data-ttu-id="2cfae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cfae-117">Application</span></span>|<span data-ttu-id="2cfae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cfae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cfae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cfae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2cfae-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cfae-120">Request headers</span></span>
|<span data-ttu-id="2cfae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cfae-121">Header</span></span>|<span data-ttu-id="2cfae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2cfae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cfae-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cfae-123">Authorization</span></span>|<span data-ttu-id="2cfae-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2cfae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cfae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2cfae-125">Accept</span></span>|<span data-ttu-id="2cfae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cfae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cfae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cfae-127">Request body</span></span>
<span data-ttu-id="2cfae-128">В тексте запроса укажите представление JSON для объекта iosImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="2cfae-128">In the request body, supply a JSON representation for the iosImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="2cfae-129">В следующей таблице показаны свойства, которые необходимы для создания iosImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="2cfae-129">The following table shows the properties that are required when you create the iosImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="2cfae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cfae-130">Property</span></span>|<span data-ttu-id="2cfae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2cfae-131">Type</span></span>|<span data-ttu-id="2cfae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2cfae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cfae-133">id</span><span class="sxs-lookup"><span data-stu-id="2cfae-133">id</span></span>|<span data-ttu-id="2cfae-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2cfae-134">String</span></span>|<span data-ttu-id="2cfae-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2cfae-135">Key of the entity.</span></span> <span data-ttu-id="2cfae-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cfae-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cfae-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cfae-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2cfae-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cfae-138">DateTimeOffset</span></span>|<span data-ttu-id="2cfae-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2cfae-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2cfae-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cfae-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cfae-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2cfae-141">roleScopeTagIds</span></span>|<span data-ttu-id="2cfae-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2cfae-142">String collection</span></span>|<span data-ttu-id="2cfae-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2cfae-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2cfae-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cfae-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cfae-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2cfae-145">supportsScopeTags</span></span>|<span data-ttu-id="2cfae-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2cfae-146">Boolean</span></span>|<span data-ttu-id="2cfae-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="2cfae-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2cfae-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="2cfae-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2cfae-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2cfae-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2cfae-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2cfae-150">This property is read-only.</span></span> <span data-ttu-id="2cfae-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cfae-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cfae-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cfae-152">createdDateTime</span></span>|<span data-ttu-id="2cfae-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cfae-153">DateTimeOffset</span></span>|<span data-ttu-id="2cfae-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2cfae-154">DateTime the object was created.</span></span> <span data-ttu-id="2cfae-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cfae-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cfae-156">описание</span><span class="sxs-lookup"><span data-stu-id="2cfae-156">description</span></span>|<span data-ttu-id="2cfae-157">Строка</span><span class="sxs-lookup"><span data-stu-id="2cfae-157">String</span></span>|<span data-ttu-id="2cfae-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cfae-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2cfae-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cfae-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cfae-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2cfae-160">displayName</span></span>|<span data-ttu-id="2cfae-161">Строка</span><span class="sxs-lookup"><span data-stu-id="2cfae-161">String</span></span>|<span data-ttu-id="2cfae-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cfae-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2cfae-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cfae-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cfae-164">version</span><span class="sxs-lookup"><span data-stu-id="2cfae-164">version</span></span>|<span data-ttu-id="2cfae-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2cfae-165">Int32</span></span>|<span data-ttu-id="2cfae-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cfae-166">Version of the device configuration.</span></span> <span data-ttu-id="2cfae-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cfae-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cfae-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="2cfae-168">intendedPurpose</span></span>|[<span data-ttu-id="2cfae-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="2cfae-169">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="2cfae-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2cfae-170">Not yet documented.</span></span> <span data-ttu-id="2cfae-171">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="2cfae-171">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="2cfae-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cfae-172">Response</span></span>
<span data-ttu-id="2cfae-173">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2cfae-173">If successful, this method returns a `201 Created` response code and a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cfae-174">Пример</span><span class="sxs-lookup"><span data-stu-id="2cfae-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="2cfae-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cfae-175">Request</span></span>
<span data-ttu-id="2cfae-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cfae-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 367

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="2cfae-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cfae-177">Response</span></span>
<span data-ttu-id="2cfae-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2cfae-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```





