---
title: Обновление объекта onPremisesConditionalAccessSettings
description: Обновляет свойства объекта onPremisesConditionalAccessSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e545680a0f1268fc1012f03c20e6b65582dafb1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941605"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="6914a-103">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="6914a-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="6914a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6914a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6914a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6914a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6914a-106">Обновляет свойства объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="6914a-106">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6914a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6914a-107">Prerequisites</span></span>
<span data-ttu-id="6914a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6914a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6914a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6914a-110">Permission type</span></span>|<span data-ttu-id="6914a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6914a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6914a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6914a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6914a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6914a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6914a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6914a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6914a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6914a-115">Not supported.</span></span>|
|<span data-ttu-id="6914a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6914a-116">Application</span></span>|<span data-ttu-id="6914a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6914a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6914a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6914a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="6914a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6914a-119">Request headers</span></span>
|<span data-ttu-id="6914a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6914a-120">Header</span></span>|<span data-ttu-id="6914a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6914a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6914a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6914a-122">Authorization</span></span>|<span data-ttu-id="6914a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6914a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6914a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6914a-124">Accept</span></span>|<span data-ttu-id="6914a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6914a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6914a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6914a-126">Request body</span></span>
<span data-ttu-id="6914a-127">В теле запроса добавьте представление объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6914a-127">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="6914a-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="6914a-128">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="6914a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6914a-129">Property</span></span>|<span data-ttu-id="6914a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6914a-130">Type</span></span>|<span data-ttu-id="6914a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6914a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6914a-132">id</span><span class="sxs-lookup"><span data-stu-id="6914a-132">id</span></span>|<span data-ttu-id="6914a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6914a-133">String</span></span>|<span data-ttu-id="6914a-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6914a-134">Not yet documented</span></span>|
|<span data-ttu-id="6914a-135">enabled</span><span class="sxs-lookup"><span data-stu-id="6914a-135">enabled</span></span>|<span data-ttu-id="6914a-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="6914a-136">Boolean</span></span>|<span data-ttu-id="6914a-137">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="6914a-137">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="6914a-138">includedGroups</span><span class="sxs-lookup"><span data-stu-id="6914a-138">includedGroups</span></span>|<span data-ttu-id="6914a-139">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="6914a-139">Guid collection</span></span>|<span data-ttu-id="6914a-140">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="6914a-140">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="6914a-141">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="6914a-141">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="6914a-142">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="6914a-142">excludedGroups</span></span>|<span data-ttu-id="6914a-143">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="6914a-143">Guid collection</span></span>|<span data-ttu-id="6914a-144">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="6914a-144">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="6914a-145">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="6914a-145">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="6914a-146">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="6914a-146">overrideDefaultRule</span></span>|<span data-ttu-id="6914a-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="6914a-147">Boolean</span></span>|<span data-ttu-id="6914a-148">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="6914a-148">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="6914a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6914a-149">Response</span></span>
<span data-ttu-id="6914a-150">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6914a-150">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6914a-151">Пример</span><span class="sxs-lookup"><span data-stu-id="6914a-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="6914a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="6914a-152">Request</span></span>
<span data-ttu-id="6914a-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6914a-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="6914a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="6914a-154">Response</span></span>
<span data-ttu-id="6914a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6914a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```





