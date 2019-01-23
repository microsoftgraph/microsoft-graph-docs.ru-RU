---
title: Обновление deviceConfigurationConflictSummary
description: Обновление свойства объекта deviceConfigurationConflictSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ad5c5c7ad9db02afed53b4deb0cb6af3d2c57e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416358"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="d22b4-103">Обновление deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="d22b4-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="d22b4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d22b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d22b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d22b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d22b4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d22b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d22b4-107">Обновление свойства объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d22b4-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d22b4-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="d22b4-108">Prerequisites</span></span>
<span data-ttu-id="d22b4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d22b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d22b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d22b4-111">Permission type</span></span>|<span data-ttu-id="d22b4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d22b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d22b4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d22b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d22b4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d22b4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d22b4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d22b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d22b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d22b4-116">Not supported.</span></span>|
|<span data-ttu-id="d22b4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d22b4-117">Application</span></span>|<span data-ttu-id="d22b4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d22b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d22b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d22b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d22b4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d22b4-120">Request headers</span></span>
|<span data-ttu-id="d22b4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d22b4-121">Header</span></span>|<span data-ttu-id="d22b4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d22b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d22b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d22b4-123">Authorization</span></span>|<span data-ttu-id="d22b4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d22b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d22b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d22b4-125">Accept</span></span>|<span data-ttu-id="d22b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d22b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d22b4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d22b4-127">Request body</span></span>
<span data-ttu-id="d22b4-128">В тексте запроса укажите представление JSON для объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d22b4-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="d22b4-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d22b4-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="d22b4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d22b4-130">Property</span></span>|<span data-ttu-id="d22b4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d22b4-131">Type</span></span>|<span data-ttu-id="d22b4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d22b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d22b4-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="d22b4-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="d22b4-134">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="d22b4-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="d22b4-135">Набор политик конфликтует с данного параметра</span><span class="sxs-lookup"><span data-stu-id="d22b4-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="d22b4-136">id</span><span class="sxs-lookup"><span data-stu-id="d22b4-136">id</span></span>|<span data-ttu-id="d22b4-137">String</span><span class="sxs-lookup"><span data-stu-id="d22b4-137">String</span></span>|<span data-ttu-id="d22b4-138">Идентификатор для этого набора конфликтующие политики.</span><span class="sxs-lookup"><span data-stu-id="d22b4-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="d22b4-139">Этот идентификатор — идентификаторы всех политик в ConflictingDeviceConfigurations в лексикографических порядке, разделенных точкой с подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="d22b4-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="d22b4-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="d22b4-140">contributingSettings</span></span>|<span data-ttu-id="d22b4-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d22b4-141">String collection</span></span>|<span data-ttu-id="d22b4-142">Набор параметров конфликтует с указанной политики</span><span class="sxs-lookup"><span data-stu-id="d22b4-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="d22b4-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="d22b4-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="d22b4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d22b4-144">Int32</span></span>|<span data-ttu-id="d22b4-145">Count возвраты, на которые оказывает влияние конфликтующие политики и параметры</span><span class="sxs-lookup"><span data-stu-id="d22b4-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="d22b4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d22b4-146">Response</span></span>
<span data-ttu-id="d22b4-147">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d22b4-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d22b4-148">Пример</span><span class="sxs-lookup"><span data-stu-id="d22b4-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d22b4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="d22b4-149">Request</span></span>
<span data-ttu-id="d22b4-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d22b4-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d22b4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d22b4-151">Response</span></span>
<span data-ttu-id="d22b4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d22b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




