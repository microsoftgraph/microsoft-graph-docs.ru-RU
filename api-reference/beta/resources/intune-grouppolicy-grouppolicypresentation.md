---
title: Тип ресурса Граупполиципресентатион
description: Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00151ec7c75a071df9c6485a68749cce07e6f91a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575830"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="9d315-103">Тип ресурса Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="9d315-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="9d315-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d315-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d315-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d315-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d315-106">Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.</span><span class="sxs-lookup"><span data-stu-id="9d315-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="9d315-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9d315-107">Methods</span></span>
|<span data-ttu-id="9d315-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9d315-108">Method</span></span>|<span data-ttu-id="9d315-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9d315-109">Return Type</span></span>|<span data-ttu-id="9d315-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d315-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9d315-111">Получение Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="9d315-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="9d315-112">Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="9d315-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="9d315-113">Чтение свойств и связей объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="9d315-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="9d315-114">Обновление Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="9d315-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="9d315-115">Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="9d315-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="9d315-116">Обновление свойств объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="9d315-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9d315-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d315-117">Properties</span></span>
|<span data-ttu-id="9d315-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d315-118">Property</span></span>|<span data-ttu-id="9d315-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9d315-119">Type</span></span>|<span data-ttu-id="9d315-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9d315-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d315-121">label</span><span class="sxs-lookup"><span data-stu-id="9d315-121">label</span></span>|<span data-ttu-id="9d315-122">String</span><span class="sxs-lookup"><span data-stu-id="9d315-122">String</span></span>|<span data-ttu-id="9d315-123">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="9d315-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9d315-124">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="9d315-124">The default value is empty.</span></span>|
|<span data-ttu-id="9d315-125">id</span><span class="sxs-lookup"><span data-stu-id="9d315-125">id</span></span>|<span data-ttu-id="9d315-126">String</span><span class="sxs-lookup"><span data-stu-id="9d315-126">String</span></span>|<span data-ttu-id="9d315-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d315-127">Key of the entity.</span></span>|
|<span data-ttu-id="9d315-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d315-128">lastModifiedDateTime</span></span>|<span data-ttu-id="9d315-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d315-129">DateTimeOffset</span></span>|<span data-ttu-id="9d315-130">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9d315-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d315-131">Связи</span><span class="sxs-lookup"><span data-stu-id="9d315-131">Relationships</span></span>
|<span data-ttu-id="9d315-132">Отношение</span><span class="sxs-lookup"><span data-stu-id="9d315-132">Relationship</span></span>|<span data-ttu-id="9d315-133">Тип</span><span class="sxs-lookup"><span data-stu-id="9d315-133">Type</span></span>|<span data-ttu-id="9d315-134">Описание</span><span class="sxs-lookup"><span data-stu-id="9d315-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d315-135">RDLC</span><span class="sxs-lookup"><span data-stu-id="9d315-135">definition</span></span>|[<span data-ttu-id="9d315-136">Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="9d315-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9d315-137">Определение групповой политики, связанное с презентацией.</span><span class="sxs-lookup"><span data-stu-id="9d315-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d315-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d315-138">JSON Representation</span></span>
<span data-ttu-id="9d315-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d315-139">Here is a JSON representation of the resource.</span></span>
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





