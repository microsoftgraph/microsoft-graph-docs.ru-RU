---
title: Создание deviceConfigurationConflictSummary
description: Создание нового объекта deviceConfigurationConflictSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ea5aa43cf4df325afbffddcc1323f98bf89a3166
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968402"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="f233c-103">Создание deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="f233c-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="f233c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f233c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f233c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f233c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f233c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f233c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f233c-107">Создание нового объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f233c-107">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f233c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f233c-108">Prerequisites</span></span>
<span data-ttu-id="f233c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f233c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f233c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f233c-111">Permission type</span></span>|<span data-ttu-id="f233c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f233c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f233c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f233c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f233c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f233c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f233c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f233c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f233c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f233c-116">Not supported.</span></span>|
|<span data-ttu-id="f233c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f233c-117">Application</span></span>|<span data-ttu-id="f233c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f233c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f233c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f233c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="f233c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f233c-120">Request headers</span></span>
|<span data-ttu-id="f233c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f233c-121">Header</span></span>|<span data-ttu-id="f233c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f233c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f233c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f233c-123">Authorization</span></span>|<span data-ttu-id="f233c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f233c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f233c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f233c-125">Accept</span></span>|<span data-ttu-id="f233c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f233c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f233c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f233c-127">Request body</span></span>
<span data-ttu-id="f233c-128">В тексте запроса укажите представление JSON для объекта deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="f233c-128">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="f233c-129">В следующей таблице показаны свойства, которые необходимы для создания deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="f233c-129">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="f233c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f233c-130">Property</span></span>|<span data-ttu-id="f233c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f233c-131">Type</span></span>|<span data-ttu-id="f233c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f233c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f233c-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="f233c-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="f233c-134">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="f233c-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="f233c-135">Набор политик конфликтует с данного параметра</span><span class="sxs-lookup"><span data-stu-id="f233c-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="f233c-136">id</span><span class="sxs-lookup"><span data-stu-id="f233c-136">id</span></span>|<span data-ttu-id="f233c-137">String</span><span class="sxs-lookup"><span data-stu-id="f233c-137">String</span></span>|<span data-ttu-id="f233c-138">Идентификатор для этого набора конфликтующие политики.</span><span class="sxs-lookup"><span data-stu-id="f233c-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="f233c-139">Этот идентификатор — идентификаторы всех политик в ConflictingDeviceConfigurations в лексикографических порядке, разделенных точкой с подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="f233c-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="f233c-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="f233c-140">contributingSettings</span></span>|<span data-ttu-id="f233c-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f233c-141">String collection</span></span>|<span data-ttu-id="f233c-142">Набор параметров конфликтует с указанной политики</span><span class="sxs-lookup"><span data-stu-id="f233c-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="f233c-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="f233c-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="f233c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f233c-144">Int32</span></span>|<span data-ttu-id="f233c-145">Count возвраты, на которые оказывает влияние конфликтующие политики и параметры</span><span class="sxs-lookup"><span data-stu-id="f233c-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="f233c-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="f233c-146">Response</span></span>
<span data-ttu-id="f233c-147">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f233c-147">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f233c-148">Пример</span><span class="sxs-lookup"><span data-stu-id="f233c-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="f233c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f233c-149">Request</span></span>
<span data-ttu-id="f233c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f233c-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f233c-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="f233c-151">Response</span></span>
<span data-ttu-id="f233c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f233c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





