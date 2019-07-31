---
title: Тип ресурса Граупполиципресентатион
description: Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7fb950a19eed475a8a9ec7f7b55aeec84e079ec5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998620"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="0d51b-103">Тип ресурса Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="0d51b-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="0d51b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d51b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d51b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d51b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d51b-106">Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.</span><span class="sxs-lookup"><span data-stu-id="0d51b-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="0d51b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0d51b-107">Methods</span></span>
|<span data-ttu-id="0d51b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0d51b-108">Method</span></span>|<span data-ttu-id="0d51b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0d51b-109">Return Type</span></span>|<span data-ttu-id="0d51b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0d51b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0d51b-111">Получение Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="0d51b-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="0d51b-112">Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="0d51b-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="0d51b-113">Чтение свойств и связей объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="0d51b-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="0d51b-114">Обновление Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="0d51b-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="0d51b-115">Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="0d51b-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="0d51b-116">Обновление свойств объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="0d51b-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0d51b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d51b-117">Properties</span></span>
|<span data-ttu-id="0d51b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d51b-118">Property</span></span>|<span data-ttu-id="0d51b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0d51b-119">Type</span></span>|<span data-ttu-id="0d51b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0d51b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d51b-121">label</span><span class="sxs-lookup"><span data-stu-id="0d51b-121">label</span></span>|<span data-ttu-id="0d51b-122">String</span><span class="sxs-lookup"><span data-stu-id="0d51b-122">String</span></span>|<span data-ttu-id="0d51b-123">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="0d51b-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="0d51b-124">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="0d51b-124">The default value is empty.</span></span>|
|<span data-ttu-id="0d51b-125">id</span><span class="sxs-lookup"><span data-stu-id="0d51b-125">id</span></span>|<span data-ttu-id="0d51b-126">String</span><span class="sxs-lookup"><span data-stu-id="0d51b-126">String</span></span>|<span data-ttu-id="0d51b-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0d51b-127">Key of the entity.</span></span>|
|<span data-ttu-id="0d51b-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d51b-128">lastModifiedDateTime</span></span>|<span data-ttu-id="0d51b-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d51b-129">DateTimeOffset</span></span>|<span data-ttu-id="0d51b-130">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0d51b-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d51b-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="0d51b-131">Relationships</span></span>
|<span data-ttu-id="0d51b-132">Отношение</span><span class="sxs-lookup"><span data-stu-id="0d51b-132">Relationship</span></span>|<span data-ttu-id="0d51b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0d51b-133">Type</span></span>|<span data-ttu-id="0d51b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0d51b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d51b-135">RDLC</span><span class="sxs-lookup"><span data-stu-id="0d51b-135">definition</span></span>|[<span data-ttu-id="0d51b-136">Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="0d51b-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="0d51b-137">Определение групповой политики, связанное с презентацией.</span><span class="sxs-lookup"><span data-stu-id="0d51b-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d51b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d51b-138">JSON Representation</span></span>
<span data-ttu-id="0d51b-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d51b-139">Here is a JSON representation of the resource.</span></span>
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





