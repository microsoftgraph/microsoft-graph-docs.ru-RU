---
title: Создание Граупполицисеттингмаппинг
description: Создание нового объекта Граупполицисеттингмаппинг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8e6a557bebac11004b5548bc90d931356ba852d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943272"
---
# <a name="create-grouppolicysettingmapping"></a><span data-ttu-id="8bf09-103">Создание Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="8bf09-103">Create groupPolicySettingMapping</span></span>

> <span data-ttu-id="8bf09-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bf09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bf09-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bf09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bf09-106">Создание нового объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="8bf09-106">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bf09-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8bf09-107">Prerequisites</span></span>
<span data-ttu-id="8bf09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bf09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bf09-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bf09-110">Permission type</span></span>|<span data-ttu-id="8bf09-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bf09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bf09-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bf09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bf09-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bf09-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bf09-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bf09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bf09-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bf09-115">Not supported.</span></span>|
|<span data-ttu-id="8bf09-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bf09-116">Application</span></span>|<span data-ttu-id="8bf09-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bf09-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bf09-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bf09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="8bf09-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8bf09-119">Request headers</span></span>
|<span data-ttu-id="8bf09-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bf09-120">Header</span></span>|<span data-ttu-id="8bf09-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8bf09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bf09-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bf09-122">Authorization</span></span>|<span data-ttu-id="8bf09-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bf09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bf09-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8bf09-124">Accept</span></span>|<span data-ttu-id="8bf09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8bf09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bf09-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8bf09-126">Request body</span></span>
<span data-ttu-id="8bf09-127">В тексте запроса добавьте представление объекта Граупполицисеттингмаппинг в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bf09-127">In the request body, supply a JSON representation for the groupPolicySettingMapping object.</span></span>

<span data-ttu-id="8bf09-128">В следующей таблице приведены свойства, необходимые при создании Граупполицисеттингмаппинг.</span><span class="sxs-lookup"><span data-stu-id="8bf09-128">The following table shows the properties that are required when you create the groupPolicySettingMapping.</span></span>

