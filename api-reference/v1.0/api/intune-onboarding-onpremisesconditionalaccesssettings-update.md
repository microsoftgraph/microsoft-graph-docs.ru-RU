---
title: Обновление объекта onPremisesConditionalAccessSettings
description: Обновляет свойства объекта onPremisesConditionalAccessSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e77767900b40fc3f921d9d3ffd34fd6930bf19c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024086"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="0c92c-103">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0c92c-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="0c92c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c92c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c92c-105">Обновляет свойства объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="0c92c-105">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c92c-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c92c-106">Prerequisites</span></span>
<span data-ttu-id="0c92c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c92c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c92c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c92c-109">Permission type</span></span>|<span data-ttu-id="0c92c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c92c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c92c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c92c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c92c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c92c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c92c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c92c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c92c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c92c-114">Not supported.</span></span>|
|<span data-ttu-id="0c92c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c92c-115">Application</span></span>|<span data-ttu-id="0c92c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c92c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c92c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c92c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="0c92c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c92c-118">Request headers</span></span>
|<span data-ttu-id="0c92c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c92c-119">Header</span></span>|<span data-ttu-id="0c92c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0c92c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c92c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c92c-121">Authorization</span></span>|<span data-ttu-id="0c92c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c92c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c92c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0c92c-123">Accept</span></span>|<span data-ttu-id="0c92c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0c92c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c92c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c92c-125">Request body</span></span>
<span data-ttu-id="0c92c-126">В теле запроса добавьте представление объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c92c-126">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="0c92c-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="0c92c-127">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="0c92c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c92c-128">Property</span></span>|<span data-ttu-id="0c92c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0c92c-129">Type</span></span>|<span data-ttu-id="0c92c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0c92c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c92c-131">id</span><span class="sxs-lookup"><span data-stu-id="0c92c-131">id</span></span>|<span data-ttu-id="0c92c-132">String</span><span class="sxs-lookup"><span data-stu-id="0c92c-132">String</span></span>|<span data-ttu-id="0c92c-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0c92c-133">Not yet documented</span></span>|
|<span data-ttu-id="0c92c-134">enabled</span><span class="sxs-lookup"><span data-stu-id="0c92c-134">enabled</span></span>|<span data-ttu-id="0c92c-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c92c-135">Boolean</span></span>|<span data-ttu-id="0c92c-136">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="0c92c-136">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="0c92c-137">includedGroups</span><span class="sxs-lookup"><span data-stu-id="0c92c-137">includedGroups</span></span>|<span data-ttu-id="0c92c-138">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="0c92c-138">Guid collection</span></span>|<span data-ttu-id="0c92c-139">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="0c92c-139">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="0c92c-140">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="0c92c-140">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="0c92c-141">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="0c92c-141">excludedGroups</span></span>|<span data-ttu-id="0c92c-142">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="0c92c-142">Guid collection</span></span>|<span data-ttu-id="0c92c-143">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="0c92c-143">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="0c92c-144">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="0c92c-144">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="0c92c-145">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="0c92c-145">overrideDefaultRule</span></span>|<span data-ttu-id="0c92c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c92c-146">Boolean</span></span>|<span data-ttu-id="0c92c-147">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="0c92c-147">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="0c92c-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c92c-148">Response</span></span>
<span data-ttu-id="0c92c-149">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0c92c-149">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c92c-150">Пример</span><span class="sxs-lookup"><span data-stu-id="0c92c-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c92c-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c92c-151">Request</span></span>
<span data-ttu-id="0c92c-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c92c-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
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

### <a name="response"></a><span data-ttu-id="0c92c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c92c-153">Response</span></span>
<span data-ttu-id="0c92c-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c92c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



