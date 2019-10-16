---
title: Обновление Граупполицисеттингмаппинг
description: Обновление свойств объекта Граупполицисеттингмаппинг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ceda370eafffa0937323585ca85bd94359ac027a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535746"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="dc9d2-103">Обновление Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="dc9d2-103">Update groupPolicySettingMapping</span></span>

> <span data-ttu-id="dc9d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc9d2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc9d2-106">Обновление свойств объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="dc9d2-106">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc9d2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dc9d2-107">Prerequisites</span></span>
<span data-ttu-id="dc9d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc9d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc9d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc9d2-110">Permission type</span></span>|<span data-ttu-id="dc9d2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc9d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc9d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc9d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc9d2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc9d2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc9d2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc9d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc9d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-115">Not supported.</span></span>|
|<span data-ttu-id="dc9d2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="dc9d2-116">Application</span></span>|<span data-ttu-id="dc9d2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc9d2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc9d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc9d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="dc9d2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc9d2-119">Request headers</span></span>
|<span data-ttu-id="dc9d2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc9d2-120">Header</span></span>|<span data-ttu-id="dc9d2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dc9d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc9d2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc9d2-122">Authorization</span></span>|<span data-ttu-id="dc9d2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc9d2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dc9d2-124">Accept</span></span>|<span data-ttu-id="dc9d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc9d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc9d2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc9d2-126">Request body</span></span>
<span data-ttu-id="dc9d2-127">В тексте запроса добавьте представление объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-127">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="dc9d2-128">В следующей таблице приведены свойства, необходимые при создании [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span><span class="sxs-lookup"><span data-stu-id="dc9d2-128">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="dc9d2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc9d2-129">Property</span></span>|<span data-ttu-id="dc9d2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dc9d2-130">Type</span></span>|<span data-ttu-id="dc9d2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dc9d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc9d2-132">id</span><span class="sxs-lookup"><span data-stu-id="dc9d2-132">id</span></span>|<span data-ttu-id="dc9d2-133">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-133">String</span></span>|<span data-ttu-id="dc9d2-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-134">Not yet documented</span></span>|
|<span data-ttu-id="dc9d2-135">parentId</span><span class="sxs-lookup"><span data-stu-id="dc9d2-135">parentId</span></span>|<span data-ttu-id="dc9d2-136">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-136">String</span></span>|<span data-ttu-id="dc9d2-137">Родительский идентификатор параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-137">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="dc9d2-138">чилдидлист</span><span class="sxs-lookup"><span data-stu-id="dc9d2-138">childIdList</span></span>|<span data-ttu-id="dc9d2-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-139">String collection</span></span>|<span data-ttu-id="dc9d2-140">Список дочерних идентификаторов параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-140">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="dc9d2-141">settingName</span><span class="sxs-lookup"><span data-stu-id="dc9d2-141">settingName</span></span>|<span data-ttu-id="dc9d2-142">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-142">String</span></span>|<span data-ttu-id="dc9d2-143">Имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-143">The name of this group policy setting.</span></span>|
|<span data-ttu-id="dc9d2-144">settingValue</span><span class="sxs-lookup"><span data-stu-id="dc9d2-144">settingValue</span></span>|<span data-ttu-id="dc9d2-145">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-145">String</span></span>|<span data-ttu-id="dc9d2-146">Значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-146">The value of this group policy setting.</span></span>|
|<span data-ttu-id="dc9d2-147">сеттингвалуетипе</span><span class="sxs-lookup"><span data-stu-id="dc9d2-147">settingValueType</span></span>|<span data-ttu-id="dc9d2-148">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-148">String</span></span>|<span data-ttu-id="dc9d2-149">Тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-149">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="dc9d2-150">сеттингдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="dc9d2-150">settingDisplayName</span></span>|<span data-ttu-id="dc9d2-151">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-151">String</span></span>|<span data-ttu-id="dc9d2-152">Отображаемое имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-152">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="dc9d2-153">сеттингдисплайвалуе</span><span class="sxs-lookup"><span data-stu-id="dc9d2-153">settingDisplayValue</span></span>|<span data-ttu-id="dc9d2-154">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-154">String</span></span>|<span data-ttu-id="dc9d2-155">Отображаемое значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-155">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="dc9d2-156">сеттингдисплайвалуетипе</span><span class="sxs-lookup"><span data-stu-id="dc9d2-156">settingDisplayValueType</span></span>|<span data-ttu-id="dc9d2-157">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-157">String</span></span>|<span data-ttu-id="dc9d2-158">Отображаемый тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-158">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="dc9d2-159">сеттингвалуедисплайунитс</span><span class="sxs-lookup"><span data-stu-id="dc9d2-159">settingValueDisplayUnits</span></span>|<span data-ttu-id="dc9d2-160">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-160">String</span></span>|<span data-ttu-id="dc9d2-161">Отображаемые единицы значения параметра групповой политики</span><span class="sxs-lookup"><span data-stu-id="dc9d2-161">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="dc9d2-162">сеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="dc9d2-162">settingCategory</span></span>|<span data-ttu-id="dc9d2-163">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-163">String</span></span>|<span data-ttu-id="dc9d2-164">Категория, в которой находится параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-164">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="dc9d2-165">мдмкспнаме</span><span class="sxs-lookup"><span data-stu-id="dc9d2-165">mdmCspName</span></span>|<span data-ttu-id="dc9d2-166">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-166">String</span></span>|<span data-ttu-id="dc9d2-167">Имя CSP, которое сопоставляется параметру групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-167">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="dc9d2-168">мдмсеттингури</span><span class="sxs-lookup"><span data-stu-id="dc9d2-168">mdmSettingUri</span></span>|<span data-ttu-id="dc9d2-169">String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-169">String</span></span>|<span data-ttu-id="dc9d2-170">Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-170">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="dc9d2-171">мдмминимумосверсион</span><span class="sxs-lookup"><span data-stu-id="dc9d2-171">mdmMinimumOSVersion</span></span>|<span data-ttu-id="dc9d2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="dc9d2-172">Int32</span></span>|<span data-ttu-id="dc9d2-173">Минимальная версия ОС, поддерживаемая параметром MDM.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-173">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="dc9d2-174">сеттингтипе</span><span class="sxs-lookup"><span data-stu-id="dc9d2-174">settingType</span></span>|[<span data-ttu-id="dc9d2-175">граупполицисеттингтипе</span><span class="sxs-lookup"><span data-stu-id="dc9d2-175">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="dc9d2-176">Тип параметра (Security или ADMX) групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-176">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="dc9d2-177">Возможные значения: `unknown`, `policy`, `account`.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-177">Possible values are: `unknown`, `policy`, `account`.</span></span>|
|<span data-ttu-id="dc9d2-178">исмдмсуппортед</span><span class="sxs-lookup"><span data-stu-id="dc9d2-178">isMdmSupported</span></span>|<span data-ttu-id="dc9d2-179">Логический</span><span class="sxs-lookup"><span data-stu-id="dc9d2-179">Boolean</span></span>|<span data-ttu-id="dc9d2-180">Указывает, поддерживается ли Intune или нет</span><span class="sxs-lookup"><span data-stu-id="dc9d2-180">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="dc9d2-181">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="dc9d2-181">settingScope</span></span>|[<span data-ttu-id="dc9d2-182">граупполицисеттингскопе</span><span class="sxs-lookup"><span data-stu-id="dc9d2-182">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="dc9d2-183">Область применения параметра.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-183">The scope of the setting.</span></span> <span data-ttu-id="dc9d2-184">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-184">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="dc9d2-185">интунесеттингурилист</span><span class="sxs-lookup"><span data-stu-id="dc9d2-185">intuneSettingUriList</span></span>|<span data-ttu-id="dc9d2-186">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dc9d2-186">String collection</span></span>|<span data-ttu-id="dc9d2-187">Список URI параметров Intune, которые сопоставлены параметру групповой политики</span><span class="sxs-lookup"><span data-stu-id="dc9d2-187">The list of Intune Setting URIs this group policy setting maps to</span></span>|



## <a name="response"></a><span data-ttu-id="dc9d2-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc9d2-188">Response</span></span>
<span data-ttu-id="dc9d2-189">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-189">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc9d2-190">Пример</span><span class="sxs-lookup"><span data-stu-id="dc9d2-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc9d2-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc9d2-191">Request</span></span>
<span data-ttu-id="dc9d2-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 850

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
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="dc9d2-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc9d2-193">Response</span></span>
<span data-ttu-id="dc9d2-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc9d2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 899

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
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```






