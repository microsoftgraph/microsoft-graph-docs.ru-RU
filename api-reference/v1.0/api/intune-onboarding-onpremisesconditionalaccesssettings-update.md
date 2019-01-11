---
title: Обновление объекта onPremisesConditionalAccessSettings
description: Обновляет свойства объекта onPremisesConditionalAccessSettings.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 761da1d549430c1f49f2d68b05194bffea661618
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889784"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="a7278-103">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="a7278-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="a7278-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a7278-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7278-105">Обновляет свойства объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="a7278-105">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7278-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7278-106">Prerequisites</span></span>
<span data-ttu-id="a7278-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7278-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7278-109">Permission type</span></span>|<span data-ttu-id="a7278-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7278-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7278-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7278-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7278-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7278-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a7278-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7278-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7278-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7278-114">Not supported.</span></span>|
|<span data-ttu-id="a7278-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7278-115">Application</span></span>|<span data-ttu-id="a7278-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7278-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7278-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7278-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="a7278-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7278-118">Request headers</span></span>
|<span data-ttu-id="a7278-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7278-119">Header</span></span>|<span data-ttu-id="a7278-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a7278-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7278-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7278-121">Authorization</span></span>|<span data-ttu-id="a7278-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a7278-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7278-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a7278-123">Accept</span></span>|<span data-ttu-id="a7278-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a7278-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7278-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7278-125">Request body</span></span>
<span data-ttu-id="a7278-126">В теле запроса добавьте представление объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7278-126">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="a7278-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="a7278-127">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="a7278-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7278-128">Property</span></span>|<span data-ttu-id="a7278-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a7278-129">Type</span></span>|<span data-ttu-id="a7278-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a7278-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7278-131">id</span><span class="sxs-lookup"><span data-stu-id="a7278-131">id</span></span>|<span data-ttu-id="a7278-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a7278-132">String</span></span>|<span data-ttu-id="a7278-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a7278-133">Not yet documented</span></span>|
|<span data-ttu-id="a7278-134">enabled</span><span class="sxs-lookup"><span data-stu-id="a7278-134">enabled</span></span>|<span data-ttu-id="a7278-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7278-135">Boolean</span></span>|<span data-ttu-id="a7278-136">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="a7278-136">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="a7278-137">includedGroups</span><span class="sxs-lookup"><span data-stu-id="a7278-137">includedGroups</span></span>|<span data-ttu-id="a7278-138">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="a7278-138">Guid collection</span></span>|<span data-ttu-id="a7278-139">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="a7278-139">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="a7278-140">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="a7278-140">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="a7278-141">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="a7278-141">excludedGroups</span></span>|<span data-ttu-id="a7278-142">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="a7278-142">Guid collection</span></span>|<span data-ttu-id="a7278-143">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="a7278-143">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="a7278-144">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="a7278-144">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="a7278-145">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="a7278-145">overrideDefaultRule</span></span>|<span data-ttu-id="a7278-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7278-146">Boolean</span></span>|<span data-ttu-id="a7278-147">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="a7278-147">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="a7278-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7278-148">Response</span></span>
<span data-ttu-id="a7278-149">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a7278-149">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7278-150">Пример</span><span class="sxs-lookup"><span data-stu-id="a7278-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7278-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7278-151">Request</span></span>
<span data-ttu-id="a7278-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7278-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7278-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7278-153">Response</span></span>
<span data-ttu-id="a7278-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a7278-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



