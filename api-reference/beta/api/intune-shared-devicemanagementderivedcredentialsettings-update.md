---
title: Обновление deviceManagementDerivedCredentialSettings
description: Обновление свойств объекта deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f94ac3eb5328cd8723008a25fd72e30347a1ac9
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867856"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="6b41c-103">Обновление deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="6b41c-103">Update deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="6b41c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b41c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b41c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b41c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b41c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b41c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b41c-107">Обновление свойств объекта [deviceManagementDerivedCredentialSettings.](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6b41c-107">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b41c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6b41c-108">Prerequisites</span></span>
<span data-ttu-id="6b41c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b41c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b41c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b41c-111">Permission type</span></span>|<span data-ttu-id="6b41c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b41c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b41c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b41c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6b41c-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="6b41c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6b41c-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b41c-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="6b41c-116">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="6b41c-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="6b41c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b41c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b41c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b41c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b41c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b41c-119">Not supported.</span></span>|
|<span data-ttu-id="6b41c-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6b41c-120">Application</span></span>||
| <span data-ttu-id="6b41c-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="6b41c-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6b41c-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b41c-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="6b41c-123">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="6b41c-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="6b41c-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b41c-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b41c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b41c-125">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6b41c-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6b41c-126">Request headers</span></span>
|<span data-ttu-id="6b41c-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b41c-127">Header</span></span>|<span data-ttu-id="6b41c-128">Значение</span><span class="sxs-lookup"><span data-stu-id="6b41c-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b41c-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b41c-129">Authorization</span></span>|<span data-ttu-id="6b41c-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b41c-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b41c-131">Accept</span><span class="sxs-lookup"><span data-stu-id="6b41c-131">Accept</span></span>|<span data-ttu-id="6b41c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="6b41c-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b41c-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b41c-133">Request body</span></span>
<span data-ttu-id="6b41c-134">В теле запроса поставляем представление JSON для [объекта deviceManagementDerivedCredentialSettings.](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6b41c-134">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="6b41c-135">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementDerivedCredentialSettings.](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6b41c-135">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="6b41c-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b41c-136">Property</span></span>|<span data-ttu-id="6b41c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="6b41c-137">Type</span></span>|<span data-ttu-id="6b41c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6b41c-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b41c-139">id</span><span class="sxs-lookup"><span data-stu-id="6b41c-139">id</span></span>|<span data-ttu-id="6b41c-140">String</span><span class="sxs-lookup"><span data-stu-id="6b41c-140">String</span></span>|<span data-ttu-id="6b41c-141">Уникальный идентификатор для производных учетных данных</span><span class="sxs-lookup"><span data-stu-id="6b41c-141">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="6b41c-142">**Политика RA**</span><span class="sxs-lookup"><span data-stu-id="6b41c-142">**RA Policy**</span></span>|
|<span data-ttu-id="6b41c-143">helpUrl</span><span class="sxs-lookup"><span data-stu-id="6b41c-143">helpUrl</span></span>|<span data-ttu-id="6b41c-144">String</span><span class="sxs-lookup"><span data-stu-id="6b41c-144">String</span></span>|<span data-ttu-id="6b41c-145">URL-адрес, который будет доступен конечным пользователям по мере получения полученных учетных данных с помощью портала компании.</span><span class="sxs-lookup"><span data-stu-id="6b41c-145">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="6b41c-146">displayName</span><span class="sxs-lookup"><span data-stu-id="6b41c-146">displayName</span></span>|<span data-ttu-id="6b41c-147">String</span><span class="sxs-lookup"><span data-stu-id="6b41c-147">String</span></span>|<span data-ttu-id="6b41c-148">Имя отображения для профиля.</span><span class="sxs-lookup"><span data-stu-id="6b41c-148">The display name for the profile.</span></span>|
|<span data-ttu-id="6b41c-149">эмитент</span><span class="sxs-lookup"><span data-stu-id="6b41c-149">issuer</span></span>|[<span data-ttu-id="6b41c-150">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="6b41c-150">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-rapolicy-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="6b41c-151">Полученный поставщик учетных данных для использования.</span><span class="sxs-lookup"><span data-stu-id="6b41c-151">The derived credential provider to use.</span></span> <span data-ttu-id="6b41c-152">Возможные значения: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="6b41c-152">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="6b41c-153">notificationType</span><span class="sxs-lookup"><span data-stu-id="6b41c-153">notificationType</span></span>|[<span data-ttu-id="6b41c-154">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="6b41c-154">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-rapolicy-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="6b41c-155">Методы, используемые для информирования конечному пользователю об открытом портале компании для доставки профилей Wi-Fi, VPN или электронной почты, с помощью сертификатов на устройство.</span><span class="sxs-lookup"><span data-stu-id="6b41c-155">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="6b41c-156">Возможные значения: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="6b41c-156">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="6b41c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b41c-157">Response</span></span>
<span data-ttu-id="6b41c-158">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6b41c-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b41c-159">Пример</span><span class="sxs-lookup"><span data-stu-id="6b41c-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b41c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b41c-160">Request</span></span>
<span data-ttu-id="6b41c-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b41c-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="6b41c-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b41c-162">Response</span></span>
<span data-ttu-id="6b41c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b41c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```








