---
title: Тип ресурса remoteAssistancePartner
description: Ресурсы Ремотеассистпартнер представляют метаданные и состояние данной службы партнерской службы удаленного помощника.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3343d0e9d68c76db91f1153704176d70b06a7483
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566306"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="bbae9-103">Тип ресурса remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="bbae9-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="bbae9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbae9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbae9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbae9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbae9-106">Ресурсы Ремотеассистпартнер представляют метаданные и состояние данной службы партнерской службы удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="bbae9-106">RemoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="bbae9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bbae9-107">Methods</span></span>
|<span data-ttu-id="bbae9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bbae9-108">Method</span></span>|<span data-ttu-id="bbae9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bbae9-109">Return Type</span></span>|<span data-ttu-id="bbae9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bbae9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bbae9-111">Список объектов remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="bbae9-111">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="bbae9-112">Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)</span><span class="sxs-lookup"><span data-stu-id="bbae9-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="bbae9-113">Список свойств и связей объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="bbae9-113">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="bbae9-114">Получение объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="bbae9-114">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="bbae9-115">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="bbae9-115">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="bbae9-116">Чтение свойств и связей объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="bbae9-116">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="bbae9-117">Создание объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="bbae9-117">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="bbae9-118">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="bbae9-118">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="bbae9-119">Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="bbae9-119">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="bbae9-120">Удаление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="bbae9-120">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="bbae9-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bbae9-121">None</span></span>|<span data-ttu-id="bbae9-122">Удаляет объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="bbae9-122">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="bbae9-123">Обновление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="bbae9-123">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="bbae9-124">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="bbae9-124">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="bbae9-125">Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="bbae9-125">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="bbae9-126">Действие beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="bbae9-126">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="bbae9-127">Нет</span><span class="sxs-lookup"><span data-stu-id="bbae9-127">None</span></span>|<span data-ttu-id="bbae9-128">Запрос на запуск входящей миграции.</span><span class="sxs-lookup"><span data-stu-id="bbae9-128">A request to start onboarding.</span></span>  <span data-ttu-id="bbae9-129">Должен быть связан с соответствующими сведениями учетной записи TeamViewer</span><span class="sxs-lookup"><span data-stu-id="bbae9-129">Must be coupled with the appropriate TeamViewer account information</span></span>|
|[<span data-ttu-id="bbae9-130">Действие disconnect</span><span class="sxs-lookup"><span data-stu-id="bbae9-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="bbae9-131">Нет</span><span class="sxs-lookup"><span data-stu-id="bbae9-131">None</span></span>|<span data-ttu-id="bbae9-132">Запрос на удаление активного соединителя TeamViewer Connector</span><span class="sxs-lookup"><span data-stu-id="bbae9-132">A request to remove the active TeamViewer connector</span></span>|

## <a name="properties"></a><span data-ttu-id="bbae9-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbae9-133">Properties</span></span>
|<span data-ttu-id="bbae9-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbae9-134">Property</span></span>|<span data-ttu-id="bbae9-135">Тип</span><span class="sxs-lookup"><span data-stu-id="bbae9-135">Type</span></span>|<span data-ttu-id="bbae9-136">Описание</span><span class="sxs-lookup"><span data-stu-id="bbae9-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbae9-137">id</span><span class="sxs-lookup"><span data-stu-id="bbae9-137">id</span></span>|<span data-ttu-id="bbae9-138">String</span><span class="sxs-lookup"><span data-stu-id="bbae9-138">String</span></span>|<span data-ttu-id="bbae9-139">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="bbae9-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="bbae9-140">displayName</span><span class="sxs-lookup"><span data-stu-id="bbae9-140">displayName</span></span>|<span data-ttu-id="bbae9-141">Строка</span><span class="sxs-lookup"><span data-stu-id="bbae9-141">String</span></span>|<span data-ttu-id="bbae9-142">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="bbae9-142">Display name of the partner.</span></span>|
|<span data-ttu-id="bbae9-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="bbae9-143">onboardingUrl</span></span>|<span data-ttu-id="bbae9-144">String</span><span class="sxs-lookup"><span data-stu-id="bbae9-144">String</span></span>|<span data-ttu-id="bbae9-145">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="bbae9-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="bbae9-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="bbae9-146">onboardingStatus</span></span>|[<span data-ttu-id="bbae9-147">Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="bbae9-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="bbae9-148">Понятное описание состояния текущего соединителя TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="bbae9-148">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="bbae9-149">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="bbae9-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="bbae9-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="bbae9-150">lastConnectionDateTime</span></span>|<span data-ttu-id="bbae9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbae9-151">DateTimeOffset</span></span>|<span data-ttu-id="bbae9-152">Метка времени последнего запроса, отправленного службе Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="bbae9-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbae9-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="bbae9-153">Relationships</span></span>
<span data-ttu-id="bbae9-154">Нет</span><span class="sxs-lookup"><span data-stu-id="bbae9-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbae9-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbae9-155">JSON Representation</span></span>
<span data-ttu-id="bbae9-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbae9-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```





