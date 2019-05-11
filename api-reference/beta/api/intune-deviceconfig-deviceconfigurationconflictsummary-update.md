---
title: Обновление Девицеконфигуратионконфликтсуммари
description: Обновление свойств объекта Девицеконфигуратионконфликтсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b09b9e3ab563b0d00fed9a8dfca2eec6118641b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927407"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="31f08-103">Обновление Девицеконфигуратионконфликтсуммари</span><span class="sxs-lookup"><span data-stu-id="31f08-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="31f08-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31f08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31f08-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31f08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31f08-106">Обновление свойств объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="31f08-106">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31f08-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31f08-107">Prerequisites</span></span>
<span data-ttu-id="31f08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31f08-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31f08-110">Permission type</span></span>|<span data-ttu-id="31f08-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31f08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31f08-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31f08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31f08-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31f08-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31f08-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31f08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31f08-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31f08-115">Not supported.</span></span>|
|<span data-ttu-id="31f08-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31f08-116">Application</span></span>|<span data-ttu-id="31f08-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31f08-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31f08-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31f08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="31f08-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31f08-119">Request headers</span></span>
|<span data-ttu-id="31f08-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31f08-120">Header</span></span>|<span data-ttu-id="31f08-121">Значение</span><span class="sxs-lookup"><span data-stu-id="31f08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31f08-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31f08-122">Authorization</span></span>|<span data-ttu-id="31f08-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31f08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31f08-124">Accept</span><span class="sxs-lookup"><span data-stu-id="31f08-124">Accept</span></span>|<span data-ttu-id="31f08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31f08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31f08-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="31f08-126">Request body</span></span>
<span data-ttu-id="31f08-127">В тексте запроса добавьте представление объекта [Девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31f08-127">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="31f08-128">В следующей таблице приведены свойства, необходимые при создании [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="31f08-128">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="31f08-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="31f08-129">Property</span></span>|<span data-ttu-id="31f08-130">Тип</span><span class="sxs-lookup"><span data-stu-id="31f08-130">Type</span></span>|<span data-ttu-id="31f08-131">Описание</span><span class="sxs-lookup"><span data-stu-id="31f08-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31f08-132">Конфликтингдевицеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="31f08-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="31f08-133">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="31f08-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="31f08-134">Набор политик в конфликте с заданным параметром</span><span class="sxs-lookup"><span data-stu-id="31f08-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="31f08-135">id</span><span class="sxs-lookup"><span data-stu-id="31f08-135">id</span></span>|<span data-ttu-id="31f08-136">Строка</span><span class="sxs-lookup"><span data-stu-id="31f08-136">String</span></span>|<span data-ttu-id="31f08-137">Идентификатор этого набора конфликтующих политик.</span><span class="sxs-lookup"><span data-stu-id="31f08-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="31f08-138">Этот идентификатор — идентификаторы всех политик в Конфликтингдевицеконфигуратионс в лексикографикал порядке, разделенных символами подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="31f08-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="31f08-139">Контрибутингсеттингс</span><span class="sxs-lookup"><span data-stu-id="31f08-139">contributingSettings</span></span>|<span data-ttu-id="31f08-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="31f08-140">String collection</span></span>|<span data-ttu-id="31f08-141">Набор параметров в конфликте с заданными политиками</span><span class="sxs-lookup"><span data-stu-id="31f08-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="31f08-142">Девицечеккинсимпактед</span><span class="sxs-lookup"><span data-stu-id="31f08-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="31f08-143">Int32</span><span class="sxs-lookup"><span data-stu-id="31f08-143">Int32</span></span>|<span data-ttu-id="31f08-144">Число возвратов, затронутых конфликтующими политиками и параметрами</span><span class="sxs-lookup"><span data-stu-id="31f08-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="31f08-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="31f08-145">Response</span></span>
<span data-ttu-id="31f08-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31f08-146">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31f08-147">Пример</span><span class="sxs-lookup"><span data-stu-id="31f08-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="31f08-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="31f08-148">Request</span></span>
<span data-ttu-id="31f08-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31f08-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="31f08-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="31f08-150">Response</span></span>
<span data-ttu-id="31f08-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31f08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




