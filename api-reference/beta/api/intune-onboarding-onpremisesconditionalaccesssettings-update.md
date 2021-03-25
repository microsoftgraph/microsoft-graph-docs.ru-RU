---
title: Обновление объекта onPremisesConditionalAccessSettings
description: Обновляет свойства объекта onPremisesConditionalAccessSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ddbf3995677150713def936a5cd26eda471ab0a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156858"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="45d97-103">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="45d97-103">Update onPremisesConditionalAccessSettings</span></span>

<span data-ttu-id="45d97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45d97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45d97-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45d97-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45d97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45d97-107">Обновляет свойства объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="45d97-107">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45d97-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45d97-108">Prerequisites</span></span>
<span data-ttu-id="45d97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45d97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45d97-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45d97-111">Permission type</span></span>|<span data-ttu-id="45d97-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45d97-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45d97-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45d97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45d97-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d97-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="45d97-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45d97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45d97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d97-116">Not supported.</span></span>|
|<span data-ttu-id="45d97-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="45d97-117">Application</span></span>|<span data-ttu-id="45d97-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d97-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45d97-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45d97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="45d97-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45d97-120">Request headers</span></span>
|<span data-ttu-id="45d97-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45d97-121">Header</span></span>|<span data-ttu-id="45d97-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45d97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45d97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45d97-123">Authorization</span></span>|<span data-ttu-id="45d97-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45d97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45d97-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45d97-125">Accept</span></span>|<span data-ttu-id="45d97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45d97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45d97-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45d97-127">Request body</span></span>
<span data-ttu-id="45d97-128">В теле запроса добавьте представление объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45d97-128">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="45d97-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="45d97-129">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="45d97-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="45d97-130">Property</span></span>|<span data-ttu-id="45d97-131">Тип</span><span class="sxs-lookup"><span data-stu-id="45d97-131">Type</span></span>|<span data-ttu-id="45d97-132">Описание</span><span class="sxs-lookup"><span data-stu-id="45d97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45d97-133">id</span><span class="sxs-lookup"><span data-stu-id="45d97-133">id</span></span>|<span data-ttu-id="45d97-134">Строка</span><span class="sxs-lookup"><span data-stu-id="45d97-134">String</span></span>|<span data-ttu-id="45d97-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="45d97-135">Not yet documented</span></span>|
|<span data-ttu-id="45d97-136">enabled</span><span class="sxs-lookup"><span data-stu-id="45d97-136">enabled</span></span>|<span data-ttu-id="45d97-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="45d97-137">Boolean</span></span>|<span data-ttu-id="45d97-138">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="45d97-138">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="45d97-139">includedGroups</span><span class="sxs-lookup"><span data-stu-id="45d97-139">includedGroups</span></span>|<span data-ttu-id="45d97-140">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="45d97-140">Guid collection</span></span>|<span data-ttu-id="45d97-141">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="45d97-141">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="45d97-142">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="45d97-142">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="45d97-143">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="45d97-143">excludedGroups</span></span>|<span data-ttu-id="45d97-144">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="45d97-144">Guid collection</span></span>|<span data-ttu-id="45d97-145">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="45d97-145">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="45d97-146">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="45d97-146">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="45d97-147">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="45d97-147">overrideDefaultRule</span></span>|<span data-ttu-id="45d97-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="45d97-148">Boolean</span></span>|<span data-ttu-id="45d97-149">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="45d97-149">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="45d97-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="45d97-150">Response</span></span>
<span data-ttu-id="45d97-151">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45d97-151">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45d97-152">Пример</span><span class="sxs-lookup"><span data-stu-id="45d97-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="45d97-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="45d97-153">Request</span></span>
<span data-ttu-id="45d97-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45d97-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45d97-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="45d97-155">Response</span></span>
<span data-ttu-id="45d97-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45d97-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




