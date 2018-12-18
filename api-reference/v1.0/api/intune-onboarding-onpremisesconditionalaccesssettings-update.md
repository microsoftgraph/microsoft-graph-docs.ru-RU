---
title: Обновление объекта onPremisesConditionalAccessSettings
description: Обновляет свойства объекта onPremisesConditionalAccessSettings.
author: tfitzmac
ms.openlocfilehash: 255693dfa1bb53083f792da950333a5c05717f1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346804"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="49306-103">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="49306-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="49306-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="49306-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49306-105">Обновляет свойства объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="49306-105">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49306-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49306-106">Prerequisites</span></span>
<span data-ttu-id="49306-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49306-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49306-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49306-109">Permission type</span></span>|<span data-ttu-id="49306-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49306-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49306-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49306-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49306-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49306-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49306-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49306-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49306-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49306-114">Not supported.</span></span>|
|<span data-ttu-id="49306-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49306-115">Application</span></span>|<span data-ttu-id="49306-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49306-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49306-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49306-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="49306-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49306-118">Request headers</span></span>
|<span data-ttu-id="49306-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49306-119">Header</span></span>|<span data-ttu-id="49306-120">Значение</span><span class="sxs-lookup"><span data-stu-id="49306-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49306-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49306-121">Authorization</span></span>|<span data-ttu-id="49306-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="49306-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49306-123">Accept</span><span class="sxs-lookup"><span data-stu-id="49306-123">Accept</span></span>|<span data-ttu-id="49306-124">application/json</span><span class="sxs-lookup"><span data-stu-id="49306-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49306-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49306-125">Request body</span></span>
<span data-ttu-id="49306-126">В теле запроса добавьте представление объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49306-126">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="49306-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="49306-127">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="49306-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="49306-128">Property</span></span>|<span data-ttu-id="49306-129">Тип</span><span class="sxs-lookup"><span data-stu-id="49306-129">Type</span></span>|<span data-ttu-id="49306-130">Описание</span><span class="sxs-lookup"><span data-stu-id="49306-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49306-131">id</span><span class="sxs-lookup"><span data-stu-id="49306-131">id</span></span>|<span data-ttu-id="49306-132">Строка</span><span class="sxs-lookup"><span data-stu-id="49306-132">String</span></span>|<span data-ttu-id="49306-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="49306-133">Not yet documented</span></span>|
|<span data-ttu-id="49306-134">enabled</span><span class="sxs-lookup"><span data-stu-id="49306-134">enabled</span></span>|<span data-ttu-id="49306-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="49306-135">Boolean</span></span>|<span data-ttu-id="49306-136">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="49306-136">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="49306-137">includedGroups</span><span class="sxs-lookup"><span data-stu-id="49306-137">includedGroups</span></span>|<span data-ttu-id="49306-138">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="49306-138">Guid collection</span></span>|<span data-ttu-id="49306-139">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="49306-139">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="49306-140">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="49306-140">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="49306-141">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="49306-141">excludedGroups</span></span>|<span data-ttu-id="49306-142">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="49306-142">Guid collection</span></span>|<span data-ttu-id="49306-143">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="49306-143">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="49306-144">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="49306-144">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="49306-145">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="49306-145">overrideDefaultRule</span></span>|<span data-ttu-id="49306-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="49306-146">Boolean</span></span>|<span data-ttu-id="49306-147">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="49306-147">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="49306-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="49306-148">Response</span></span>
<span data-ttu-id="49306-149">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="49306-149">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49306-150">Пример</span><span class="sxs-lookup"><span data-stu-id="49306-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="49306-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="49306-151">Request</span></span>
<span data-ttu-id="49306-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49306-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="49306-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="49306-153">Response</span></span>
<span data-ttu-id="49306-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="49306-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



