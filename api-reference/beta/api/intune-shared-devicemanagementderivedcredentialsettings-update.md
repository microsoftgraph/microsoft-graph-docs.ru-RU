---
title: Обновление Девицеманажементдериведкредентиалсеттингс
description: Обновление свойств объекта Девицеманажементдериведкредентиалсеттингс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8acef91bdb015c7bd65a5eaa81145e58f9132701
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43389827"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="49019-103">Обновление Девицеманажементдериведкредентиалсеттингс</span><span class="sxs-lookup"><span data-stu-id="49019-103">Update deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="49019-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49019-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49019-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49019-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49019-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49019-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49019-107">Обновление свойств объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="49019-107">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49019-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49019-108">Prerequisites</span></span>
<span data-ttu-id="49019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49019-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49019-111">Permission type</span></span>|<span data-ttu-id="49019-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49019-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49019-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49019-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="49019-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="49019-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="49019-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49019-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="49019-116">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="49019-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="49019-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49019-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49019-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49019-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49019-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49019-119">Not supported.</span></span>|
|<span data-ttu-id="49019-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="49019-120">Application</span></span>||
| <span data-ttu-id="49019-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="49019-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="49019-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49019-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="49019-123">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="49019-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="49019-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49019-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49019-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49019-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a><span data-ttu-id="49019-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49019-126">Request headers</span></span>
|<span data-ttu-id="49019-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49019-127">Header</span></span>|<span data-ttu-id="49019-128">Значение</span><span class="sxs-lookup"><span data-stu-id="49019-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49019-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="49019-129">Authorization</span></span>|<span data-ttu-id="49019-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49019-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49019-131">Accept</span><span class="sxs-lookup"><span data-stu-id="49019-131">Accept</span></span>|<span data-ttu-id="49019-132">application/json</span><span class="sxs-lookup"><span data-stu-id="49019-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49019-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49019-133">Request body</span></span>
<span data-ttu-id="49019-134">В тексте запроса добавьте представление объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49019-134">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="49019-135">В следующей таблице приведены свойства, необходимые при создании [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="49019-135">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="49019-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="49019-136">Property</span></span>|<span data-ttu-id="49019-137">Тип</span><span class="sxs-lookup"><span data-stu-id="49019-137">Type</span></span>|<span data-ttu-id="49019-138">Описание</span><span class="sxs-lookup"><span data-stu-id="49019-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49019-139">id</span><span class="sxs-lookup"><span data-stu-id="49019-139">id</span></span>|<span data-ttu-id="49019-140">String</span><span class="sxs-lookup"><span data-stu-id="49019-140">String</span></span>|<span data-ttu-id="49019-141">Уникальный идентификатор для производных учетных данных</span><span class="sxs-lookup"><span data-stu-id="49019-141">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="49019-142">**Политика RA**</span><span class="sxs-lookup"><span data-stu-id="49019-142">**RA Policy**</span></span>|
|<span data-ttu-id="49019-143">helpUrl</span><span class="sxs-lookup"><span data-stu-id="49019-143">helpUrl</span></span>|<span data-ttu-id="49019-144">String</span><span class="sxs-lookup"><span data-stu-id="49019-144">String</span></span>|<span data-ttu-id="49019-145">URL-адрес, который будет доступен конечным пользователям для получения производных учетных данных с помощью корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="49019-145">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="49019-146">displayName</span><span class="sxs-lookup"><span data-stu-id="49019-146">displayName</span></span>|<span data-ttu-id="49019-147">Строка</span><span class="sxs-lookup"><span data-stu-id="49019-147">String</span></span>|<span data-ttu-id="49019-148">Отображаемое имя профиля.</span><span class="sxs-lookup"><span data-stu-id="49019-148">The display name for the profile.</span></span>|
|<span data-ttu-id="49019-149">имени</span><span class="sxs-lookup"><span data-stu-id="49019-149">issuer</span></span>|<span data-ttu-id="49019-150">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="49019-150">deviceManagementDerivedCredentialIssuer</span></span>|<span data-ttu-id="49019-151">Производный поставщик учетных данных, который будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="49019-151">The derived credential provider to use.</span></span> <span data-ttu-id="49019-152">Возможные значения: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="49019-152">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="49019-153">notificationType</span><span class="sxs-lookup"><span data-stu-id="49019-153">notificationType</span></span>|<span data-ttu-id="49019-154">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="49019-154">deviceManagementDerivedCredentialNotificationType</span></span>|<span data-ttu-id="49019-155">Методы, используемые для информирования конечного пользователя об открытии корпоративного портала для доставки в сеть Wi-Fi, VPN или профилей электронной почты, использующих сертификаты для устройства.</span><span class="sxs-lookup"><span data-stu-id="49019-155">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="49019-156">Возможные значения: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="49019-156">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="49019-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="49019-157">Response</span></span>
<span data-ttu-id="49019-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49019-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49019-159">Пример</span><span class="sxs-lookup"><span data-stu-id="49019-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="49019-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="49019-160">Request</span></span>
<span data-ttu-id="49019-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49019-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="49019-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="49019-162">Response</span></span>
<span data-ttu-id="49019-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49019-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```







