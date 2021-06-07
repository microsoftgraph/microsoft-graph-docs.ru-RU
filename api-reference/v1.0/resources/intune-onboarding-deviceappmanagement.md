---
title: Тип ресурса deviceAppManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae8bd6389d40b45d59d82d183fcfa6b3a2327367
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753502"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="05602-103">Тип ресурса deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="05602-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="05602-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05602-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05602-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05602-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05602-106">Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.</span><span class="sxs-lookup"><span data-stu-id="05602-106">Singleton entity that acts as a container for all device app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="05602-107">Методы</span><span class="sxs-lookup"><span data-stu-id="05602-107">Methods</span></span>
|<span data-ttu-id="05602-108">Метод</span><span class="sxs-lookup"><span data-stu-id="05602-108">Method</span></span>|<span data-ttu-id="05602-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05602-109">Return Type</span></span>|<span data-ttu-id="05602-110">Описание</span><span class="sxs-lookup"><span data-stu-id="05602-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05602-111">Получение объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="05602-111">Get deviceAppManagement</span></span>](../api/intune-onboarding-deviceappmanagement-get.md)|[<span data-ttu-id="05602-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="05602-112">deviceAppManagement</span></span>](../resources/intune-onboarding-deviceappmanagement.md)|<span data-ttu-id="05602-113">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="05602-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="05602-114">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="05602-114">Update deviceAppManagement</span></span>](../api/intune-onboarding-deviceappmanagement-update.md)|[<span data-ttu-id="05602-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="05602-115">deviceAppManagement</span></span>](../resources/intune-onboarding-deviceappmanagement.md)|<span data-ttu-id="05602-116">Обновление свойств объекта [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="05602-116">Update the properties of a [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="05602-117">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="05602-117">syncMicrosoftStoreForBusinessApps action</span></span>](../api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|<span data-ttu-id="05602-118">Нет</span><span class="sxs-lookup"><span data-stu-id="05602-118">None</span></span>|<span data-ttu-id="05602-119">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="05602-119">Syncs Intune account with Microsoft Store For Business</span></span>|

## <a name="properties"></a><span data-ttu-id="05602-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="05602-120">Properties</span></span>
|<span data-ttu-id="05602-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="05602-121">Property</span></span>|<span data-ttu-id="05602-122">Тип</span><span class="sxs-lookup"><span data-stu-id="05602-122">Type</span></span>|<span data-ttu-id="05602-123">Описание</span><span class="sxs-lookup"><span data-stu-id="05602-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05602-124">id</span><span class="sxs-lookup"><span data-stu-id="05602-124">id</span></span>|<span data-ttu-id="05602-125">String</span><span class="sxs-lookup"><span data-stu-id="05602-125">String</span></span>|<span data-ttu-id="05602-126">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05602-126">Not yet documented</span></span>|
|<span data-ttu-id="05602-127">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="05602-127">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="05602-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05602-128">DateTimeOffset</span></span>|<span data-ttu-id="05602-129">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="05602-129">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="05602-130">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="05602-130">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="05602-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="05602-131">Boolean</span></span>|<span data-ttu-id="05602-132">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="05602-132">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="05602-133">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="05602-133">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="05602-134">String</span><span class="sxs-lookup"><span data-stu-id="05602-134">String</span></span>|<span data-ttu-id="05602-135">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="05602-135">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="05602-136">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="05602-136">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="05602-137">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="05602-137">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="05602-138">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="05602-138">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="05602-139">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="05602-139">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="05602-140">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="05602-140">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="05602-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05602-141">DateTimeOffset</span></span>|<span data-ttu-id="05602-142">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="05602-142">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05602-143">Связи</span><span class="sxs-lookup"><span data-stu-id="05602-143">Relationships</span></span>
|<span data-ttu-id="05602-144">Связь</span><span class="sxs-lookup"><span data-stu-id="05602-144">Relationship</span></span>|<span data-ttu-id="05602-145">Тип</span><span class="sxs-lookup"><span data-stu-id="05602-145">Type</span></span>|<span data-ttu-id="05602-146">Описание</span><span class="sxs-lookup"><span data-stu-id="05602-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05602-147">VPP токены</span><span class="sxs-lookup"><span data-stu-id="05602-147">vppTokens</span></span>|<span data-ttu-id="05602-148">[vpp Токен](../resources/intune-onboarding-vpptoken.md) коллекция</span><span class="sxs-lookup"><span data-stu-id="05602-148">[vppToken](../resources/intune-onboarding-vpptoken.md) collection</span></span>|<span data-ttu-id="05602-149">Список Vpp маркеров для данной организации.</span><span class="sxs-lookup"><span data-stu-id="05602-149">List of Vpp tokens for this organization.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05602-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05602-150">JSON Representation</span></span>
<span data-ttu-id="05602-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05602-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```




