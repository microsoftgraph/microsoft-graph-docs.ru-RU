---
title: Обновление объекта onPremisesConditionalAccessSettings
description: Обновляет свойства объекта onPremisesConditionalAccessSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 51b27d551f4cd34c8472781b750bebc87941a9ee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943944"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="f7fe6-103">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f7fe6-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="f7fe6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7fe6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7fe6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7fe6-107">Обновляет свойства объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe6-107">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7fe6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f7fe6-108">Prerequisites</span></span>
<span data-ttu-id="f7fe6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7fe6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7fe6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7fe6-111">Permission type</span></span>|<span data-ttu-id="f7fe6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7fe6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7fe6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7fe6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7fe6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f7fe6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7fe6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7fe6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-116">Not supported.</span></span>|
|<span data-ttu-id="f7fe6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7fe6-117">Application</span></span>|<span data-ttu-id="f7fe6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7fe6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7fe6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="f7fe6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7fe6-120">Request headers</span></span>
|<span data-ttu-id="f7fe6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7fe6-121">Header</span></span>|<span data-ttu-id="f7fe6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7fe6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7fe6-123">Authorization</span></span>|<span data-ttu-id="f7fe6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f7fe6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7fe6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7fe6-125">Accept</span></span>|<span data-ttu-id="f7fe6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7fe6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7fe6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7fe6-127">Request body</span></span>
<span data-ttu-id="f7fe6-128">В теле запроса добавьте представление объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-128">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="f7fe6-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe6-129">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="f7fe6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7fe6-130">Property</span></span>|<span data-ttu-id="f7fe6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7fe6-131">Type</span></span>|<span data-ttu-id="f7fe6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7fe6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7fe6-133">id</span><span class="sxs-lookup"><span data-stu-id="f7fe6-133">id</span></span>|<span data-ttu-id="f7fe6-134">String</span><span class="sxs-lookup"><span data-stu-id="f7fe6-134">String</span></span>|<span data-ttu-id="f7fe6-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7fe6-135">Not yet documented</span></span>|
|<span data-ttu-id="f7fe6-136">enabled</span><span class="sxs-lookup"><span data-stu-id="f7fe6-136">enabled</span></span>|<span data-ttu-id="f7fe6-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7fe6-137">Boolean</span></span>|<span data-ttu-id="f7fe6-138">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="f7fe6-138">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="f7fe6-139">includedGroups</span><span class="sxs-lookup"><span data-stu-id="f7fe6-139">includedGroups</span></span>|<span data-ttu-id="f7fe6-140">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="f7fe6-140">Guid collection</span></span>|<span data-ttu-id="f7fe6-141">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-141">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="f7fe6-142">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-142">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="f7fe6-143">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="f7fe6-143">excludedGroups</span></span>|<span data-ttu-id="f7fe6-144">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="f7fe6-144">Guid collection</span></span>|<span data-ttu-id="f7fe6-145">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-145">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="f7fe6-146">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-146">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="f7fe6-147">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="f7fe6-147">overrideDefaultRule</span></span>|<span data-ttu-id="f7fe6-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7fe6-148">Boolean</span></span>|<span data-ttu-id="f7fe6-149">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-149">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="f7fe6-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7fe6-150">Response</span></span>
<span data-ttu-id="f7fe6-151">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-151">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7fe6-152">Пример</span><span class="sxs-lookup"><span data-stu-id="f7fe6-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="f7fe6-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7fe6-153">Request</span></span>
<span data-ttu-id="f7fe6-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 201

{
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

### <a name="response"></a><span data-ttu-id="f7fe6-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7fe6-155">Response</span></span>
<span data-ttu-id="f7fe6-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f7fe6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





