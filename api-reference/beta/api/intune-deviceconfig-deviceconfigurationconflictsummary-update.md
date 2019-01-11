---
title: Обновление deviceConfigurationConflictSummary
description: Обновление свойства объекта deviceConfigurationConflictSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4fb01b5fe7321d25e6b1d7e346a029e830375247
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812763"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="e650a-103">Обновление deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="e650a-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="e650a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e650a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e650a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e650a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e650a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e650a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e650a-107">Обновление свойства объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e650a-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e650a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e650a-108">Prerequisites</span></span>
<span data-ttu-id="e650a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e650a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e650a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e650a-111">Permission type</span></span>|<span data-ttu-id="e650a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e650a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e650a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e650a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e650a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e650a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e650a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e650a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e650a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e650a-116">Not supported.</span></span>|
|<span data-ttu-id="e650a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e650a-117">Application</span></span>|<span data-ttu-id="e650a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e650a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e650a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e650a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e650a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e650a-120">Request headers</span></span>
|<span data-ttu-id="e650a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e650a-121">Header</span></span>|<span data-ttu-id="e650a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e650a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e650a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e650a-123">Authorization</span></span>|<span data-ttu-id="e650a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e650a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e650a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e650a-125">Accept</span></span>|<span data-ttu-id="e650a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e650a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e650a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e650a-127">Request body</span></span>
<span data-ttu-id="e650a-128">В тексте запроса укажите представление JSON для объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e650a-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="e650a-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e650a-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="e650a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e650a-130">Property</span></span>|<span data-ttu-id="e650a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e650a-131">Type</span></span>|<span data-ttu-id="e650a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e650a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e650a-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="e650a-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="e650a-134">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="e650a-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="e650a-135">Набор политик конфликтует с данного параметра</span><span class="sxs-lookup"><span data-stu-id="e650a-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="e650a-136">id</span><span class="sxs-lookup"><span data-stu-id="e650a-136">id</span></span>|<span data-ttu-id="e650a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e650a-137">String</span></span>|<span data-ttu-id="e650a-138">Идентификатор для этого набора конфликтующие политики.</span><span class="sxs-lookup"><span data-stu-id="e650a-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="e650a-139">Этот идентификатор — идентификаторы всех политик в ConflictingDeviceConfigurations в лексикографических порядке, разделенных точкой с подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="e650a-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="e650a-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="e650a-140">contributingSettings</span></span>|<span data-ttu-id="e650a-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e650a-141">String collection</span></span>|<span data-ttu-id="e650a-142">Набор параметров конфликтует с указанной политики</span><span class="sxs-lookup"><span data-stu-id="e650a-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="e650a-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="e650a-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="e650a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e650a-144">Int32</span></span>|<span data-ttu-id="e650a-145">Count возвраты, на которые оказывает влияние конфликтующие политики и параметры</span><span class="sxs-lookup"><span data-stu-id="e650a-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="e650a-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="e650a-146">Response</span></span>
<span data-ttu-id="e650a-147">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e650a-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e650a-148">Пример</span><span class="sxs-lookup"><span data-stu-id="e650a-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="e650a-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e650a-149">Request</span></span>
<span data-ttu-id="e650a-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e650a-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e650a-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="e650a-151">Response</span></span>
<span data-ttu-id="e650a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e650a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