|<span data-ttu-id="8bf09-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bf09-129">Property</span></span>|<span data-ttu-id="8bf09-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8bf09-130">Type</span></span>|<span data-ttu-id="8bf09-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8bf09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bf09-132">id</span><span class="sxs-lookup"><span data-stu-id="8bf09-132">id</span></span>|<span data-ttu-id="8bf09-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-133">String</span></span>|<span data-ttu-id="8bf09-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8bf09-134">Not yet documented</span></span>|
|<span data-ttu-id="8bf09-135">parentId</span><span class="sxs-lookup"><span data-stu-id="8bf09-135">parentId</span></span>|<span data-ttu-id="8bf09-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-136">String</span></span>|<span data-ttu-id="8bf09-137">Родительский идентификатор параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-137">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="8bf09-138">чилдидлист</span><span class="sxs-lookup"><span data-stu-id="8bf09-138">childIdList</span></span>|<span data-ttu-id="8bf09-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8bf09-139">String collection</span></span>|<span data-ttu-id="8bf09-140">Список дочерних идентификаторов параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-140">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="8bf09-141">settingName</span><span class="sxs-lookup"><span data-stu-id="8bf09-141">settingName</span></span>|<span data-ttu-id="8bf09-142">String</span><span class="sxs-lookup"><span data-stu-id="8bf09-142">String</span></span>|<span data-ttu-id="8bf09-143">Имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-143">The name of this group policy setting.</span></span>|
|<span data-ttu-id="8bf09-144">settingValue</span><span class="sxs-lookup"><span data-stu-id="8bf09-144">settingValue</span></span>|<span data-ttu-id="8bf09-145">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-145">String</span></span>|<span data-ttu-id="8bf09-146">Значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-146">The value of this group policy setting.</span></span>|
|<span data-ttu-id="8bf09-147">сеттингвалуетипе</span><span class="sxs-lookup"><span data-stu-id="8bf09-147">settingValueType</span></span>|<span data-ttu-id="8bf09-148">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-148">String</span></span>|<span data-ttu-id="8bf09-149">Тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-149">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="8bf09-150">сеттингдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="8bf09-150">settingDisplayName</span></span>|<span data-ttu-id="8bf09-151">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-151">String</span></span>|<span data-ttu-id="8bf09-152">Отображаемое имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-152">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="8bf09-153">сеттингдисплайвалуе</span><span class="sxs-lookup"><span data-stu-id="8bf09-153">settingDisplayValue</span></span>|<span data-ttu-id="8bf09-154">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-154">String</span></span>|<span data-ttu-id="8bf09-155">Отображаемое значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-155">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="8bf09-156">сеттингдисплайвалуетипе</span><span class="sxs-lookup"><span data-stu-id="8bf09-156">settingDisplayValueType</span></span>|<span data-ttu-id="8bf09-157">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-157">String</span></span>|<span data-ttu-id="8bf09-158">Отображаемый тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-158">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="8bf09-159">сеттингвалуедисплайунитс</span><span class="sxs-lookup"><span data-stu-id="8bf09-159">settingValueDisplayUnits</span></span>|<span data-ttu-id="8bf09-160">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-160">String</span></span>|<span data-ttu-id="8bf09-161">Отображаемые единицы значения параметра групповой политики</span><span class="sxs-lookup"><span data-stu-id="8bf09-161">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="8bf09-162">сеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="8bf09-162">settingCategory</span></span>|<span data-ttu-id="8bf09-163">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-163">String</span></span>|<span data-ttu-id="8bf09-164">Категория, в которой находится параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-164">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="8bf09-165">мдмкспнаме</span><span class="sxs-lookup"><span data-stu-id="8bf09-165">mdmCspName</span></span>|<span data-ttu-id="8bf09-166">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-166">String</span></span>|<span data-ttu-id="8bf09-167">Имя CSP, которое сопоставляется параметру групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-167">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="8bf09-168">мдмсеттингури</span><span class="sxs-lookup"><span data-stu-id="8bf09-168">mdmSettingUri</span></span>|<span data-ttu-id="8bf09-169">Строка</span><span class="sxs-lookup"><span data-stu-id="8bf09-169">String</span></span>|<span data-ttu-id="8bf09-170">Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-170">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="8bf09-171">мдмминимумосверсион</span><span class="sxs-lookup"><span data-stu-id="8bf09-171">mdmMinimumOSVersion</span></span>|<span data-ttu-id="8bf09-172">Int32</span><span class="sxs-lookup"><span data-stu-id="8bf09-172">Int32</span></span>|<span data-ttu-id="8bf09-173">Минимальная версия ОС, поддерживаемая параметром MDM.</span><span class="sxs-lookup"><span data-stu-id="8bf09-173">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="8bf09-174">сеттингтипе</span><span class="sxs-lookup"><span data-stu-id="8bf09-174">settingType</span></span>|[<span data-ttu-id="8bf09-175">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="8bf09-175">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="8bf09-176">Тип параметра (Security или ADMX) групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bf09-176">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="8bf09-177">Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="8bf09-177">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="8bf09-178">исмдмсуппортед</span><span class="sxs-lookup"><span data-stu-id="8bf09-178">isMdmSupported</span></span>|<span data-ttu-id="8bf09-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bf09-179">Boolean</span></span>|<span data-ttu-id="8bf09-180">Указывает, поддерживается ли Intune или нет</span><span class="sxs-lookup"><span data-stu-id="8bf09-180">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="8bf09-181">мдмсуппортедстате</span><span class="sxs-lookup"><span data-stu-id="8bf09-181">mdmSupportedState</span></span>|[<span data-ttu-id="8bf09-182">мдмсуппортедстате</span><span class="sxs-lookup"><span data-stu-id="8bf09-182">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="8bf09-183">Указывает, поддерживается ли параметр в MDM.</span><span class="sxs-lookup"><span data-stu-id="8bf09-183">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="8bf09-184">Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="8bf09-184">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="8bf09-185">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="8bf09-185">settingScope</span></span>|[<span data-ttu-id="8bf09-186">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="8bf09-186">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="8bf09-187">Область применения параметра.</span><span class="sxs-lookup"><span data-stu-id="8bf09-187">The scope of the setting.</span></span> <span data-ttu-id="8bf09-188">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="8bf09-188">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="8bf09-189">интунесеттингурилист</span><span class="sxs-lookup"><span data-stu-id="8bf09-189">intuneSettingUriList</span></span>|<span data-ttu-id="8bf09-190">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8bf09-190">String collection</span></span>|<span data-ttu-id="8bf09-191">Список URI параметров Intune, которые сопоставлены параметру групповой политики</span><span class="sxs-lookup"><span data-stu-id="8bf09-191">The list of Intune Setting URIs this group policy setting maps to</span></span>|



## <a name="response"></a><span data-ttu-id="8bf09-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="8bf09-192">Response</span></span>
<span data-ttu-id="8bf09-193">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8bf09-193">If successful, this method returns a `201 Created` response code and a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bf09-194">Пример</span><span class="sxs-lookup"><span data-stu-id="8bf09-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bf09-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bf09-195">Request</span></span>
<span data-ttu-id="8bf09-196">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bf09-196">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8bf09-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bf09-197">Response</span></span>
<span data-ttu-id="8bf09-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bf09-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





