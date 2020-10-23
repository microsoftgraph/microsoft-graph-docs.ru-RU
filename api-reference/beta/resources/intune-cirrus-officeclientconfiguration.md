---
title: Тип ресурса officeClientConfiguration
description: Настройка клиента Office.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87351ed868a1f46ff769882fea4e12da25aed16e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693999"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="52174-103">Тип ресурса officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="52174-103">officeClientConfiguration resource type</span></span>

<span data-ttu-id="52174-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52174-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52174-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52174-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52174-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52174-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52174-107">Настройка клиента Office.</span><span class="sxs-lookup"><span data-stu-id="52174-107">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="52174-108">Методы</span><span class="sxs-lookup"><span data-stu-id="52174-108">Methods</span></span>
|<span data-ttu-id="52174-109">Метод</span><span class="sxs-lookup"><span data-stu-id="52174-109">Method</span></span>|<span data-ttu-id="52174-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52174-110">Return Type</span></span>|<span data-ttu-id="52174-111">Описание</span><span class="sxs-lookup"><span data-stu-id="52174-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="52174-112">Список Оффицеклиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="52174-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="52174-113">Коллекция [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52174-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="52174-114">Список свойств и связей объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="52174-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="52174-115">Получение officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="52174-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="52174-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="52174-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="52174-117">Чтение свойств и связей объекта [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="52174-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="52174-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="52174-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="52174-119">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="52174-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="52174-120">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="52174-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="52174-121">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="52174-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="52174-122">Нет</span><span class="sxs-lookup"><span data-stu-id="52174-122">None</span></span>|<span data-ttu-id="52174-123">Обновление приоритетов политики.</span><span class="sxs-lookup"><span data-stu-id="52174-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="52174-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="52174-124">Properties</span></span>
|<span data-ttu-id="52174-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="52174-125">Property</span></span>|<span data-ttu-id="52174-126">Тип</span><span class="sxs-lookup"><span data-stu-id="52174-126">Type</span></span>|<span data-ttu-id="52174-127">Описание</span><span class="sxs-lookup"><span data-stu-id="52174-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52174-128">id</span><span class="sxs-lookup"><span data-stu-id="52174-128">id</span></span>|<span data-ttu-id="52174-129">Строка</span><span class="sxs-lookup"><span data-stu-id="52174-129">String</span></span>|<span data-ttu-id="52174-130">Идентификатор политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="52174-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="52174-131">усерпреференцепайлоад</span><span class="sxs-lookup"><span data-stu-id="52174-131">userPreferencePayload</span></span>|<span data-ttu-id="52174-132">Stream</span><span class="sxs-lookup"><span data-stu-id="52174-132">Stream</span></span>|<span data-ttu-id="52174-133">Строка JSON параметров настройки в двоичном формате. Эти значения могут быть переопределены пользователем.</span><span class="sxs-lookup"><span data-stu-id="52174-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="52174-134">полиципайлоад</span><span class="sxs-lookup"><span data-stu-id="52174-134">policyPayload</span></span>|<span data-ttu-id="52174-135">Stream</span><span class="sxs-lookup"><span data-stu-id="52174-135">Stream</span></span>|<span data-ttu-id="52174-136">Строка JSON параметров политики в двоичном формате эти значения не могут быть изменены пользователем.</span><span class="sxs-lookup"><span data-stu-id="52174-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="52174-137">description</span><span class="sxs-lookup"><span data-stu-id="52174-137">description</span></span>|<span data-ttu-id="52174-138">Строка</span><span class="sxs-lookup"><span data-stu-id="52174-138">String</span></span>|<span data-ttu-id="52174-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="52174-139">Not yet documented</span></span>|
|<span data-ttu-id="52174-140">displayName</span><span class="sxs-lookup"><span data-stu-id="52174-140">displayName</span></span>|<span data-ttu-id="52174-141">Строка</span><span class="sxs-lookup"><span data-stu-id="52174-141">String</span></span>|<span data-ttu-id="52174-142">Администратор предоставил описание политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="52174-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="52174-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52174-143">lastModifiedDateTime</span></span>|<span data-ttu-id="52174-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="52174-144">DateTime</span></span>|<span data-ttu-id="52174-145">Метка даты и времени последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="52174-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="52174-146">priority</span><span class="sxs-lookup"><span data-stu-id="52174-146">priority</span></span>|<span data-ttu-id="52174-147">Int32</span><span class="sxs-lookup"><span data-stu-id="52174-147">Int32</span></span>|<span data-ttu-id="52174-148">Значение Priority должно быть уникальным для каждой политики в клиенте и использоваться для разрешения конфликтов, низкие значения имеют высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="52174-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="52174-149">усерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="52174-149">userCheckinSummary</span></span>|[<span data-ttu-id="52174-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="52174-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="52174-151">Сводка по возврату пользователя для политики.</span><span class="sxs-lookup"><span data-stu-id="52174-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="52174-152">чеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="52174-152">checkinStatuses</span></span>|<span data-ttu-id="52174-153">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="52174-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="52174-154">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="52174-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52174-155">Связи</span><span class="sxs-lookup"><span data-stu-id="52174-155">Relationships</span></span>
|<span data-ttu-id="52174-156">Связь</span><span class="sxs-lookup"><span data-stu-id="52174-156">Relationship</span></span>|<span data-ttu-id="52174-157">Тип</span><span class="sxs-lookup"><span data-stu-id="52174-157">Type</span></span>|<span data-ttu-id="52174-158">Описание</span><span class="sxs-lookup"><span data-stu-id="52174-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52174-159">assignments</span><span class="sxs-lookup"><span data-stu-id="52174-159">assignments</span></span>|<span data-ttu-id="52174-160">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="52174-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="52174-161">Список назначений групп для политики.</span><span class="sxs-lookup"><span data-stu-id="52174-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52174-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52174-162">JSON Representation</span></span>
<span data-ttu-id="52174-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52174-163">Here is a JSON representation of the resource.</span></span>
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





