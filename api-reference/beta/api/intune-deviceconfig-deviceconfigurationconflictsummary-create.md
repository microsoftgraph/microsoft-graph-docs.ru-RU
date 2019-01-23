---
title: Создание deviceConfigurationConflictSummary
description: Создание нового объекта deviceConfigurationConflictSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9488f61819a67f7ab648a6677a30e7422be0539c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412081"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="83f86-103">Создание deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="83f86-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="83f86-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="83f86-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83f86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83f86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83f86-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83f86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83f86-107">Создание нового объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="83f86-107">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83f86-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="83f86-108">Prerequisites</span></span>
<span data-ttu-id="83f86-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="83f86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="83f86-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83f86-111">Permission type</span></span>|<span data-ttu-id="83f86-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83f86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83f86-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83f86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83f86-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f86-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83f86-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83f86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83f86-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83f86-116">Not supported.</span></span>|
|<span data-ttu-id="83f86-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83f86-117">Application</span></span>|<span data-ttu-id="83f86-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83f86-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83f86-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83f86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="83f86-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83f86-120">Request headers</span></span>
|<span data-ttu-id="83f86-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83f86-121">Header</span></span>|<span data-ttu-id="83f86-122">Значение</span><span class="sxs-lookup"><span data-stu-id="83f86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83f86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83f86-123">Authorization</span></span>|<span data-ttu-id="83f86-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="83f86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83f86-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83f86-125">Accept</span></span>|<span data-ttu-id="83f86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83f86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83f86-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83f86-127">Request body</span></span>
<span data-ttu-id="83f86-128">В тексте запроса укажите представление JSON для объекта deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="83f86-128">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="83f86-129">В следующей таблице показаны свойства, которые необходимы для создания deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="83f86-129">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="83f86-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="83f86-130">Property</span></span>|<span data-ttu-id="83f86-131">Тип</span><span class="sxs-lookup"><span data-stu-id="83f86-131">Type</span></span>|<span data-ttu-id="83f86-132">Описание</span><span class="sxs-lookup"><span data-stu-id="83f86-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83f86-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="83f86-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="83f86-134">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="83f86-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="83f86-135">Набор политик конфликтует с данного параметра</span><span class="sxs-lookup"><span data-stu-id="83f86-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="83f86-136">id</span><span class="sxs-lookup"><span data-stu-id="83f86-136">id</span></span>|<span data-ttu-id="83f86-137">String</span><span class="sxs-lookup"><span data-stu-id="83f86-137">String</span></span>|<span data-ttu-id="83f86-138">Идентификатор для этого набора конфликтующие политики.</span><span class="sxs-lookup"><span data-stu-id="83f86-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="83f86-139">Этот идентификатор — идентификаторы всех политик в ConflictingDeviceConfigurations в лексикографических порядке, разделенных точкой с подчеркивания.</span><span class="sxs-lookup"><span data-stu-id="83f86-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="83f86-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="83f86-140">contributingSettings</span></span>|<span data-ttu-id="83f86-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="83f86-141">String collection</span></span>|<span data-ttu-id="83f86-142">Набор параметров конфликтует с указанной политики</span><span class="sxs-lookup"><span data-stu-id="83f86-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="83f86-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="83f86-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="83f86-144">Int32</span><span class="sxs-lookup"><span data-stu-id="83f86-144">Int32</span></span>|<span data-ttu-id="83f86-145">Count возвраты, на которые оказывает влияние конфликтующие политики и параметры</span><span class="sxs-lookup"><span data-stu-id="83f86-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="83f86-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="83f86-146">Response</span></span>
<span data-ttu-id="83f86-147">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="83f86-147">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83f86-148">Пример</span><span class="sxs-lookup"><span data-stu-id="83f86-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="83f86-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="83f86-149">Request</span></span>
<span data-ttu-id="83f86-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83f86-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83f86-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="83f86-151">Response</span></span>
<span data-ttu-id="83f86-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="83f86-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




