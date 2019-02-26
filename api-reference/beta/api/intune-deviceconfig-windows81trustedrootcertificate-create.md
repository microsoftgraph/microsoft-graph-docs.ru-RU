---
title: Создание windows81TrustedRootCertificate
description: Создание нового объекта windows81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17160a20cc6a0afb7ed7d87e99af088c98d585db
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150367"
---
# <a name="create-windows81trustedrootcertificate"></a><span data-ttu-id="d7ad5-103">Создание windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d7ad5-103">Create windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="d7ad5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7ad5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7ad5-106">Создание нового объекта [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d7ad5-106">Create a new [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7ad5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7ad5-107">Prerequisites</span></span>
<span data-ttu-id="d7ad5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7ad5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d7ad5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7ad5-110">Permission type</span></span>|<span data-ttu-id="d7ad5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7ad5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7ad5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7ad5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7ad5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7ad5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7ad5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7ad5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7ad5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-115">Not supported.</span></span>|
|<span data-ttu-id="d7ad5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7ad5-116">Application</span></span>|<span data-ttu-id="d7ad5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7ad5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7ad5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="d7ad5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7ad5-119">Request headers</span></span>
|<span data-ttu-id="d7ad5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7ad5-120">Header</span></span>|<span data-ttu-id="d7ad5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d7ad5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7ad5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7ad5-122">Authorization</span></span>|<span data-ttu-id="d7ad5-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d7ad5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7ad5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d7ad5-124">Accept</span></span>|<span data-ttu-id="d7ad5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7ad5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7ad5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7ad5-126">Request body</span></span>
<span data-ttu-id="d7ad5-127">В тексте запроса добавьте представление объекта windows81TrustedRootCertificate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-127">In the request body, supply a JSON representation for the windows81TrustedRootCertificate object.</span></span>

<span data-ttu-id="d7ad5-128">В следующей таблице приведены свойства, необходимые при создании windows81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-128">The following table shows the properties that are required when you create the windows81TrustedRootCertificate.</span></span>

|<span data-ttu-id="d7ad5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7ad5-129">Property</span></span>|<span data-ttu-id="d7ad5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d7ad5-130">Type</span></span>|<span data-ttu-id="d7ad5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d7ad5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7ad5-132">id</span><span class="sxs-lookup"><span data-stu-id="d7ad5-132">id</span></span>|<span data-ttu-id="d7ad5-133">String</span><span class="sxs-lookup"><span data-stu-id="d7ad5-133">String</span></span>|<span data-ttu-id="d7ad5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-134">Key of the entity.</span></span> <span data-ttu-id="d7ad5-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ad5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ad5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7ad5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d7ad5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ad5-137">DateTimeOffset</span></span>|<span data-ttu-id="d7ad5-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d7ad5-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ad5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ad5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7ad5-140">roleScopeTagIds</span></span>|<span data-ttu-id="d7ad5-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d7ad5-141">String collection</span></span>|<span data-ttu-id="d7ad5-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d7ad5-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ad5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ad5-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d7ad5-144">supportsScopeTags</span></span>|<span data-ttu-id="d7ad5-145">Логический</span><span class="sxs-lookup"><span data-stu-id="d7ad5-145">Boolean</span></span>|<span data-ttu-id="d7ad5-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d7ad5-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d7ad5-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d7ad5-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-149">This property is read-only.</span></span> <span data-ttu-id="d7ad5-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ad5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ad5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7ad5-151">createdDateTime</span></span>|<span data-ttu-id="d7ad5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ad5-152">DateTimeOffset</span></span>|<span data-ttu-id="d7ad5-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-153">DateTime the object was created.</span></span> <span data-ttu-id="d7ad5-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ad5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ad5-155">description</span><span class="sxs-lookup"><span data-stu-id="d7ad5-155">description</span></span>|<span data-ttu-id="d7ad5-156">String</span><span class="sxs-lookup"><span data-stu-id="d7ad5-156">String</span></span>|<span data-ttu-id="d7ad5-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d7ad5-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ad5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ad5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d7ad5-159">displayName</span></span>|<span data-ttu-id="d7ad5-160">String</span><span class="sxs-lookup"><span data-stu-id="d7ad5-160">String</span></span>|<span data-ttu-id="d7ad5-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d7ad5-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ad5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ad5-163">version</span><span class="sxs-lookup"><span data-stu-id="d7ad5-163">version</span></span>|<span data-ttu-id="d7ad5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d7ad5-164">Int32</span></span>|<span data-ttu-id="d7ad5-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-165">Version of the device configuration.</span></span> <span data-ttu-id="d7ad5-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ad5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ad5-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d7ad5-167">trustedRootCertificate</span></span>|<span data-ttu-id="d7ad5-168">Binary</span><span class="sxs-lookup"><span data-stu-id="d7ad5-168">Binary</span></span>|<span data-ttu-id="d7ad5-169">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="d7ad5-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="d7ad5-170">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="d7ad5-170">certFileName</span></span>|<span data-ttu-id="d7ad5-171">String</span><span class="sxs-lookup"><span data-stu-id="d7ad5-171">String</span></span>|<span data-ttu-id="d7ad5-172">Имя файла, отображаемое в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-172">File name to display in UI.</span></span>|
|<span data-ttu-id="d7ad5-173">Дестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="d7ad5-173">destinationStore</span></span>|[<span data-ttu-id="d7ad5-174">Цертификатедестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="d7ad5-174">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="d7ad5-175">Расположение хранилища назначения для доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-175">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="d7ad5-176">Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-176">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="d7ad5-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7ad5-177">Response</span></span>
<span data-ttu-id="d7ad5-178">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-178">If successful, this method returns a `201 Created` response code and a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7ad5-179">Пример</span><span class="sxs-lookup"><span data-stu-id="d7ad5-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7ad5-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7ad5-180">Request</span></span>
<span data-ttu-id="d7ad5-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
Content-type: application/json
Content-length: 425

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="d7ad5-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7ad5-182">Response</span></span>
<span data-ttu-id="d7ad5-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d7ad5-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 597

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




