---
title: Создание Граупполицисеттингмаппинг
description: Создание нового объекта Граупполицисеттингмаппинг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35c568fcaee401f249923e047d25d874a9dbc0eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465452"
---
# <a name="create-grouppolicysettingmapping"></a><span data-ttu-id="a3dcd-103">Создание Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="a3dcd-103">Create groupPolicySettingMapping</span></span>

<span data-ttu-id="a3dcd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3dcd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3dcd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3dcd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3dcd-107">Создание нового объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="a3dcd-107">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3dcd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a3dcd-108">Prerequisites</span></span>
<span data-ttu-id="a3dcd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3dcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3dcd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3dcd-111">Permission type</span></span>|<span data-ttu-id="a3dcd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3dcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3dcd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3dcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3dcd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3dcd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3dcd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3dcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3dcd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-116">Not supported.</span></span>|
|<span data-ttu-id="a3dcd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3dcd-117">Application</span></span>|<span data-ttu-id="a3dcd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3dcd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3dcd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3dcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="a3dcd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a3dcd-120">Request headers</span></span>
|<span data-ttu-id="a3dcd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3dcd-121">Header</span></span>|<span data-ttu-id="a3dcd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3dcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3dcd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3dcd-123">Authorization</span></span>|<span data-ttu-id="a3dcd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3dcd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3dcd-125">Accept</span></span>|<span data-ttu-id="a3dcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3dcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3dcd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3dcd-127">Request body</span></span>
<span data-ttu-id="a3dcd-128">В тексте запроса добавьте представление объекта Граупполицисеттингмаппинг в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-128">In the request body, supply a JSON representation for the groupPolicySettingMapping object.</span></span>

<span data-ttu-id="a3dcd-129">В следующей таблице приведены свойства, необходимые при создании Граупполицисеттингмаппинг.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-129">The following table shows the properties that are required when you create the groupPolicySettingMapping.</span></span>

