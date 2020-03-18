---
title: Обновление Девицеконфигуратионконфликтсуммари
description: Обновление свойств объекта Девицеконфигуратионконфликтсуммари.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2719bb572896c743edb794f86bc5b921bbc4e717
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42754267"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="64eeb-103">Обновление Девицеконфигуратионконфликтсуммари</span><span class="sxs-lookup"><span data-stu-id="64eeb-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="64eeb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64eeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64eeb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64eeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64eeb-106">Обновление свойств объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="64eeb-106">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64eeb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="64eeb-107">Prerequisites</span></span>
<span data-ttu-id="64eeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64eeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64eeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64eeb-110">Permission type</span></span>|<span data-ttu-id="64eeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64eeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64eeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64eeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64eeb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64eeb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64eeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64eeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64eeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64eeb-115">Not supported.</span></span>|
|<span data-ttu-id="64eeb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="64eeb-116">Application</span></span>|<span data-ttu-id="64eeb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64eeb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64eeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64eeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="64eeb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="64eeb-119">Request headers</span></span>
|<span data-ttu-id="64eeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64eeb-120">Header</span></span>|<span data-ttu-id="64eeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64eeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64eeb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64eeb-122">Authorization</span></span>|<span data-ttu-id="64eeb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64eeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64eeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="64eeb-124">Accept</span></span>|<span data-ttu-id="64eeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64eeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64eeb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64eeb-126">Request body</span></span>
<span data-ttu-id="64eeb-127">В тексте запроса добавьте представление объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64eeb-127">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="64eeb-128">В следующей таблице приведены свойства, необходимые при создании [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="64eeb-128">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="64eeb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="64eeb-129">Property</span></span>|<span data-ttu-id="64eeb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="64eeb-130">Type</span></span>|<span data-ttu-id="64eeb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="64eeb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64eeb-132">конфликтингдевицеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="64eeb-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="64eeb-133">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="64eeb-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="64eeb-134">Набор политик в конфликте с заданным параметром</span><span class="sxs-lookup"><span data-stu-id="64eeb-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="64eeb-135">id</span><span class="sxs-lookup"><span data-stu-id="64eeb-135">id</span></span>|<span data-ttu-id="64eeb-136">String</span><span class="sxs-lookup"><span data-stu-id="64eeb-136">String</span></span>|<span data-ttu-id="64eeb-137">Идентификатор этого набора конфликтующих политик.</span><span class="sxs-lookup"><span data-stu-id="64eeb-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="64eeb-138">Этот идентификатор — идентификаторы всех политик в Конфликтингдевицеконфигуратионс в лексикографикал порядке, разделенных символами подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="64eeb-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="64eeb-139">контрибутингсеттингс</span><span class="sxs-lookup"><span data-stu-id="64eeb-139">contributingSettings</span></span>|<span data-ttu-id="64eeb-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64eeb-140">String collection</span></span>|<span data-ttu-id="64eeb-141">Набор параметров в конфликте с заданными политиками</span><span class="sxs-lookup"><span data-stu-id="64eeb-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="64eeb-142">девицечеккинсимпактед</span><span class="sxs-lookup"><span data-stu-id="64eeb-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="64eeb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="64eeb-143">Int32</span></span>|<span data-ttu-id="64eeb-144">Число возвратов, затронутых конфликтующими политиками и параметрами</span><span class="sxs-lookup"><span data-stu-id="64eeb-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="64eeb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="64eeb-145">Response</span></span>
<span data-ttu-id="64eeb-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64eeb-146">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64eeb-147">Пример</span><span class="sxs-lookup"><span data-stu-id="64eeb-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="64eeb-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="64eeb-148">Request</span></span>
<span data-ttu-id="64eeb-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64eeb-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="64eeb-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="64eeb-150">Response</span></span>
<span data-ttu-id="64eeb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64eeb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




