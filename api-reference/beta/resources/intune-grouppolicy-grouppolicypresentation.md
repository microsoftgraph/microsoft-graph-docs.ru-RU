---
title: Тип ресурса groupPolicyPresentation
description: Базовая сущность для отображения представления Дополнительные параметры в определении групповой политики.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 736b599eaf310bc63530daa45ffa1aee7ede4c3f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430867"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="99c9e-103">Тип ресурса groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="99c9e-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="99c9e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99c9e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99c9e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99c9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99c9e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99c9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99c9e-107">Базовая сущность для отображения представления Дополнительные параметры в определении групповой политики.</span><span class="sxs-lookup"><span data-stu-id="99c9e-107">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="99c9e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="99c9e-108">Methods</span></span>
|<span data-ttu-id="99c9e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="99c9e-109">Method</span></span>|<span data-ttu-id="99c9e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="99c9e-110">Return Type</span></span>|<span data-ttu-id="99c9e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="99c9e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="99c9e-112">Получение groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="99c9e-112">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="99c9e-113">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="99c9e-113">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="99c9e-114">Чтение свойства и связи объекта [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="99c9e-114">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="99c9e-115">Обновление groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="99c9e-115">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="99c9e-116">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="99c9e-116">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="99c9e-117">Обновление свойства объекта [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="99c9e-117">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="99c9e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="99c9e-118">Properties</span></span>
|<span data-ttu-id="99c9e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="99c9e-119">Property</span></span>|<span data-ttu-id="99c9e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="99c9e-120">Type</span></span>|<span data-ttu-id="99c9e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="99c9e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c9e-122">label</span><span class="sxs-lookup"><span data-stu-id="99c9e-122">label</span></span>|<span data-ttu-id="99c9e-123">String</span><span class="sxs-lookup"><span data-stu-id="99c9e-123">String</span></span>|<span data-ttu-id="99c9e-124">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="99c9e-124">Localized text label for any presentation entity.</span></span> <span data-ttu-id="99c9e-125">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="99c9e-125">The default value is empty.</span></span>|
|<span data-ttu-id="99c9e-126">id</span><span class="sxs-lookup"><span data-stu-id="99c9e-126">id</span></span>|<span data-ttu-id="99c9e-127">String</span><span class="sxs-lookup"><span data-stu-id="99c9e-127">String</span></span>|<span data-ttu-id="99c9e-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="99c9e-128">Key of the entity.</span></span>|
|<span data-ttu-id="99c9e-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99c9e-129">lastModifiedDateTime</span></span>|<span data-ttu-id="99c9e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99c9e-130">DateTimeOffset</span></span>|<span data-ttu-id="99c9e-131">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="99c9e-131">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99c9e-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="99c9e-132">Relationships</span></span>
|<span data-ttu-id="99c9e-133">Связь</span><span class="sxs-lookup"><span data-stu-id="99c9e-133">Relationship</span></span>|<span data-ttu-id="99c9e-134">Тип</span><span class="sxs-lookup"><span data-stu-id="99c9e-134">Type</span></span>|<span data-ttu-id="99c9e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="99c9e-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c9e-136">definition</span><span class="sxs-lookup"><span data-stu-id="99c9e-136">definition</span></span>|[<span data-ttu-id="99c9e-137">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="99c9e-137">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="99c9e-138">Определение политики группы, связанные с презентации.</span><span class="sxs-lookup"><span data-stu-id="99c9e-138">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99c9e-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99c9e-139">JSON Representation</span></span>
<span data-ttu-id="99c9e-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99c9e-140">Here is a JSON representation of the resource.</span></span>
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




