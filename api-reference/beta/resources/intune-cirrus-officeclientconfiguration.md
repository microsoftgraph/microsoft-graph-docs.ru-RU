---
title: Тип ресурса officeClientConfiguration
description: Конфигурация клиента Office.
ms.openlocfilehash: de510d7a57c10d1f74a3e58856afb9233243ec17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077775"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="29475-103">Тип ресурса officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="29475-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="29475-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="29475-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29475-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29475-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29475-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="29475-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29475-107">Конфигурация клиента Office.</span><span class="sxs-lookup"><span data-stu-id="29475-107">Office Client Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="29475-108">Методы</span><span class="sxs-lookup"><span data-stu-id="29475-108">Methods</span></span>
|<span data-ttu-id="29475-109">Метод</span><span class="sxs-lookup"><span data-stu-id="29475-109">Method</span></span>|<span data-ttu-id="29475-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="29475-110">Return Type</span></span>|<span data-ttu-id="29475-111">Описание</span><span class="sxs-lookup"><span data-stu-id="29475-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29475-112">Список officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="29475-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="29475-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="29475-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="29475-114">Свойства списка и связей объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="29475-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="29475-115">Получение officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="29475-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="29475-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="29475-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="29475-117">Чтение свойства и связи объекта [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="29475-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="29475-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="29475-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="29475-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="29475-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="29475-120">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="29475-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="29475-121">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="29475-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="29475-122">Нет</span><span class="sxs-lookup"><span data-stu-id="29475-122">None</span></span>|<span data-ttu-id="29475-123">Обновление политики приоритетов.</span><span class="sxs-lookup"><span data-stu-id="29475-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="29475-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="29475-124">Properties</span></span>
|<span data-ttu-id="29475-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="29475-125">Property</span></span>|<span data-ttu-id="29475-126">Тип</span><span class="sxs-lookup"><span data-stu-id="29475-126">Type</span></span>|<span data-ttu-id="29475-127">Описание</span><span class="sxs-lookup"><span data-stu-id="29475-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29475-128">id</span><span class="sxs-lookup"><span data-stu-id="29475-128">id</span></span>|<span data-ttu-id="29475-129">String</span><span class="sxs-lookup"><span data-stu-id="29475-129">String</span></span>|<span data-ttu-id="29475-130">Идентификатор политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="29475-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="29475-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="29475-131">userPreferencePayload</span></span>|<span data-ttu-id="29475-132">Stream</span><span class="sxs-lookup"><span data-stu-id="29475-132">Stream</span></span>|<span data-ttu-id="29475-133">Строка настройки JSON в двоичном формате, эти значения можно переопределить пользователем.</span><span class="sxs-lookup"><span data-stu-id="29475-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="29475-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="29475-134">policyPayload</span></span>|<span data-ttu-id="29475-135">Stream</span><span class="sxs-lookup"><span data-stu-id="29475-135">Stream</span></span>|<span data-ttu-id="29475-136">Параметры политики JSON string в двоичном формате, пользователь не может изменить эти значения.</span><span class="sxs-lookup"><span data-stu-id="29475-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="29475-137">описание</span><span class="sxs-lookup"><span data-stu-id="29475-137">description</span></span>|<span data-ttu-id="29475-138">String</span><span class="sxs-lookup"><span data-stu-id="29475-138">String</span></span>|<span data-ttu-id="29475-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="29475-139">Not yet documented</span></span>|
|<span data-ttu-id="29475-140">displayName</span><span class="sxs-lookup"><span data-stu-id="29475-140">displayName</span></span>|<span data-ttu-id="29475-141">String</span><span class="sxs-lookup"><span data-stu-id="29475-141">String</span></span>|<span data-ttu-id="29475-142">Admin предоставляются описание клиента office конфигурации политики.</span><span class="sxs-lookup"><span data-stu-id="29475-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="29475-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29475-143">lastModifiedDateTime</span></span>|<span data-ttu-id="29475-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="29475-144">DateTime</span></span>|<span data-ttu-id="29475-145">Отметка измененные даты и времени последнего политики.</span><span class="sxs-lookup"><span data-stu-id="29475-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="29475-146">priority</span><span class="sxs-lookup"><span data-stu-id="29475-146">priority</span></span>|<span data-ttu-id="29475-147">Int32</span><span class="sxs-lookup"><span data-stu-id="29475-147">Int32</span></span>|<span data-ttu-id="29475-148">Значение приоритета должно быть уникальное значение для каждой политики в области клиента и будет использоваться для разрешения конфликтов, меньшее значение означает, что высокого приоритета.</span><span class="sxs-lookup"><span data-stu-id="29475-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="29475-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="29475-149">userCheckinSummary</span></span>|[<span data-ttu-id="29475-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="29475-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="29475-151">Возврат Сводка пользователей для политики.</span><span class="sxs-lookup"><span data-stu-id="29475-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="29475-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="29475-152">checkinStatuses</span></span>|<span data-ttu-id="29475-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="29475-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="29475-154">Список office состояние возврата клиента.</span><span class="sxs-lookup"><span data-stu-id="29475-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29475-155">Связи</span><span class="sxs-lookup"><span data-stu-id="29475-155">Relationships</span></span>
|<span data-ttu-id="29475-156">Связь</span><span class="sxs-lookup"><span data-stu-id="29475-156">Relationship</span></span>|<span data-ttu-id="29475-157">Тип</span><span class="sxs-lookup"><span data-stu-id="29475-157">Type</span></span>|<span data-ttu-id="29475-158">Описание</span><span class="sxs-lookup"><span data-stu-id="29475-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29475-159">assignments</span><span class="sxs-lookup"><span data-stu-id="29475-159">assignments</span></span>|<span data-ttu-id="29475-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="29475-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="29475-161">Список назначений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="29475-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29475-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29475-162">JSON Representation</span></span>
<span data-ttu-id="29475-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29475-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```



