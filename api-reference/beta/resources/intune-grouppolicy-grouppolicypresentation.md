---
title: Тип ресурса Граупполиципресентатион
description: Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: db195263c806a2e48a72f9bd7c09d0d663be584d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446929"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="6dc60-103">Тип ресурса Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="6dc60-103">groupPolicyPresentation resource type</span></span>

<span data-ttu-id="6dc60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dc60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6dc60-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dc60-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6dc60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc60-107">Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.</span><span class="sxs-lookup"><span data-stu-id="6dc60-107">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="6dc60-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6dc60-108">Methods</span></span>
|<span data-ttu-id="6dc60-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6dc60-109">Method</span></span>|<span data-ttu-id="6dc60-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6dc60-110">Return Type</span></span>|<span data-ttu-id="6dc60-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6dc60-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6dc60-112">Получение Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="6dc60-112">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="6dc60-113">граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="6dc60-113">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="6dc60-114">Чтение свойств и связей объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="6dc60-114">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="6dc60-115">Обновление Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="6dc60-115">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="6dc60-116">граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="6dc60-116">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="6dc60-117">Обновление свойств объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="6dc60-117">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6dc60-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="6dc60-118">Properties</span></span>
|<span data-ttu-id="6dc60-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="6dc60-119">Property</span></span>|<span data-ttu-id="6dc60-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6dc60-120">Type</span></span>|<span data-ttu-id="6dc60-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6dc60-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc60-122">label</span><span class="sxs-lookup"><span data-stu-id="6dc60-122">label</span></span>|<span data-ttu-id="6dc60-123">String</span><span class="sxs-lookup"><span data-stu-id="6dc60-123">String</span></span>|<span data-ttu-id="6dc60-124">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="6dc60-124">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6dc60-125">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="6dc60-125">The default value is empty.</span></span>|
|<span data-ttu-id="6dc60-126">id</span><span class="sxs-lookup"><span data-stu-id="6dc60-126">id</span></span>|<span data-ttu-id="6dc60-127">String</span><span class="sxs-lookup"><span data-stu-id="6dc60-127">String</span></span>|<span data-ttu-id="6dc60-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6dc60-128">Key of the entity.</span></span>|
|<span data-ttu-id="6dc60-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc60-129">lastModifiedDateTime</span></span>|<span data-ttu-id="6dc60-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dc60-130">DateTimeOffset</span></span>|<span data-ttu-id="6dc60-131">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6dc60-131">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dc60-132">Связи</span><span class="sxs-lookup"><span data-stu-id="6dc60-132">Relationships</span></span>
|<span data-ttu-id="6dc60-133">Связь</span><span class="sxs-lookup"><span data-stu-id="6dc60-133">Relationship</span></span>|<span data-ttu-id="6dc60-134">Тип</span><span class="sxs-lookup"><span data-stu-id="6dc60-134">Type</span></span>|<span data-ttu-id="6dc60-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6dc60-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc60-136">RDLC</span><span class="sxs-lookup"><span data-stu-id="6dc60-136">definition</span></span>|[<span data-ttu-id="6dc60-137">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="6dc60-137">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="6dc60-138">Определение групповой политики, связанное с презентацией.</span><span class="sxs-lookup"><span data-stu-id="6dc60-138">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6dc60-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6dc60-139">JSON Representation</span></span>
<span data-ttu-id="6dc60-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6dc60-140">Here is a JSON representation of the resource.</span></span>
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



