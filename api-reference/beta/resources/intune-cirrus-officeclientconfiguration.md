---
title: Тип ресурса officeClientConfiguration
description: Настройка клиента Office.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a8371da85ee4bbc54943a8fbb29ec99dcb49a49
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561315"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="556dc-103">Тип ресурса officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="556dc-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="556dc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="556dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="556dc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="556dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="556dc-106">Настройка клиента Office.</span><span class="sxs-lookup"><span data-stu-id="556dc-106">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="556dc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="556dc-107">Methods</span></span>
|<span data-ttu-id="556dc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="556dc-108">Method</span></span>|<span data-ttu-id="556dc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="556dc-109">Return Type</span></span>|<span data-ttu-id="556dc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="556dc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="556dc-111">Список Оффицеклиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="556dc-111">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="556dc-112">Коллекция [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="556dc-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="556dc-113">Список свойств и связей объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="556dc-113">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="556dc-114">Получение officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="556dc-114">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="556dc-115">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="556dc-115">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="556dc-116">Чтение свойств и связей объекта [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="556dc-116">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="556dc-117">Действие assign</span><span class="sxs-lookup"><span data-stu-id="556dc-117">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="556dc-118">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="556dc-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="556dc-119">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="556dc-119">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="556dc-120">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="556dc-120">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="556dc-121">Нет</span><span class="sxs-lookup"><span data-stu-id="556dc-121">None</span></span>|<span data-ttu-id="556dc-122">Обновление приоритетов политики.</span><span class="sxs-lookup"><span data-stu-id="556dc-122">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="556dc-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="556dc-123">Properties</span></span>
|<span data-ttu-id="556dc-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="556dc-124">Property</span></span>|<span data-ttu-id="556dc-125">Тип</span><span class="sxs-lookup"><span data-stu-id="556dc-125">Type</span></span>|<span data-ttu-id="556dc-126">Описание</span><span class="sxs-lookup"><span data-stu-id="556dc-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="556dc-127">id</span><span class="sxs-lookup"><span data-stu-id="556dc-127">id</span></span>|<span data-ttu-id="556dc-128">Строка</span><span class="sxs-lookup"><span data-stu-id="556dc-128">String</span></span>|<span data-ttu-id="556dc-129">Идентификатор политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="556dc-129">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="556dc-130">Усерпреференцепайлоад</span><span class="sxs-lookup"><span data-stu-id="556dc-130">userPreferencePayload</span></span>|<span data-ttu-id="556dc-131">Поток</span><span class="sxs-lookup"><span data-stu-id="556dc-131">Stream</span></span>|<span data-ttu-id="556dc-132">Строка JSON параметров настройки в двоичном формате. Эти значения могут быть переопределены пользователем.</span><span class="sxs-lookup"><span data-stu-id="556dc-132">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="556dc-133">Полиципайлоад</span><span class="sxs-lookup"><span data-stu-id="556dc-133">policyPayload</span></span>|<span data-ttu-id="556dc-134">Поток</span><span class="sxs-lookup"><span data-stu-id="556dc-134">Stream</span></span>|<span data-ttu-id="556dc-135">Строка JSON параметров политики в двоичном формате эти значения не могут быть изменены пользователем.</span><span class="sxs-lookup"><span data-stu-id="556dc-135">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="556dc-136">description</span><span class="sxs-lookup"><span data-stu-id="556dc-136">description</span></span>|<span data-ttu-id="556dc-137">String</span><span class="sxs-lookup"><span data-stu-id="556dc-137">String</span></span>|<span data-ttu-id="556dc-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="556dc-138">Not yet documented</span></span>|
|<span data-ttu-id="556dc-139">displayName</span><span class="sxs-lookup"><span data-stu-id="556dc-139">displayName</span></span>|<span data-ttu-id="556dc-140">String</span><span class="sxs-lookup"><span data-stu-id="556dc-140">String</span></span>|<span data-ttu-id="556dc-141">Администратор предоставил описание политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="556dc-141">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="556dc-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="556dc-142">lastModifiedDateTime</span></span>|<span data-ttu-id="556dc-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="556dc-143">DateTime</span></span>|<span data-ttu-id="556dc-144">Метка даты и времени последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="556dc-144">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="556dc-145">priority</span><span class="sxs-lookup"><span data-stu-id="556dc-145">priority</span></span>|<span data-ttu-id="556dc-146">Int32</span><span class="sxs-lookup"><span data-stu-id="556dc-146">Int32</span></span>|<span data-ttu-id="556dc-147">Значение Priority должно быть уникальным для каждой политики в клиенте и использоваться для разрешения конфликтов, низкие значения имеют высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="556dc-147">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="556dc-148">Усерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="556dc-148">userCheckinSummary</span></span>|[<span data-ttu-id="556dc-149">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="556dc-149">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="556dc-150">Сводка по возврату пользователя для политики.</span><span class="sxs-lookup"><span data-stu-id="556dc-150">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="556dc-151">Чеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="556dc-151">checkinStatuses</span></span>|<span data-ttu-id="556dc-152">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="556dc-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="556dc-153">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="556dc-153">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="556dc-154">Связи</span><span class="sxs-lookup"><span data-stu-id="556dc-154">Relationships</span></span>
|<span data-ttu-id="556dc-155">Отношение</span><span class="sxs-lookup"><span data-stu-id="556dc-155">Relationship</span></span>|<span data-ttu-id="556dc-156">Тип</span><span class="sxs-lookup"><span data-stu-id="556dc-156">Type</span></span>|<span data-ttu-id="556dc-157">Описание</span><span class="sxs-lookup"><span data-stu-id="556dc-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="556dc-158">assignments</span><span class="sxs-lookup"><span data-stu-id="556dc-158">assignments</span></span>|<span data-ttu-id="556dc-159">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="556dc-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="556dc-160">Список назначений групп для политики.</span><span class="sxs-lookup"><span data-stu-id="556dc-160">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="556dc-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="556dc-161">JSON Representation</span></span>
<span data-ttu-id="556dc-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="556dc-162">Here is a JSON representation of the resource.</span></span>
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



