---
title: Создание deviceConfigurationConflictSummary
description: Создание нового объекта deviceConfigurationConflictSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e120e6ce3070012eb1dffcfb06cf77040c0f44cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812420"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="4b684-103">Создание deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="4b684-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="4b684-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b684-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b684-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b684-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b684-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4b684-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b684-107">Создание нового объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4b684-107">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b684-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b684-108">Prerequisites</span></span>
<span data-ttu-id="4b684-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b684-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b684-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b684-111">Permission type</span></span>|<span data-ttu-id="4b684-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b684-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b684-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b684-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b684-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b684-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b684-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b684-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b684-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b684-116">Not supported.</span></span>|
|<span data-ttu-id="4b684-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b684-117">Application</span></span>|<span data-ttu-id="4b684-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b684-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b684-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b684-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="4b684-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b684-120">Request headers</span></span>
|<span data-ttu-id="4b684-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b684-121">Header</span></span>|<span data-ttu-id="4b684-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b684-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b684-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b684-123">Authorization</span></span>|<span data-ttu-id="4b684-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4b684-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b684-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b684-125">Accept</span></span>|<span data-ttu-id="4b684-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b684-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b684-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b684-127">Request body</span></span>
<span data-ttu-id="4b684-128">В тексте запроса укажите представление JSON для объекта deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="4b684-128">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="4b684-129">В следующей таблице показаны свойства, которые необходимы для создания deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="4b684-129">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="4b684-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b684-130">Property</span></span>|<span data-ttu-id="4b684-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b684-131">Type</span></span>|<span data-ttu-id="4b684-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b684-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b684-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="4b684-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="4b684-134">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="4b684-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="4b684-135">Набор политик конфликтует с данного параметра</span><span class="sxs-lookup"><span data-stu-id="4b684-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="4b684-136">id</span><span class="sxs-lookup"><span data-stu-id="4b684-136">id</span></span>|<span data-ttu-id="4b684-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4b684-137">String</span></span>|<span data-ttu-id="4b684-138">Идентификатор для этого набора конфликтующие политики.</span><span class="sxs-lookup"><span data-stu-id="4b684-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="4b684-139">Этот идентификатор — идентификаторы всех политик в ConflictingDeviceConfigurations в лексикографических порядке, разделенных точкой с подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="4b684-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="4b684-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="4b684-140">contributingSettings</span></span>|<span data-ttu-id="4b684-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b684-141">String collection</span></span>|<span data-ttu-id="4b684-142">Набор параметров конфликтует с указанной политики</span><span class="sxs-lookup"><span data-stu-id="4b684-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="4b684-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="4b684-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="4b684-144">Int32</span><span class="sxs-lookup"><span data-stu-id="4b684-144">Int32</span></span>|<span data-ttu-id="4b684-145">Count возвраты, на которые оказывает влияние конфликтующие политики и параметры</span><span class="sxs-lookup"><span data-stu-id="4b684-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="4b684-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b684-146">Response</span></span>
<span data-ttu-id="4b684-147">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4b684-147">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b684-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4b684-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b684-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b684-149">Request</span></span>
<span data-ttu-id="4b684-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b684-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b684-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b684-151">Response</span></span>
<span data-ttu-id="4b684-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4b684-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