|<span data-ttu-id="a3dcd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3dcd-130">Property</span></span>|<span data-ttu-id="a3dcd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3dcd-131">Type</span></span>|<span data-ttu-id="a3dcd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3dcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3dcd-133">id</span><span class="sxs-lookup"><span data-stu-id="a3dcd-133">id</span></span>|<span data-ttu-id="a3dcd-134">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-134">String</span></span>|<span data-ttu-id="a3dcd-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-135">Not yet documented</span></span>|
|<span data-ttu-id="a3dcd-136">parentId</span><span class="sxs-lookup"><span data-stu-id="a3dcd-136">parentId</span></span>|<span data-ttu-id="a3dcd-137">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-137">String</span></span>|<span data-ttu-id="a3dcd-138">Родительский идентификатор параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="a3dcd-139">чилдидлист</span><span class="sxs-lookup"><span data-stu-id="a3dcd-139">childIdList</span></span>|<span data-ttu-id="a3dcd-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-140">String collection</span></span>|<span data-ttu-id="a3dcd-141">Список дочерних идентификаторов параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="a3dcd-142">settingName</span><span class="sxs-lookup"><span data-stu-id="a3dcd-142">settingName</span></span>|<span data-ttu-id="a3dcd-143">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-143">String</span></span>|<span data-ttu-id="a3dcd-144">Имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="a3dcd-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="a3dcd-145">settingValue</span></span>|<span data-ttu-id="a3dcd-146">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-146">String</span></span>|<span data-ttu-id="a3dcd-147">Значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="a3dcd-148">сеттингвалуетипе</span><span class="sxs-lookup"><span data-stu-id="a3dcd-148">settingValueType</span></span>|<span data-ttu-id="a3dcd-149">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-149">String</span></span>|<span data-ttu-id="a3dcd-150">Тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="a3dcd-151">сеттингдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="a3dcd-151">settingDisplayName</span></span>|<span data-ttu-id="a3dcd-152">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-152">String</span></span>|<span data-ttu-id="a3dcd-153">Отображаемое имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="a3dcd-154">сеттингдисплайвалуе</span><span class="sxs-lookup"><span data-stu-id="a3dcd-154">settingDisplayValue</span></span>|<span data-ttu-id="a3dcd-155">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-155">String</span></span>|<span data-ttu-id="a3dcd-156">Отображаемое значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="a3dcd-157">сеттингдисплайвалуетипе</span><span class="sxs-lookup"><span data-stu-id="a3dcd-157">settingDisplayValueType</span></span>|<span data-ttu-id="a3dcd-158">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-158">String</span></span>|<span data-ttu-id="a3dcd-159">Отображаемый тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="a3dcd-160">сеттингвалуедисплайунитс</span><span class="sxs-lookup"><span data-stu-id="a3dcd-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="a3dcd-161">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-161">String</span></span>|<span data-ttu-id="a3dcd-162">Отображаемые единицы значения параметра групповой политики</span><span class="sxs-lookup"><span data-stu-id="a3dcd-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="a3dcd-163">сеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="a3dcd-163">settingCategory</span></span>|<span data-ttu-id="a3dcd-164">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-164">String</span></span>|<span data-ttu-id="a3dcd-165">Категория, в которой находится параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="a3dcd-166">мдмкспнаме</span><span class="sxs-lookup"><span data-stu-id="a3dcd-166">mdmCspName</span></span>|<span data-ttu-id="a3dcd-167">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-167">String</span></span>|<span data-ttu-id="a3dcd-168">Имя CSP, которое сопоставляется параметру групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="a3dcd-169">мдмсеттингури</span><span class="sxs-lookup"><span data-stu-id="a3dcd-169">mdmSettingUri</span></span>|<span data-ttu-id="a3dcd-170">String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-170">String</span></span>|<span data-ttu-id="a3dcd-171">Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="a3dcd-172">мдмминимумосверсион</span><span class="sxs-lookup"><span data-stu-id="a3dcd-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="a3dcd-173">Int32</span><span class="sxs-lookup"><span data-stu-id="a3dcd-173">Int32</span></span>|<span data-ttu-id="a3dcd-174">Минимальная версия ОС, поддерживаемая параметром MDM.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="a3dcd-175">сеттингтипе</span><span class="sxs-lookup"><span data-stu-id="a3dcd-175">settingType</span></span>|[<span data-ttu-id="a3dcd-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="a3dcd-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="a3dcd-177">Тип параметра (Security или ADMX) групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="a3dcd-178">Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="a3dcd-179">исмдмсуппортед</span><span class="sxs-lookup"><span data-stu-id="a3dcd-179">isMdmSupported</span></span>|<span data-ttu-id="a3dcd-180">Логический</span><span class="sxs-lookup"><span data-stu-id="a3dcd-180">Boolean</span></span>|<span data-ttu-id="a3dcd-181">Указывает, поддерживается ли Intune или нет</span><span class="sxs-lookup"><span data-stu-id="a3dcd-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="a3dcd-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="a3dcd-182">mdmSupportedState</span></span>|[<span data-ttu-id="a3dcd-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="a3dcd-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="a3dcd-184">Указывает, поддерживается ли параметр в MDM.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="a3dcd-185">Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="a3dcd-186">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="a3dcd-186">settingScope</span></span>|[<span data-ttu-id="a3dcd-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="a3dcd-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="a3dcd-188">Область применения параметра.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-188">The scope of the setting.</span></span> <span data-ttu-id="a3dcd-189">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="a3dcd-190">интунесеттингурилист</span><span class="sxs-lookup"><span data-stu-id="a3dcd-190">intuneSettingUriList</span></span>|<span data-ttu-id="a3dcd-191">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3dcd-191">String collection</span></span>|<span data-ttu-id="a3dcd-192">Список URI параметров Intune, которые сопоставлены параметру групповой политики</span><span class="sxs-lookup"><span data-stu-id="a3dcd-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|



## <a name="response"></a><span data-ttu-id="a3dcd-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3dcd-193">Response</span></span>
<span data-ttu-id="a3dcd-194">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-194">If successful, this method returns a `201 Created` response code and a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3dcd-195">Пример</span><span class="sxs-lookup"><span data-stu-id="a3dcd-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3dcd-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3dcd-196">Request</span></span>
<span data-ttu-id="a3dcd-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
Content-type: application/json
Content-length: 887

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a3dcd-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3dcd-198">Response</span></span>
<span data-ttu-id="a3dcd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3dcd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 936

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```





