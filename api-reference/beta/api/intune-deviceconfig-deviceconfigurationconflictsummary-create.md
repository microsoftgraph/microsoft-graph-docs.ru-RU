---
title: Создание Девицеконфигуратионконфликтсуммари
description: Создание нового объекта Девицеконфигуратионконфликтсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab41f1249438ef9ebf8942ef7b84caa09da45f0f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949457"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="f2547-103">Создание Девицеконфигуратионконфликтсуммари</span><span class="sxs-lookup"><span data-stu-id="f2547-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="f2547-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2547-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2547-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2547-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2547-106">Создание нового объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f2547-106">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2547-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f2547-107">Prerequisites</span></span>
<span data-ttu-id="f2547-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2547-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2547-110">Permission type</span></span>|<span data-ttu-id="f2547-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2547-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2547-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2547-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2547-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2547-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2547-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2547-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2547-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2547-115">Not supported.</span></span>|
|<span data-ttu-id="f2547-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2547-116">Application</span></span>|<span data-ttu-id="f2547-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2547-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2547-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2547-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="f2547-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f2547-119">Request headers</span></span>
|<span data-ttu-id="f2547-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2547-120">Header</span></span>|<span data-ttu-id="f2547-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f2547-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2547-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2547-122">Authorization</span></span>|<span data-ttu-id="f2547-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2547-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2547-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f2547-124">Accept</span></span>|<span data-ttu-id="f2547-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2547-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2547-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2547-126">Request body</span></span>
<span data-ttu-id="f2547-127">В тексте запроса добавьте представление объекта Девицеконфигуратионконфликтсуммари в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2547-127">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="f2547-128">В следующей таблице приведены свойства, необходимые при создании Девицеконфигуратионконфликтсуммари.</span><span class="sxs-lookup"><span data-stu-id="f2547-128">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="f2547-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2547-129">Property</span></span>|<span data-ttu-id="f2547-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f2547-130">Type</span></span>|<span data-ttu-id="f2547-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f2547-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2547-132">конфликтингдевицеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="f2547-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="f2547-133">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="f2547-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="f2547-134">Набор политик в конфликте с заданным параметром</span><span class="sxs-lookup"><span data-stu-id="f2547-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="f2547-135">id</span><span class="sxs-lookup"><span data-stu-id="f2547-135">id</span></span>|<span data-ttu-id="f2547-136">Строка</span><span class="sxs-lookup"><span data-stu-id="f2547-136">String</span></span>|<span data-ttu-id="f2547-137">Идентификатор этого набора конфликтующих политик.</span><span class="sxs-lookup"><span data-stu-id="f2547-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="f2547-138">Этот идентификатор — идентификаторы всех политик в Конфликтингдевицеконфигуратионс в лексикографикал порядке, разделенных символами подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="f2547-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="f2547-139">контрибутингсеттингс</span><span class="sxs-lookup"><span data-stu-id="f2547-139">contributingSettings</span></span>|<span data-ttu-id="f2547-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f2547-140">String collection</span></span>|<span data-ttu-id="f2547-141">Набор параметров в конфликте с заданными политиками</span><span class="sxs-lookup"><span data-stu-id="f2547-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="f2547-142">девицечеккинсимпактед</span><span class="sxs-lookup"><span data-stu-id="f2547-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="f2547-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f2547-143">Int32</span></span>|<span data-ttu-id="f2547-144">Число возвратов, затронутых конфликтующими политиками и параметрами</span><span class="sxs-lookup"><span data-stu-id="f2547-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="f2547-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2547-145">Response</span></span>
<span data-ttu-id="f2547-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2547-146">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2547-147">Пример</span><span class="sxs-lookup"><span data-stu-id="f2547-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2547-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2547-148">Request</span></span>
<span data-ttu-id="f2547-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2547-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
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

### <a name="response"></a><span data-ttu-id="f2547-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2547-150">Response</span></span>
<span data-ttu-id="f2547-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2547-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





