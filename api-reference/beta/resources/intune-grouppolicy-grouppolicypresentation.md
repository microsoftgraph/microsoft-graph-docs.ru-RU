---
title: Тип ресурса Граупполиципресентатион
description: Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 72f19ee5690da4a5466fa1f1902fc71729a23f01
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782997"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="32b29-103">Тип ресурса Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="32b29-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="32b29-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32b29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32b29-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32b29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32b29-106">Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.</span><span class="sxs-lookup"><span data-stu-id="32b29-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="32b29-107">Методы</span><span class="sxs-lookup"><span data-stu-id="32b29-107">Methods</span></span>
|<span data-ttu-id="32b29-108">Метод</span><span class="sxs-lookup"><span data-stu-id="32b29-108">Method</span></span>|<span data-ttu-id="32b29-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="32b29-109">Return Type</span></span>|<span data-ttu-id="32b29-110">Описание</span><span class="sxs-lookup"><span data-stu-id="32b29-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="32b29-111">Получение Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="32b29-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="32b29-112">граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="32b29-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="32b29-113">Чтение свойств и связей объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="32b29-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="32b29-114">Обновление Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="32b29-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="32b29-115">граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="32b29-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="32b29-116">Обновление свойств объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="32b29-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="32b29-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="32b29-117">Properties</span></span>
|<span data-ttu-id="32b29-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="32b29-118">Property</span></span>|<span data-ttu-id="32b29-119">Тип</span><span class="sxs-lookup"><span data-stu-id="32b29-119">Type</span></span>|<span data-ttu-id="32b29-120">Описание</span><span class="sxs-lookup"><span data-stu-id="32b29-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32b29-121">label</span><span class="sxs-lookup"><span data-stu-id="32b29-121">label</span></span>|<span data-ttu-id="32b29-122">String</span><span class="sxs-lookup"><span data-stu-id="32b29-122">String</span></span>|<span data-ttu-id="32b29-123">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="32b29-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="32b29-124">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="32b29-124">The default value is empty.</span></span>|
|<span data-ttu-id="32b29-125">id</span><span class="sxs-lookup"><span data-stu-id="32b29-125">id</span></span>|<span data-ttu-id="32b29-126">String</span><span class="sxs-lookup"><span data-stu-id="32b29-126">String</span></span>|<span data-ttu-id="32b29-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="32b29-127">Key of the entity.</span></span>|
|<span data-ttu-id="32b29-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32b29-128">lastModifiedDateTime</span></span>|<span data-ttu-id="32b29-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b29-129">DateTimeOffset</span></span>|<span data-ttu-id="32b29-130">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="32b29-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32b29-131">Связи</span><span class="sxs-lookup"><span data-stu-id="32b29-131">Relationships</span></span>
|<span data-ttu-id="32b29-132">Связь</span><span class="sxs-lookup"><span data-stu-id="32b29-132">Relationship</span></span>|<span data-ttu-id="32b29-133">Тип</span><span class="sxs-lookup"><span data-stu-id="32b29-133">Type</span></span>|<span data-ttu-id="32b29-134">Описание</span><span class="sxs-lookup"><span data-stu-id="32b29-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32b29-135">RDLC</span><span class="sxs-lookup"><span data-stu-id="32b29-135">definition</span></span>|[<span data-ttu-id="32b29-136">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="32b29-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="32b29-137">Определение групповой политики, связанное с презентацией.</span><span class="sxs-lookup"><span data-stu-id="32b29-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32b29-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32b29-138">JSON Representation</span></span>
<span data-ttu-id="32b29-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32b29-139">Here is a JSON representation of the resource.</span></span>
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



