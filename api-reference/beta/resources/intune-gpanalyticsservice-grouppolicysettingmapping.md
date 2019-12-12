---
title: Тип ресурса Граупполицисеттингмаппинг
description: Параметр групповой политики для сопоставления MDM/Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1b36a644ab9aa09e8de65f1d8a0d5ee95b6385bf
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955675"
---
# <a name="grouppolicysettingmapping-resource-type"></a><span data-ttu-id="c0a84-103">Тип ресурса Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="c0a84-103">groupPolicySettingMapping resource type</span></span>

> <span data-ttu-id="c0a84-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0a84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0a84-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0a84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0a84-106">Параметр групповой политики для сопоставления MDM/Intune.</span><span class="sxs-lookup"><span data-stu-id="c0a84-106">The Group Policy setting to MDM/Intune mapping.</span></span>

## <a name="methods"></a><span data-ttu-id="c0a84-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c0a84-107">Methods</span></span>
|<span data-ttu-id="c0a84-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c0a84-108">Method</span></span>|<span data-ttu-id="c0a84-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c0a84-109">Return Type</span></span>|<span data-ttu-id="c0a84-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c0a84-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0a84-111">Список Граупполицисеттингмаппингс</span><span class="sxs-lookup"><span data-stu-id="c0a84-111">List groupPolicySettingMappings</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|<span data-ttu-id="c0a84-112">Коллекция [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)</span><span class="sxs-lookup"><span data-stu-id="c0a84-112">[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) collection</span></span>|<span data-ttu-id="c0a84-113">Список свойств и связей объектов [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="c0a84-113">List properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects.</span></span>|
|[<span data-ttu-id="c0a84-114">Получение Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="c0a84-114">Get groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[<span data-ttu-id="c0a84-115">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="c0a84-115">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="c0a84-116">Чтение свойств и связей объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="c0a84-116">Read properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="c0a84-117">Создание Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="c0a84-117">Create groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[<span data-ttu-id="c0a84-118">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="c0a84-118">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="c0a84-119">Создание нового объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="c0a84-119">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="c0a84-120">Удаление Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="c0a84-120">Delete groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|<span data-ttu-id="c0a84-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c0a84-121">None</span></span>|<span data-ttu-id="c0a84-122">Удаляет объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span><span class="sxs-lookup"><span data-stu-id="c0a84-122">Deletes a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>|
|[<span data-ttu-id="c0a84-123">Обновление Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="c0a84-123">Update groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[<span data-ttu-id="c0a84-124">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="c0a84-124">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="c0a84-125">Обновление свойств объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="c0a84-125">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0a84-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0a84-126">Properties</span></span>
|<span data-ttu-id="c0a84-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0a84-127">Property</span></span>|<span data-ttu-id="c0a84-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c0a84-128">Type</span></span>|<span data-ttu-id="c0a84-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c0a84-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0a84-130">id</span><span class="sxs-lookup"><span data-stu-id="c0a84-130">id</span></span>|<span data-ttu-id="c0a84-131">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-131">String</span></span>|<span data-ttu-id="c0a84-132">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c0a84-132">Not yet documented</span></span>|
|<span data-ttu-id="c0a84-133">parentId</span><span class="sxs-lookup"><span data-stu-id="c0a84-133">parentId</span></span>|<span data-ttu-id="c0a84-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-134">String</span></span>|<span data-ttu-id="c0a84-135">Родительский идентификатор параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-135">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="c0a84-136">чилдидлист</span><span class="sxs-lookup"><span data-stu-id="c0a84-136">childIdList</span></span>|<span data-ttu-id="c0a84-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c0a84-137">String collection</span></span>|<span data-ttu-id="c0a84-138">Список дочерних идентификаторов параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-138">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="c0a84-139">settingName</span><span class="sxs-lookup"><span data-stu-id="c0a84-139">settingName</span></span>|<span data-ttu-id="c0a84-140">String</span><span class="sxs-lookup"><span data-stu-id="c0a84-140">String</span></span>|<span data-ttu-id="c0a84-141">Имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-141">The name of this group policy setting.</span></span>|
|<span data-ttu-id="c0a84-142">settingValue</span><span class="sxs-lookup"><span data-stu-id="c0a84-142">settingValue</span></span>|<span data-ttu-id="c0a84-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-143">String</span></span>|<span data-ttu-id="c0a84-144">Значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-144">The value of this group policy setting.</span></span>|
|<span data-ttu-id="c0a84-145">сеттингвалуетипе</span><span class="sxs-lookup"><span data-stu-id="c0a84-145">settingValueType</span></span>|<span data-ttu-id="c0a84-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-146">String</span></span>|<span data-ttu-id="c0a84-147">Тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-147">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="c0a84-148">сеттингдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="c0a84-148">settingDisplayName</span></span>|<span data-ttu-id="c0a84-149">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-149">String</span></span>|<span data-ttu-id="c0a84-150">Отображаемое имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-150">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="c0a84-151">сеттингдисплайвалуе</span><span class="sxs-lookup"><span data-stu-id="c0a84-151">settingDisplayValue</span></span>|<span data-ttu-id="c0a84-152">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-152">String</span></span>|<span data-ttu-id="c0a84-153">Отображаемое значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-153">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="c0a84-154">сеттингдисплайвалуетипе</span><span class="sxs-lookup"><span data-stu-id="c0a84-154">settingDisplayValueType</span></span>|<span data-ttu-id="c0a84-155">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-155">String</span></span>|<span data-ttu-id="c0a84-156">Отображаемый тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-156">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="c0a84-157">сеттингвалуедисплайунитс</span><span class="sxs-lookup"><span data-stu-id="c0a84-157">settingValueDisplayUnits</span></span>|<span data-ttu-id="c0a84-158">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-158">String</span></span>|<span data-ttu-id="c0a84-159">Отображаемые единицы значения параметра групповой политики</span><span class="sxs-lookup"><span data-stu-id="c0a84-159">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="c0a84-160">сеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="c0a84-160">settingCategory</span></span>|<span data-ttu-id="c0a84-161">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-161">String</span></span>|<span data-ttu-id="c0a84-162">Категория, в которой находится параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-162">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="c0a84-163">мдмкспнаме</span><span class="sxs-lookup"><span data-stu-id="c0a84-163">mdmCspName</span></span>|<span data-ttu-id="c0a84-164">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-164">String</span></span>|<span data-ttu-id="c0a84-165">Имя CSP, которое сопоставляется параметру групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-165">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="c0a84-166">мдмсеттингури</span><span class="sxs-lookup"><span data-stu-id="c0a84-166">mdmSettingUri</span></span>|<span data-ttu-id="c0a84-167">Строка</span><span class="sxs-lookup"><span data-stu-id="c0a84-167">String</span></span>|<span data-ttu-id="c0a84-168">Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-168">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="c0a84-169">мдмминимумосверсион</span><span class="sxs-lookup"><span data-stu-id="c0a84-169">mdmMinimumOSVersion</span></span>|<span data-ttu-id="c0a84-170">Int32</span><span class="sxs-lookup"><span data-stu-id="c0a84-170">Int32</span></span>|<span data-ttu-id="c0a84-171">Минимальная версия ОС, поддерживаемая параметром MDM.</span><span class="sxs-lookup"><span data-stu-id="c0a84-171">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="c0a84-172">сеттингтипе</span><span class="sxs-lookup"><span data-stu-id="c0a84-172">settingType</span></span>|[<span data-ttu-id="c0a84-173">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="c0a84-173">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="c0a84-174">Тип параметра (Security или ADMX) групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c0a84-174">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="c0a84-175">Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="c0a84-175">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="c0a84-176">исмдмсуппортед</span><span class="sxs-lookup"><span data-stu-id="c0a84-176">isMdmSupported</span></span>|<span data-ttu-id="c0a84-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a84-177">Boolean</span></span>|<span data-ttu-id="c0a84-178">Указывает, поддерживается ли Intune или нет</span><span class="sxs-lookup"><span data-stu-id="c0a84-178">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="c0a84-179">мдмсуппортедстате</span><span class="sxs-lookup"><span data-stu-id="c0a84-179">mdmSupportedState</span></span>|[<span data-ttu-id="c0a84-180">мдмсуппортедстате</span><span class="sxs-lookup"><span data-stu-id="c0a84-180">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="c0a84-181">Указывает, поддерживается ли параметр в MDM.</span><span class="sxs-lookup"><span data-stu-id="c0a84-181">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="c0a84-182">Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="c0a84-182">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="c0a84-183">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="c0a84-183">settingScope</span></span>|[<span data-ttu-id="c0a84-184">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="c0a84-184">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="c0a84-185">Область применения параметра.</span><span class="sxs-lookup"><span data-stu-id="c0a84-185">The scope of the setting.</span></span> <span data-ttu-id="c0a84-186">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="c0a84-186">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="c0a84-187">интунесеттингурилист</span><span class="sxs-lookup"><span data-stu-id="c0a84-187">intuneSettingUriList</span></span>|<span data-ttu-id="c0a84-188">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c0a84-188">String collection</span></span>|<span data-ttu-id="c0a84-189">Список URI параметров Intune, которые сопоставлены параметру групповой политики</span><span class="sxs-lookup"><span data-stu-id="c0a84-189">The list of Intune Setting URIs this group policy setting maps to</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0a84-190">Связи</span><span class="sxs-lookup"><span data-stu-id="c0a84-190">Relationships</span></span>
<span data-ttu-id="c0a84-191">Нет</span><span class="sxs-lookup"><span data-stu-id="c0a84-191">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0a84-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0a84-192">JSON Representation</span></span>
<span data-ttu-id="c0a84-193">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0a84-193">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicySettingMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "String (identifier)",
  "parentId": "String",
  "childIdList": [
    "String"
  ],
  "settingName": "String",
  "settingValue": "String",
  "settingValueType": "String",
  "settingDisplayName": "String",
  "settingDisplayValue": "String",
  "settingDisplayValueType": "String",
  "settingValueDisplayUnits": "String",
  "settingCategory": "String",
  "mdmCspName": "String",
  "mdmSettingUri": "String",
  "mdmMinimumOSVersion": 1024,
  "settingType": "String",
  "isMdmSupported": true,
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ]
}
```



