---
title: Тип ресурса Граупполиципресентатион
description: Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d6abbcde241059a15969236b3ab7bcb0825d67d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166880"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="be86c-103">Тип ресурса Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="be86c-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="be86c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be86c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be86c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be86c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be86c-106">Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.</span><span class="sxs-lookup"><span data-stu-id="be86c-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="be86c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="be86c-107">Methods</span></span>
|<span data-ttu-id="be86c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="be86c-108">Method</span></span>|<span data-ttu-id="be86c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be86c-109">Return Type</span></span>|<span data-ttu-id="be86c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be86c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be86c-111">Получение Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="be86c-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="be86c-112">Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="be86c-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="be86c-113">Чтение свойств и связей объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="be86c-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="be86c-114">Обновление Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="be86c-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="be86c-115">Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="be86c-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="be86c-116">Обновление свойств объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="be86c-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="be86c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="be86c-117">Properties</span></span>
|<span data-ttu-id="be86c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="be86c-118">Property</span></span>|<span data-ttu-id="be86c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="be86c-119">Type</span></span>|<span data-ttu-id="be86c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="be86c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be86c-121">label</span><span class="sxs-lookup"><span data-stu-id="be86c-121">label</span></span>|<span data-ttu-id="be86c-122">String</span><span class="sxs-lookup"><span data-stu-id="be86c-122">String</span></span>|<span data-ttu-id="be86c-123">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="be86c-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="be86c-124">Значение по умолчанию — пустое значение.</span><span class="sxs-lookup"><span data-stu-id="be86c-124">The default value is empty.</span></span>|
|<span data-ttu-id="be86c-125">id</span><span class="sxs-lookup"><span data-stu-id="be86c-125">id</span></span>|<span data-ttu-id="be86c-126">String</span><span class="sxs-lookup"><span data-stu-id="be86c-126">String</span></span>|<span data-ttu-id="be86c-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="be86c-127">Key of the entity.</span></span>|
|<span data-ttu-id="be86c-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be86c-128">lastModifiedDateTime</span></span>|<span data-ttu-id="be86c-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be86c-129">DateTimeOffset</span></span>|<span data-ttu-id="be86c-130">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="be86c-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be86c-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="be86c-131">Relationships</span></span>
|<span data-ttu-id="be86c-132">Связь</span><span class="sxs-lookup"><span data-stu-id="be86c-132">Relationship</span></span>|<span data-ttu-id="be86c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="be86c-133">Type</span></span>|<span data-ttu-id="be86c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="be86c-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be86c-135">definition</span><span class="sxs-lookup"><span data-stu-id="be86c-135">definition</span></span>|[<span data-ttu-id="be86c-136">Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="be86c-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="be86c-137">Определение групповой политики, связанное с презентацией.</span><span class="sxs-lookup"><span data-stu-id="be86c-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be86c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be86c-138">JSON Representation</span></span>
<span data-ttu-id="be86c-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be86c-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




