---
title: Обновление Девицеконфигуратионконфликтсуммари
description: Обновление свойств объекта Девицеконфигуратионконфликтсуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f701d6323f648b1e1c6304d97a4dbd9e53cc487e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49291731"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="a2379-103">Обновление Девицеконфигуратионконфликтсуммари</span><span class="sxs-lookup"><span data-stu-id="a2379-103">Update deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="a2379-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2379-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2379-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2379-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2379-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2379-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2379-107">Обновление свойств объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a2379-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2379-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2379-108">Prerequisites</span></span>
<span data-ttu-id="a2379-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2379-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2379-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2379-111">Permission type</span></span>|<span data-ttu-id="a2379-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2379-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2379-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2379-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2379-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2379-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2379-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2379-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2379-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2379-116">Not supported.</span></span>|
|<span data-ttu-id="a2379-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2379-117">Application</span></span>|<span data-ttu-id="a2379-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2379-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2379-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2379-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a2379-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2379-120">Request headers</span></span>
|<span data-ttu-id="a2379-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2379-121">Header</span></span>|<span data-ttu-id="a2379-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2379-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2379-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2379-123">Authorization</span></span>|<span data-ttu-id="a2379-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2379-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2379-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2379-125">Accept</span></span>|<span data-ttu-id="a2379-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2379-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2379-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2379-127">Request body</span></span>
<span data-ttu-id="a2379-128">В тексте запроса добавьте представление объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2379-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="a2379-129">В следующей таблице приведены свойства, необходимые при создании [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a2379-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="a2379-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2379-130">Property</span></span>|<span data-ttu-id="a2379-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2379-131">Type</span></span>|<span data-ttu-id="a2379-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2379-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2379-133">конфликтингдевицеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="a2379-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="a2379-134">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="a2379-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="a2379-135">Набор политик в конфликте с заданным параметром</span><span class="sxs-lookup"><span data-stu-id="a2379-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="a2379-136">id</span><span class="sxs-lookup"><span data-stu-id="a2379-136">id</span></span>|<span data-ttu-id="a2379-137">String</span><span class="sxs-lookup"><span data-stu-id="a2379-137">String</span></span>|<span data-ttu-id="a2379-138">Идентификатор этого набора конфликтующих политик.</span><span class="sxs-lookup"><span data-stu-id="a2379-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="a2379-139">Этот идентификатор — идентификаторы всех политик в Конфликтингдевицеконфигуратионс в лексикографикал порядке, разделенных символами подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="a2379-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="a2379-140">контрибутингсеттингс</span><span class="sxs-lookup"><span data-stu-id="a2379-140">contributingSettings</span></span>|<span data-ttu-id="a2379-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a2379-141">String collection</span></span>|<span data-ttu-id="a2379-142">Набор параметров в конфликте с заданными политиками</span><span class="sxs-lookup"><span data-stu-id="a2379-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="a2379-143">девицечеккинсимпактед</span><span class="sxs-lookup"><span data-stu-id="a2379-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="a2379-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a2379-144">Int32</span></span>|<span data-ttu-id="a2379-145">Число возвратов, затронутых конфликтующими политиками и параметрами</span><span class="sxs-lookup"><span data-stu-id="a2379-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="a2379-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2379-146">Response</span></span>
<span data-ttu-id="a2379-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2379-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2379-148">Пример</span><span class="sxs-lookup"><span data-stu-id="a2379-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2379-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2379-149">Request</span></span>
<span data-ttu-id="a2379-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2379-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
Content-type: application/json
Content-length: 398

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value",
      "sourceType": "deviceIntent"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="a2379-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2379-151">Response</span></span>
<span data-ttu-id="a2379-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2379-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value",
      "sourceType": "deviceIntent"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




