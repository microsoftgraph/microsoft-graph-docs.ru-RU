---
title: Обновление deviceConfigurationConflictSummary
description: Обновление свойства объекта deviceConfigurationConflictSummary.
ms.openlocfilehash: 583d00b1ee7bbb3547592cc58f45899aa89c4219
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075565"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="750fb-103">Обновление deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="750fb-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="750fb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="750fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="750fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="750fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="750fb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="750fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="750fb-107">Обновление свойства объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="750fb-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="750fb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="750fb-108">Prerequisites</span></span>
<span data-ttu-id="750fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="750fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="750fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="750fb-111">Permission type</span></span>|<span data-ttu-id="750fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="750fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="750fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="750fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="750fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="750fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="750fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="750fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="750fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="750fb-116">Not supported.</span></span>|
|<span data-ttu-id="750fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="750fb-117">Application</span></span>|<span data-ttu-id="750fb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="750fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="750fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="750fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="750fb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="750fb-120">Request headers</span></span>
|<span data-ttu-id="750fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="750fb-121">Header</span></span>|<span data-ttu-id="750fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="750fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="750fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="750fb-123">Authorization</span></span>|<span data-ttu-id="750fb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="750fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="750fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="750fb-125">Accept</span></span>|<span data-ttu-id="750fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="750fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="750fb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="750fb-127">Request body</span></span>
<span data-ttu-id="750fb-128">В тексте запроса укажите представление JSON для объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="750fb-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="750fb-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="750fb-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="750fb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="750fb-130">Property</span></span>|<span data-ttu-id="750fb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="750fb-131">Type</span></span>|<span data-ttu-id="750fb-132">Description</span><span class="sxs-lookup"><span data-stu-id="750fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="750fb-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="750fb-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="750fb-134">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="750fb-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="750fb-135">Набор политик конфликтует с данного параметра</span><span class="sxs-lookup"><span data-stu-id="750fb-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="750fb-136">id</span><span class="sxs-lookup"><span data-stu-id="750fb-136">id</span></span>|<span data-ttu-id="750fb-137">String</span><span class="sxs-lookup"><span data-stu-id="750fb-137">String</span></span>|<span data-ttu-id="750fb-138">Идентификатор для этого набора конфликтующие политики.</span><span class="sxs-lookup"><span data-stu-id="750fb-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="750fb-139">Этот идентификатор — идентификаторы всех политик в ConflictingDeviceConfigurations в лексикографических порядке, разделенных точкой с подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="750fb-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="750fb-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="750fb-140">contributingSettings</span></span>|<span data-ttu-id="750fb-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="750fb-141">String collection</span></span>|<span data-ttu-id="750fb-142">Набор параметров конфликтует с указанной политики</span><span class="sxs-lookup"><span data-stu-id="750fb-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="750fb-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="750fb-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="750fb-144">Int32</span><span class="sxs-lookup"><span data-stu-id="750fb-144">Int32</span></span>|<span data-ttu-id="750fb-145">Count возвраты, на которые оказывает влияние конфликтующие политики и параметры</span><span class="sxs-lookup"><span data-stu-id="750fb-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="750fb-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="750fb-146">Response</span></span>
<span data-ttu-id="750fb-147">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="750fb-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="750fb-148">Пример</span><span class="sxs-lookup"><span data-stu-id="750fb-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="750fb-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="750fb-149">Request</span></span>
<span data-ttu-id="750fb-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="750fb-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
Content-type: application/json
Content-length: 288

{
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

### <a name="response"></a><span data-ttu-id="750fb-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="750fb-151">Response</span></span>
<span data-ttu-id="750fb-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="750fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





